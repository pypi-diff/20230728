# Comparing `tmp/mypy-boto3-iotwireless-1.28.12.tar.gz` & `tmp/mypy-boto3-iotwireless-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotwireless-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-iotwireless-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-iotwireless-1.28.12.tar` & `mypy-boto3-iotwireless-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27301 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25798 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.408475 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72150 2023-07-27 05:24:20.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    72034 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-27 05:24:20.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-27 05:24:20.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   110665 2023-07-27 05:24:22.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   110572 2023-07-27 05:24:21.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27301 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.553299 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72150 2023-07-28 20:28:47.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72034 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-28 20:28:47.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-28 20:28:47.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   101165 2023-07-28 20:28:52.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101072 2023-07-28 20:28:50.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotwireless-1.28.12/LICENSE` & `mypy-boto3-iotwireless-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.12/PKG-INFO` & `mypy-boto3-iotwireless-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iotwireless
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTWireless 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotwireless type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-iotwireless"></a>
 
 # mypy-boto3-iotwireless
 
 [![PyPI - mypy-boto3-iotwireless](https://img.shields.io/pypi/v/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,58 +303,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
-    SessionKeysAbpV10XOutputTypeDef,
     SessionKeysAbpV10XTypeDef,
-    SessionKeysAbpV11OutputTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
-    ApplicationConfigOutputTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
-    SidewalkAccountInfoOutputTypeDef,
+    ResponseMetadataTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
-    AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
     BeaconingOutputTypeDef,
     BeaconingTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
-    LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
-    LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
-    CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
-    CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
-    CreateMulticastGroupResponseTypeDef,
     TraceContentTypeDef,
-    CreateNetworkAnalyzerConfigurationResponseTypeDef,
     LoRaWANServiceProfileTypeDef,
-    CreateServiceProfileResponseTypeDef,
     SidewalkCreateWirelessDeviceTypeDef,
-    CreateWirelessDeviceResponseTypeDef,
-    CreateWirelessGatewayResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
     CreateWirelessGatewayTaskRequestRequestTypeDef,
-    CreateWirelessGatewayTaskResponseTypeDef,
     DakCertificateMetadataTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteDeviceProfileRequestRequestTypeDef,
     DeleteFuotaTaskRequestRequestTypeDef,
     DeleteMulticastGroupRequestRequestTypeDef,
     DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef,
     DeleteQueuedMessagesRequestRequestTypeDef,
@@ -395,79 +347,64 @@
     DeleteWirelessDeviceRequestRequestTypeDef,
     DeleteWirelessGatewayRequestRequestTypeDef,
     DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     DeleteWirelessGatewayTaskRequestRequestTypeDef,
     DeregisterWirelessDeviceRequestRequestTypeDef,
     DestinationsTypeDef,
     DeviceProfileTypeDef,
-    SidewalkEventNotificationConfigurationsOutputTypeDef,
     SidewalkEventNotificationConfigurationsTypeDef,
-    SidewalkResourceTypeEventConfigurationOutputTypeDef,
     SidewalkResourceTypeEventConfigurationTypeDef,
     DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef,
     DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
-    PositioningOutputTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
-    GatewayListItemOutputTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
     LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
     LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
-    TraceContentOutputTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
     WiFiAccessPointTypeDef,
-    GetPositionEstimateResponseTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
-    GetResourceLogLevelResponseTypeDef,
     GetResourcePositionRequestRequestTypeDef,
-    GetResourcePositionResponseTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
-    GetServiceEndpointResponseTypeDef,
     GetServiceProfileRequestRequestTypeDef,
     LoRaWANGetServiceProfileInfoTypeDef,
     GetWirelessDeviceImportTaskRequestRequestTypeDef,
     SidewalkGetStartImportInfoTypeDef,
     GetWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceStatisticsRequestRequestTypeDef,
     SidewalkDeviceMetadataTypeDef,
     GetWirelessGatewayCertificateRequestRequestTypeDef,
-    GetWirelessGatewayCertificateResponseTypeDef,
     GetWirelessGatewayFirmwareInformationRequestRequestTypeDef,
     GetWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayStatisticsRequestRequestTypeDef,
-    GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
-    GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
-    LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
-    LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
     ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     ListEventConfigurationsRequestRequestTypeDef,
     ListFuotaTasksRequestRequestTypeDef,
     ListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
@@ -478,137 +415,136 @@
     NetworkAnalyzerConfigurationsTypeDef,
     ListPartnerAccountsRequestRequestTypeDef,
     ListPositionConfigurationsRequestRequestTypeDef,
     ListQueuedMessagesRequestRequestTypeDef,
     ListServiceProfilesRequestRequestTypeDef,
     ServiceProfileTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListWirelessDeviceImportTasksRequestRequestTypeDef,
     ListWirelessDevicesRequestRequestTypeDef,
     ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef,
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
-    OtaaV10XOutputTypeDef,
-    OtaaV11OutputTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
-    LoRaWANGatewayVersionOutputTypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
     LoRaWANMulticastSessionTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
     ResetResourceLogLevelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendDataToMulticastGroupResponseTypeDef,
-    SendDataToWirelessDeviceResponseTypeDef,
     SidewalkSendDataToDeviceTypeDef,
     SidewalkSingleStartImportInfoTypeDef,
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
-    StartSingleWirelessDeviceImportTaskResponseTypeDef,
-    StartWirelessDeviceImportTaskResponseTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
-    TestWirelessDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
     UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
-    WirelessDeviceEventLogOptionOutputTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
-    WirelessGatewayEventLogOptionOutputTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
-    AbpV10XOutputTypeDef,
     AbpV10XTypeDef,
-    AbpV11OutputTypeDef,
     AbpV11TypeDef,
-    GetPositionResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateDeviceProfileResponseTypeDef,
+    CreateFuotaTaskResponseTypeDef,
+    CreateMulticastGroupResponseTypeDef,
+    CreateNetworkAnalyzerConfigurationResponseTypeDef,
+    CreateServiceProfileResponseTypeDef,
+    CreateWirelessDeviceResponseTypeDef,
+    CreateWirelessGatewayResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
+    CreateWirelessGatewayTaskResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetPositionEstimateResponseTypeDef,
+    GetPositionResponseTypeDef,
+    GetResourceLogLevelResponseTypeDef,
+    GetResourcePositionResponseTypeDef,
+    GetServiceEndpointResponseTypeDef,
+    GetWirelessGatewayCertificateResponseTypeDef,
+    GetWirelessGatewayStatisticsResponseTypeDef,
+    GetWirelessGatewayTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendDataToMulticastGroupResponseTypeDef,
+    SendDataToWirelessDeviceResponseTypeDef,
+    StartSingleWirelessDeviceImportTaskResponseTypeDef,
+    StartWirelessDeviceImportTaskResponseTypeDef,
+    TestWirelessDeviceResponseTypeDef,
     LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
-    ConnectionStatusEventConfigurationOutputTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
-    ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
     UpdateFuotaTaskRequestRequestTypeDef,
     CreateMulticastGroupRequestRequestTypeDef,
     UpdateMulticastGroupRequestRequestTypeDef,
     CreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
+    GetNetworkAnalyzerConfigurationResponseTypeDef,
     UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     CreateServiceProfileRequestRequestTypeDef,
     SidewalkGetDeviceProfileTypeDef,
     ListDestinationsResponseTypeDef,
     ListDeviceProfilesResponseTypeDef,
-    DeviceRegistrationStateEventConfigurationOutputTypeDef,
-    MessageDeliveryStatusEventConfigurationOutputTypeDef,
-    ProximityEventConfigurationOutputTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
-    DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef,
-    MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
-    ProximityResourceTypeEventConfigurationOutputTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
     FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
     ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    GetNetworkAnalyzerConfigurationResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
-    JoinEventConfigurationOutputTypeDef,
     JoinEventConfigurationTypeDef,
-    JoinResourceTypeEventConfigurationOutputTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
     ListMulticastGroupsByFuotaTaskResponseTypeDef,
     ListMulticastGroupsResponseTypeDef,
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
-    LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
-    LoRaWANUpdateGatewayTaskEntryTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
+    LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
     StartMulticastGroupSessionRequestRequestTypeDef,
     StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
@@ -637,17 +573,16 @@
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
     UpdateEventConfigurationByResourceTypesRequestRequestTypeDef,
     GetWirelessDeviceStatisticsResponseTypeDef,
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
-    UpdateWirelessGatewayTaskCreateOutputTypeDef,
-    UpdateWirelessGatewayTaskEntryTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
+    UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
     UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListWirelessGatewaysResponseTypeDef,
@@ -655,26 +590,26 @@
     GetWirelessDeviceResponseTypeDef,
     CreateWirelessDeviceRequestRequestTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
+    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     ListPositionConfigurationsResponseTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XOutputTypeDef:
+def get_structure() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.12/README.md` & `mypy-boto3-iotwireless-1.28.15/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iotwireless
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iotwireless type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-iotwireless"></a>
 
 # mypy-boto3-iotwireless
 
 [![PyPI - mypy-boto3-iotwireless](https://img.shields.io/pypi/v/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,58 +335,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
-    SessionKeysAbpV10XOutputTypeDef,
     SessionKeysAbpV10XTypeDef,
-    SessionKeysAbpV11OutputTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
-    ApplicationConfigOutputTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
-    SidewalkAccountInfoOutputTypeDef,
+    ResponseMetadataTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
-    AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
     BeaconingOutputTypeDef,
     BeaconingTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
-    LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
-    LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
-    CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
-    CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
-    CreateMulticastGroupResponseTypeDef,
     TraceContentTypeDef,
-    CreateNetworkAnalyzerConfigurationResponseTypeDef,
     LoRaWANServiceProfileTypeDef,
-    CreateServiceProfileResponseTypeDef,
     SidewalkCreateWirelessDeviceTypeDef,
-    CreateWirelessDeviceResponseTypeDef,
-    CreateWirelessGatewayResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
     CreateWirelessGatewayTaskRequestRequestTypeDef,
-    CreateWirelessGatewayTaskResponseTypeDef,
     DakCertificateMetadataTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteDeviceProfileRequestRequestTypeDef,
     DeleteFuotaTaskRequestRequestTypeDef,
     DeleteMulticastGroupRequestRequestTypeDef,
     DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef,
     DeleteQueuedMessagesRequestRequestTypeDef,
@@ -363,79 +379,64 @@
     DeleteWirelessDeviceRequestRequestTypeDef,
     DeleteWirelessGatewayRequestRequestTypeDef,
     DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     DeleteWirelessGatewayTaskRequestRequestTypeDef,
     DeregisterWirelessDeviceRequestRequestTypeDef,
     DestinationsTypeDef,
     DeviceProfileTypeDef,
-    SidewalkEventNotificationConfigurationsOutputTypeDef,
     SidewalkEventNotificationConfigurationsTypeDef,
-    SidewalkResourceTypeEventConfigurationOutputTypeDef,
     SidewalkResourceTypeEventConfigurationTypeDef,
     DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef,
     DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
-    PositioningOutputTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
-    GatewayListItemOutputTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
     LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
     LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
-    TraceContentOutputTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
     WiFiAccessPointTypeDef,
-    GetPositionEstimateResponseTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
-    GetResourceLogLevelResponseTypeDef,
     GetResourcePositionRequestRequestTypeDef,
-    GetResourcePositionResponseTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
-    GetServiceEndpointResponseTypeDef,
     GetServiceProfileRequestRequestTypeDef,
     LoRaWANGetServiceProfileInfoTypeDef,
     GetWirelessDeviceImportTaskRequestRequestTypeDef,
     SidewalkGetStartImportInfoTypeDef,
     GetWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceStatisticsRequestRequestTypeDef,
     SidewalkDeviceMetadataTypeDef,
     GetWirelessGatewayCertificateRequestRequestTypeDef,
-    GetWirelessGatewayCertificateResponseTypeDef,
     GetWirelessGatewayFirmwareInformationRequestRequestTypeDef,
     GetWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayStatisticsRequestRequestTypeDef,
-    GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
-    GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
-    LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
-    LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
     ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     ListEventConfigurationsRequestRequestTypeDef,
     ListFuotaTasksRequestRequestTypeDef,
     ListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
@@ -446,137 +447,136 @@
     NetworkAnalyzerConfigurationsTypeDef,
     ListPartnerAccountsRequestRequestTypeDef,
     ListPositionConfigurationsRequestRequestTypeDef,
     ListQueuedMessagesRequestRequestTypeDef,
     ListServiceProfilesRequestRequestTypeDef,
     ServiceProfileTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListWirelessDeviceImportTasksRequestRequestTypeDef,
     ListWirelessDevicesRequestRequestTypeDef,
     ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef,
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
-    OtaaV10XOutputTypeDef,
-    OtaaV11OutputTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
-    LoRaWANGatewayVersionOutputTypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
     LoRaWANMulticastSessionTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
     ResetResourceLogLevelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendDataToMulticastGroupResponseTypeDef,
-    SendDataToWirelessDeviceResponseTypeDef,
     SidewalkSendDataToDeviceTypeDef,
     SidewalkSingleStartImportInfoTypeDef,
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
-    StartSingleWirelessDeviceImportTaskResponseTypeDef,
-    StartWirelessDeviceImportTaskResponseTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
-    TestWirelessDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
     UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
-    WirelessDeviceEventLogOptionOutputTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
-    WirelessGatewayEventLogOptionOutputTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
-    AbpV10XOutputTypeDef,
     AbpV10XTypeDef,
-    AbpV11OutputTypeDef,
     AbpV11TypeDef,
-    GetPositionResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateDeviceProfileResponseTypeDef,
+    CreateFuotaTaskResponseTypeDef,
+    CreateMulticastGroupResponseTypeDef,
+    CreateNetworkAnalyzerConfigurationResponseTypeDef,
+    CreateServiceProfileResponseTypeDef,
+    CreateWirelessDeviceResponseTypeDef,
+    CreateWirelessGatewayResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
+    CreateWirelessGatewayTaskResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetPositionEstimateResponseTypeDef,
+    GetPositionResponseTypeDef,
+    GetResourceLogLevelResponseTypeDef,
+    GetResourcePositionResponseTypeDef,
+    GetServiceEndpointResponseTypeDef,
+    GetWirelessGatewayCertificateResponseTypeDef,
+    GetWirelessGatewayStatisticsResponseTypeDef,
+    GetWirelessGatewayTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendDataToMulticastGroupResponseTypeDef,
+    SendDataToWirelessDeviceResponseTypeDef,
+    StartSingleWirelessDeviceImportTaskResponseTypeDef,
+    StartWirelessDeviceImportTaskResponseTypeDef,
+    TestWirelessDeviceResponseTypeDef,
     LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
-    ConnectionStatusEventConfigurationOutputTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
-    ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
     UpdateFuotaTaskRequestRequestTypeDef,
     CreateMulticastGroupRequestRequestTypeDef,
     UpdateMulticastGroupRequestRequestTypeDef,
     CreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
+    GetNetworkAnalyzerConfigurationResponseTypeDef,
     UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     CreateServiceProfileRequestRequestTypeDef,
     SidewalkGetDeviceProfileTypeDef,
     ListDestinationsResponseTypeDef,
     ListDeviceProfilesResponseTypeDef,
-    DeviceRegistrationStateEventConfigurationOutputTypeDef,
-    MessageDeliveryStatusEventConfigurationOutputTypeDef,
-    ProximityEventConfigurationOutputTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
-    DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef,
-    MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
-    ProximityResourceTypeEventConfigurationOutputTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
     FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
     ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    GetNetworkAnalyzerConfigurationResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
-    JoinEventConfigurationOutputTypeDef,
     JoinEventConfigurationTypeDef,
-    JoinResourceTypeEventConfigurationOutputTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
     ListMulticastGroupsByFuotaTaskResponseTypeDef,
     ListMulticastGroupsResponseTypeDef,
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
-    LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
-    LoRaWANUpdateGatewayTaskEntryTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
+    LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
     StartMulticastGroupSessionRequestRequestTypeDef,
     StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
@@ -605,17 +605,16 @@
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
     UpdateEventConfigurationByResourceTypesRequestRequestTypeDef,
     GetWirelessDeviceStatisticsResponseTypeDef,
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
-    UpdateWirelessGatewayTaskCreateOutputTypeDef,
-    UpdateWirelessGatewayTaskEntryTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
+    UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
     UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListWirelessGatewaysResponseTypeDef,
@@ -623,26 +622,26 @@
     GetWirelessDeviceResponseTypeDef,
     CreateWirelessDeviceRequestRequestTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
+    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     ListPositionConfigurationsResponseTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XOutputTypeDef:
+def get_structure() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__main__.py` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTWireless 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTWireless 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
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

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.py` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.pyi` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.py` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.pyi` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.py` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotwireless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XOutputTypeDef
+    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
 
-    data: SessionKeysAbpV10XOutputTypeDef = {...}
+    data: SessionKeysAbpV10XTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -60,58 +60,42 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "SessionKeysAbpV10XOutputTypeDef",
     "SessionKeysAbpV10XTypeDef",
-    "SessionKeysAbpV11OutputTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
-    "ApplicationConfigOutputTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
-    "SidewalkAccountInfoOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
-    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
-    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
-    "CreateDestinationResponseTypeDef",
     "LoRaWANDeviceProfileTypeDef",
-    "CreateDeviceProfileResponseTypeDef",
     "LoRaWANFuotaTaskTypeDef",
-    "CreateFuotaTaskResponseTypeDef",
     "LoRaWANMulticastTypeDef",
-    "CreateMulticastGroupResponseTypeDef",
     "TraceContentTypeDef",
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
     "LoRaWANServiceProfileTypeDef",
-    "CreateServiceProfileResponseTypeDef",
     "SidewalkCreateWirelessDeviceTypeDef",
-    "CreateWirelessDeviceResponseTypeDef",
-    "CreateWirelessGatewayResponseTypeDef",
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
-    "CreateWirelessGatewayTaskResponseTypeDef",
     "DakCertificateMetadataTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteDeviceProfileRequestRequestTypeDef",
     "DeleteFuotaTaskRequestRequestTypeDef",
     "DeleteMulticastGroupRequestRequestTypeDef",
     "DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "DeleteQueuedMessagesRequestRequestTypeDef",
@@ -120,79 +104,64 @@
     "DeleteWirelessDeviceRequestRequestTypeDef",
     "DeleteWirelessGatewayRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskRequestRequestTypeDef",
     "DeregisterWirelessDeviceRequestRequestTypeDef",
     "DestinationsTypeDef",
     "DeviceProfileTypeDef",
-    "SidewalkEventNotificationConfigurationsOutputTypeDef",
     "SidewalkEventNotificationConfigurationsTypeDef",
-    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
     "SidewalkResourceTypeEventConfigurationTypeDef",
     "DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef",
     "DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromThingRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
-    "PositioningOutputTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
-    "GatewayListItemOutputTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
     "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
     "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
-    "TraceContentOutputTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
     "WiFiAccessPointTypeDef",
-    "GetPositionEstimateResponseTypeDef",
     "GetPositionRequestRequestTypeDef",
     "GetResourceEventConfigurationRequestRequestTypeDef",
     "GetResourceLogLevelRequestRequestTypeDef",
-    "GetResourceLogLevelResponseTypeDef",
     "GetResourcePositionRequestRequestTypeDef",
-    "GetResourcePositionResponseTypeDef",
     "GetServiceEndpointRequestRequestTypeDef",
-    "GetServiceEndpointResponseTypeDef",
     "GetServiceProfileRequestRequestTypeDef",
     "LoRaWANGetServiceProfileInfoTypeDef",
     "GetWirelessDeviceImportTaskRequestRequestTypeDef",
     "SidewalkGetStartImportInfoTypeDef",
     "GetWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsRequestRequestTypeDef",
     "SidewalkDeviceMetadataTypeDef",
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
-    "GetWirelessGatewayCertificateResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     "GetWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
-    "GetWirelessGatewayStatisticsResponseTypeDef",
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskRequestRequestTypeDef",
-    "GetWirelessGatewayTaskResponseTypeDef",
     "GlobalIdentityTypeDef",
     "GsmLocalIdTypeDef",
     "ImportedSidewalkDeviceTypeDef",
-    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
-    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListDeviceProfilesRequestRequestTypeDef",
     "ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef",
     "ListEventConfigurationsRequestRequestTypeDef",
     "ListFuotaTasksRequestRequestTypeDef",
     "ListMulticastGroupsByFuotaTaskRequestRequestTypeDef",
@@ -203,137 +172,136 @@
     "NetworkAnalyzerConfigurationsTypeDef",
     "ListPartnerAccountsRequestRequestTypeDef",
     "ListPositionConfigurationsRequestRequestTypeDef",
     "ListQueuedMessagesRequestRequestTypeDef",
     "ListServiceProfilesRequestRequestTypeDef",
     "ServiceProfileTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     "ListWirelessDevicesRequestRequestTypeDef",
     "ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef",
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
-    "OtaaV10XOutputTypeDef",
-    "OtaaV11OutputTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
-    "LoRaWANGatewayVersionOutputTypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
     "LoRaWANMulticastSessionTypeDef",
     "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
     "PutResourceLogLevelRequestRequestTypeDef",
     "ResetResourceLogLevelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendDataToMulticastGroupResponseTypeDef",
-    "SendDataToWirelessDeviceResponseTypeDef",
     "SidewalkSendDataToDeviceTypeDef",
     "SidewalkSingleStartImportInfoTypeDef",
     "SidewalkStartImportInfoTypeDef",
     "SidewalkUpdateAccountTypeDef",
     "SidewalkUpdateImportInfoTypeDef",
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    "StartWirelessDeviceImportTaskResponseTypeDef",
     "TdscdmaLocalIdTypeDef",
     "TdscdmaNmrObjTypeDef",
     "TestWirelessDeviceRequestRequestTypeDef",
-    "TestWirelessDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
     "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
-    "WirelessDeviceEventLogOptionOutputTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
-    "WirelessGatewayEventLogOptionOutputTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
-    "AbpV10XOutputTypeDef",
     "AbpV10XTypeDef",
-    "AbpV11OutputTypeDef",
     "AbpV11TypeDef",
-    "GetPositionResponseTypeDef",
     "AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     "CreateDestinationRequestRequestTypeDef",
     "StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateDeviceProfileResponseTypeDef",
+    "CreateFuotaTaskResponseTypeDef",
+    "CreateMulticastGroupResponseTypeDef",
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    "CreateServiceProfileResponseTypeDef",
+    "CreateWirelessDeviceResponseTypeDef",
+    "CreateWirelessGatewayResponseTypeDef",
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetPositionEstimateResponseTypeDef",
+    "GetPositionResponseTypeDef",
+    "GetResourceLogLevelResponseTypeDef",
+    "GetResourcePositionResponseTypeDef",
+    "GetServiceEndpointResponseTypeDef",
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    "GetWirelessGatewayTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SendDataToMulticastGroupResponseTypeDef",
+    "SendDataToWirelessDeviceResponseTypeDef",
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    "TestWirelessDeviceResponseTypeDef",
     "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
-    "ConnectionStatusEventConfigurationOutputTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
-    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
     "UpdateFuotaTaskRequestRequestTypeDef",
     "CreateMulticastGroupRequestRequestTypeDef",
     "UpdateMulticastGroupRequestRequestTypeDef",
     "CreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "CreateServiceProfileRequestRequestTypeDef",
     "SidewalkGetDeviceProfileTypeDef",
     "ListDestinationsResponseTypeDef",
     "ListDeviceProfilesResponseTypeDef",
-    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
-    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
-    "ProximityEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
-    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
-    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
-    "ProximityResourceTypeEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
     "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
     "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
-    "JoinEventConfigurationOutputTypeDef",
     "JoinEventConfigurationTypeDef",
-    "JoinResourceTypeEventConfigurationOutputTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     "ListMulticastGroupsResponseTypeDef",
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
-    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
-    "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "LoRaWANUpdateGatewayTaskCreateTypeDef",
+    "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "MulticastWirelessMetadataTypeDef",
     "StartMulticastGroupSessionRequestRequestTypeDef",
     "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
@@ -362,17 +330,16 @@
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
-    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
-    "UpdateWirelessGatewayTaskEntryTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
+    "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
@@ -380,53 +347,33 @@
     "GetWirelessDeviceResponseTypeDef",
     "CreateWirelessDeviceRequestRequestTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
+    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
-    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
-SessionKeysAbpV10XOutputTypeDef = TypedDict(
-    "SessionKeysAbpV10XOutputTypeDef",
-    {
-        "NwkSKey": str,
-        "AppSKey": str,
-    },
-    total=False,
-)
-
 SessionKeysAbpV10XTypeDef = TypedDict(
     "SessionKeysAbpV10XTypeDef",
     {
         "NwkSKey": str,
         "AppSKey": str,
     },
     total=False,
 )
 
-SessionKeysAbpV11OutputTypeDef = TypedDict(
-    "SessionKeysAbpV11OutputTypeDef",
-    {
-        "FNwkSIntKey": str,
-        "SNwkSIntKey": str,
-        "NwkSEncKey": str,
-        "AppSKey": str,
-    },
-    total=False,
-)
-
 SessionKeysAbpV11TypeDef = TypedDict(
     "SessionKeysAbpV11TypeDef",
     {
         "FNwkSIntKey": str,
         "SNwkSIntKey": str,
         "NwkSEncKey": str,
         "AppSKey": str,
@@ -439,24 +386,14 @@
     {
         "HorizontalAccuracy": float,
         "VerticalAccuracy": float,
     },
     total=False,
 )
 
-ApplicationConfigOutputTypeDef = TypedDict(
-    "ApplicationConfigOutputTypeDef",
-    {
-        "FPort": int,
-        "Type": Literal["SemtechGeolocation"],
-        "DestinationName": str,
-    },
-    total=False,
-)
-
 ApplicationConfigTypeDef = TypedDict(
     "ApplicationConfigTypeDef",
     {
         "FPort": int,
         "Type": Literal["SemtechGeolocation"],
         "DestinationName": str,
     },
@@ -476,21 +413,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-SidewalkAccountInfoOutputTypeDef = TypedDict(
-    "SidewalkAccountInfoOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AmazonId": str,
-        "AppServerPrivateKey": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = TypedDict(
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
         "MulticastGroupId": str,
@@ -525,22 +464,14 @@
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     {
         "Id": str,
         "IotCertificateId": str,
     },
 )
 
-AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateWirelessGatewayWithThingRequestRequestTypeDef = TypedDict(
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
@@ -603,55 +534,30 @@
     "CertificateListTypeDef",
     {
         "SigningAlg": SigningAlgType,
         "Value": str,
     },
 )
 
-LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef = TypedDict(
-    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
-    {
-        "GatewayEuiEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     {
         "GatewayEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANDeviceProfileTypeDef = TypedDict(
     "LoRaWANDeviceProfileTypeDef",
     {
         "SupportsClassB": bool,
         "ClassBTimeout": int,
         "PingSlotPeriod": int,
         "PingSlotDr": int,
@@ -670,150 +576,69 @@
         "RfRegion": str,
         "SupportsJoin": bool,
         "Supports32BitFCnt": bool,
     },
     total=False,
 )
 
-CreateDeviceProfileResponseTypeDef = TypedDict(
-    "CreateDeviceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANFuotaTaskTypeDef = TypedDict(
     "LoRaWANFuotaTaskTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
     },
     total=False,
 )
 
-CreateFuotaTaskResponseTypeDef = TypedDict(
-    "CreateFuotaTaskResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANMulticastTypeDef = TypedDict(
     "LoRaWANMulticastTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
         "DlClass": DlClassType,
     },
     total=False,
 )
 
-CreateMulticastGroupResponseTypeDef = TypedDict(
-    "CreateMulticastGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TraceContentTypeDef = TypedDict(
     "TraceContentTypeDef",
     {
         "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
         "LogLevel": LogLevelType,
         "MulticastFrameInfo": MulticastFrameInfoType,
     },
     total=False,
 )
 
-CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANServiceProfileTypeDef = TypedDict(
     "LoRaWANServiceProfileTypeDef",
     {
         "AddGwMetadata": bool,
         "DrMin": int,
         "DrMax": int,
         "PrAllowed": bool,
         "RaAllowed": bool,
     },
     total=False,
 )
 
-CreateServiceProfileResponseTypeDef = TypedDict(
-    "CreateServiceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkCreateWirelessDeviceTypeDef = TypedDict(
     "SidewalkCreateWirelessDeviceTypeDef",
     {
         "DeviceProfileId": str,
     },
     total=False,
 )
 
-CreateWirelessDeviceResponseTypeDef = TypedDict(
-    "CreateWirelessDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
         "WirelessGatewayTaskDefinitionId": str,
     },
 )
 
-CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayTaskDefinitionId": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDakCertificateMetadataTypeDef = TypedDict(
     "_RequiredDakCertificateMetadataTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalDakCertificateMetadataTypeDef = TypedDict(
@@ -975,38 +800,22 @@
         "Arn": str,
         "Name": str,
         "Id": str,
     },
     total=False,
 )
 
-SidewalkEventNotificationConfigurationsOutputTypeDef = TypedDict(
-    "SidewalkEventNotificationConfigurationsOutputTypeDef",
-    {
-        "AmazonIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 SidewalkEventNotificationConfigurationsTypeDef = TypedDict(
     "SidewalkEventNotificationConfigurationsTypeDef",
     {
         "AmazonIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-SidewalkResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 SidewalkResourceTypeEventConfigurationTypeDef = TypedDict(
     "SidewalkResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -1060,24 +869,14 @@
 DisassociateWirelessGatewayFromThingRequestRequestTypeDef = TypedDict(
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-PositioningOutputTypeDef = TypedDict(
-    "PositioningOutputTypeDef",
-    {
-        "ClockSync": int,
-        "Stream": int,
-        "Gnss": int,
-    },
-    total=False,
-)
-
 PositioningTypeDef = TypedDict(
     "PositioningTypeDef",
     {
         "ClockSync": int,
         "Stream": int,
         "Gnss": int,
     },
@@ -1090,22 +889,14 @@
         "Id": str,
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
-GatewayListItemOutputTypeDef = TypedDict(
-    "GatewayListItemOutputTypeDef",
-    {
-        "GatewayId": str,
-        "DownlinkFrequency": int,
-    },
-)
-
 GatewayListItemTypeDef = TypedDict(
     "GatewayListItemTypeDef",
     {
         "GatewayId": str,
         "DownlinkFrequency": int,
     },
 )
@@ -1113,27 +904,14 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Expression": str,
-        "ExpressionType": ExpressionTypeType,
-        "Description": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeviceProfileRequestRequestTypeDef = TypedDict(
     "GetDeviceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1219,24 +997,14 @@
 GetNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 
-TraceContentOutputTypeDef = TypedDict(
-    "TraceContentOutputTypeDef",
-    {
-        "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
-        "LogLevel": LogLevelType,
-        "MulticastFrameInfo": MulticastFrameInfoType,
-    },
-    total=False,
-)
-
 GetPartnerAccountRequestRequestTypeDef = TypedDict(
     "GetPartnerAccountRequestRequestTypeDef",
     {
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
 )
@@ -1293,22 +1061,14 @@
     "WiFiAccessPointTypeDef",
     {
         "MacAddress": str,
         "Rss": int,
     },
 )
 
-GetPositionEstimateResponseTypeDef = TypedDict(
-    "GetPositionEstimateResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPositionRequestRequestTypeDef = TypedDict(
     "GetPositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
@@ -1340,56 +1100,30 @@
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
 
-GetResourceLogLevelResponseTypeDef = TypedDict(
-    "GetResourceLogLevelResponseTypeDef",
-    {
-        "LogLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePositionRequestRequestTypeDef = TypedDict(
     "GetResourcePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
 
-GetResourcePositionResponseTypeDef = TypedDict(
-    "GetResourcePositionResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceEndpointRequestRequestTypeDef = TypedDict(
     "GetServiceEndpointRequestRequestTypeDef",
     {
         "ServiceType": WirelessGatewayServiceTypeType,
     },
     total=False,
 )
 
-GetServiceEndpointResponseTypeDef = TypedDict(
-    "GetServiceEndpointResponseTypeDef",
-    {
-        "ServiceType": WirelessGatewayServiceTypeType,
-        "ServiceEndpoint": str,
-        "ServerTrust": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceProfileRequestRequestTypeDef = TypedDict(
     "GetServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1464,23 +1198,14 @@
 GetWirelessGatewayCertificateRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
-    "GetWirelessGatewayCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "LoRaWANNetworkServerCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayFirmwareInformationRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1495,50 +1220,28 @@
 GetWirelessGatewayStatisticsRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
     {
         "WirelessGatewayId": str,
     },
 )
 
-GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
-    "GetWirelessGatewayStatisticsResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "LastUplinkReceivedAt": str,
-        "ConnectionStatus": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
 GetWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "WirelessGatewayTaskDefinitionId": str,
-        "LastUplinkReceivedAt": str,
-        "TaskCreatedAt": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GlobalIdentityTypeDef = TypedDict(
     "GlobalIdentityTypeDef",
     {
         "Lac": int,
         "GeranCid": int,
     },
 )
@@ -1558,38 +1261,22 @@
         "OnboardingStatus": OnboardStatusType,
         "OnboardingStatusReason": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-LoRaWANJoinEventNotificationConfigurationsOutputTypeDef = TypedDict(
-    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
-    {
-        "DevEuiEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANJoinEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
     {
         "DevEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANJoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -1802,22 +1489,14 @@
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
-)
-
 ListWirelessDeviceImportTasksRequestRequestTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1863,34 +1542,14 @@
         "GatewayEui": str,
         "Snr": float,
         "Rssi": float,
     },
     total=False,
 )
 
-OtaaV10XOutputTypeDef = TypedDict(
-    "OtaaV10XOutputTypeDef",
-    {
-        "AppKey": str,
-        "AppEui": str,
-        "GenAppKey": str,
-    },
-    total=False,
-)
-
-OtaaV11OutputTypeDef = TypedDict(
-    "OtaaV11OutputTypeDef",
-    {
-        "AppKey": str,
-        "NwkKey": str,
-        "JoinEui": str,
-    },
-    total=False,
-)
-
 OtaaV10XTypeDef = TypedDict(
     "OtaaV10XTypeDef",
     {
         "AppKey": str,
         "AppEui": str,
         "GenAppKey": str,
     },
@@ -1903,24 +1562,14 @@
         "AppKey": str,
         "NwkKey": str,
         "JoinEui": str,
     },
     total=False,
 )
 
-LoRaWANGatewayVersionOutputTypeDef = TypedDict(
-    "LoRaWANGatewayVersionOutputTypeDef",
-    {
-        "PackageVersion": str,
-        "Model": str,
-        "Station": str,
-    },
-    total=False,
-)
-
 LoRaWANGatewayVersionTypeDef = TypedDict(
     "LoRaWANGatewayVersionTypeDef",
     {
         "PackageVersion": str,
         "Model": str,
         "Station": str,
     },
@@ -2041,41 +1690,14 @@
     "ResetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
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
-SendDataToMulticastGroupResponseTypeDef = TypedDict(
-    "SendDataToMulticastGroupResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendDataToWirelessDeviceResponseTypeDef = TypedDict(
-    "SendDataToWirelessDeviceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkSendDataToDeviceTypeDef = TypedDict(
     "SidewalkSendDataToDeviceTypeDef",
     {
         "Seq": int,
         "MessageType": MessageTypeType,
         "AckModeRetryDurationSecs": int,
     },
@@ -2111,32 +1733,14 @@
     "SidewalkUpdateImportInfoTypeDef",
     {
         "DeviceCreationFile": str,
     },
     total=False,
 )
 
-StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TdscdmaLocalIdTypeDef = TypedDict(
     "TdscdmaLocalIdTypeDef",
     {
         "Uarfcn": int,
         "CellParams": int,
     },
 )
@@ -2166,22 +1770,14 @@
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-TestWirelessDeviceResponseTypeDef = TypedDict(
-    "TestWirelessDeviceResponseTypeDef",
-    {
-        "Result": str,
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
@@ -2294,99 +1890,50 @@
 )
 
 
 class WcdmaNmrObjTypeDef(_RequiredWcdmaNmrObjTypeDef, _OptionalWcdmaNmrObjTypeDef):
     pass
 
 
-WirelessDeviceEventLogOptionOutputTypeDef = TypedDict(
-    "WirelessDeviceEventLogOptionOutputTypeDef",
-    {
-        "Event": WirelessDeviceEventType,
-        "LogLevel": LogLevelType,
-    },
-)
-
 WirelessDeviceEventLogOptionTypeDef = TypedDict(
     "WirelessDeviceEventLogOptionTypeDef",
     {
         "Event": WirelessDeviceEventType,
         "LogLevel": LogLevelType,
     },
 )
 
-WirelessGatewayEventLogOptionOutputTypeDef = TypedDict(
-    "WirelessGatewayEventLogOptionOutputTypeDef",
-    {
-        "Event": WirelessGatewayEventType,
-        "LogLevel": LogLevelType,
-    },
-)
-
 WirelessGatewayEventLogOptionTypeDef = TypedDict(
     "WirelessGatewayEventLogOptionTypeDef",
     {
         "Event": WirelessGatewayEventType,
         "LogLevel": LogLevelType,
     },
 )
 
-AbpV10XOutputTypeDef = TypedDict(
-    "AbpV10XOutputTypeDef",
-    {
-        "DevAddr": str,
-        "SessionKeys": SessionKeysAbpV10XOutputTypeDef,
-        "FCntStart": int,
-    },
-    total=False,
-)
-
 AbpV10XTypeDef = TypedDict(
     "AbpV10XTypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV10XTypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
-AbpV11OutputTypeDef = TypedDict(
-    "AbpV11OutputTypeDef",
-    {
-        "DevAddr": str,
-        "SessionKeys": SessionKeysAbpV11OutputTypeDef,
-        "FCntStart": int,
-    },
-    total=False,
-)
-
 AbpV11TypeDef = TypedDict(
     "AbpV11TypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV11TypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
-GetPositionResponseTypeDef = TypedDict(
-    "GetPositionResponseTypeDef",
-    {
-        "Position": List[float],
-        "Accuracy": AccuracyTypeDef,
-        "SolverType": Literal["GNSS"],
-        "SolverProvider": Literal["Semtech"],
-        "SolverVersion": str,
-        "Timestamp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoTypeDef,
     },
 )
 _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
@@ -2485,17 +2032,256 @@
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
     "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
     {
-        "Sidewalk": SidewalkAccountInfoOutputTypeDef,
+        "Sidewalk": SidewalkAccountInfoTypeDef,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceProfileResponseTypeDef = TypedDict(
+    "CreateDeviceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFuotaTaskResponseTypeDef = TypedDict(
+    "CreateFuotaTaskResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMulticastGroupResponseTypeDef = TypedDict(
+    "CreateMulticastGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateServiceProfileResponseTypeDef = TypedDict(
+    "CreateServiceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessDeviceResponseTypeDef = TypedDict(
+    "CreateWirelessDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayTaskDefinitionId": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Expression": str,
+        "ExpressionType": ExpressionTypeType,
+        "Description": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionEstimateResponseTypeDef = TypedDict(
+    "GetPositionEstimateResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionResponseTypeDef = TypedDict(
+    "GetPositionResponseTypeDef",
+    {
+        "Position": List[float],
+        "Accuracy": AccuracyTypeDef,
+        "SolverType": Literal["GNSS"],
+        "SolverProvider": Literal["Semtech"],
+        "SolverVersion": str,
+        "Timestamp": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourceLogLevelResponseTypeDef = TypedDict(
+    "GetResourceLogLevelResponseTypeDef",
+    {
+        "LogLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePositionResponseTypeDef = TypedDict(
+    "GetResourcePositionResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceEndpointResponseTypeDef = TypedDict(
+    "GetServiceEndpointResponseTypeDef",
+    {
+        "ServiceType": WirelessGatewayServiceTypeType,
+        "ServiceEndpoint": str,
+        "ServerTrust": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "LoRaWANNetworkServerCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "LastUplinkReceivedAt": str,
+        "ConnectionStatus": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "WirelessGatewayTaskDefinitionId": str,
+        "LastUplinkReceivedAt": str,
+        "TaskCreatedAt": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToMulticastGroupResponseTypeDef = TypedDict(
+    "SendDataToMulticastGroupResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToWirelessDeviceResponseTypeDef = TypedDict(
+    "SendDataToWirelessDeviceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestWirelessDeviceResponseTypeDef = TypedDict(
+    "TestWirelessDeviceResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoRaWANGatewayOutputTypeDef = TypedDict(
     "LoRaWANGatewayOutputTypeDef",
     {
         "GatewayEui": str,
@@ -2573,40 +2359,23 @@
         "DeviceCertificates": List[CertificateListTypeDef],
         "DeviceProfileId": str,
         "Status": WirelessDeviceSidewalkStatusType,
     },
     total=False,
 )
 
-ConnectionStatusEventConfigurationOutputTypeDef = TypedDict(
-    "ConnectionStatusEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
-        "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 ConnectionStatusEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
         "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-ConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2753,14 +2522,28 @@
 class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
+    {
+        "TraceContent": TraceContentTypeDef,
+        "WirelessDevices": List[str],
+        "WirelessGateways": List[str],
+        "Description": str,
+        "Arn": str,
+        "Name": str,
+        "MulticastGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2808,54 +2591,27 @@
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "NextToken": str,
         "DestinationList": List[DestinationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceProfilesResponseTypeDef = TypedDict(
     "ListDeviceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "DeviceProfileList": List[DeviceProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeviceRegistrationStateEventConfigurationOutputTypeDef = TypedDict(
-    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
-MessageDeliveryStatusEventConfigurationOutputTypeDef = TypedDict(
-    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
-ProximityEventConfigurationOutputTypeDef = TypedDict(
-    "ProximityEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 DeviceRegistrationStateEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
@@ -2875,38 +2631,14 @@
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ProximityResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "ProximityResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2929,16 +2661,16 @@
 
 FPortsOutputTypeDef = TypedDict(
     "FPortsOutputTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
-        "Positioning": PositioningOutputTypeDef,
-        "Applications": List[ApplicationConfigOutputTypeDef],
+        "Positioning": PositioningTypeDef,
+        "Applications": List[ApplicationConfigTypeDef],
     },
     total=False,
 )
 
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
@@ -2961,23 +2693,23 @@
 )
 
 ListFuotaTasksResponseTypeDef = TypedDict(
     "ListFuotaTasksResponseTypeDef",
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParticipatingGatewaysOutputTypeDef = TypedDict(
     "ParticipatingGatewaysOutputTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemOutputTypeDef],
+        "GatewayList": List[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
@@ -2998,80 +2730,66 @@
         "LoRaWAN": LoRaWANFuotaTaskGetInfoTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
         "CreatedAt": datetime,
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupResponseTypeDef = TypedDict(
     "GetMulticastGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": str,
         "LoRaWAN": LoRaWANMulticastGetTypeDef,
         "CreatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "TraceContent": TraceContentOutputTypeDef,
-        "WirelessDevices": List[str],
-        "WirelessGateways": List[str],
-        "Description": str,
-        "Arn": str,
-        "Name": str,
-        "MulticastGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
         "AccountLinked": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartnerAccountsResponseTypeDef = TypedDict(
     "ListPartnerAccountsResponseTypeDef",
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceProfileResponseTypeDef = TypedDict(
     "GetServiceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANGetServiceProfileInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "GetWirelessDeviceImportTaskResponseTypeDef",
     {
         "Id": str,
@@ -3081,15 +2799,15 @@
         "CreationTime": datetime,
         "Status": ImportTaskStatusType,
         "StatusReason": str,
         "InitializedImportedDeviceCount": int,
         "PendingImportedDeviceCount": int,
         "OnboardedImportedDeviceCount": int,
         "FailedImportedDeviceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessDeviceImportTaskTypeDef = TypedDict(
     "WirelessDeviceImportTaskTypeDef",
     {
         "Id": str,
@@ -3132,89 +2850,64 @@
     "ImportedWirelessDeviceTypeDef",
     {
         "Sidewalk": ImportedSidewalkDeviceTypeDef,
     },
     total=False,
 )
 
-JoinEventConfigurationOutputTypeDef = TypedDict(
-    "JoinEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 JoinEventConfigurationTypeDef = TypedDict(
     "JoinEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-JoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "JoinResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 JoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "JoinResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
 ListMulticastGroupsByFuotaTaskResponseTypeDef = TypedDict(
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupByFuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMulticastGroupsResponseTypeDef = TypedDict(
     "ListMulticastGroupsResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkAnalyzerConfigurationsResponseTypeDef = TypedDict(
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "NetworkAnalyzerConfigurationList": List[NetworkAnalyzerConfigurationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceProfilesResponseTypeDef = TypedDict(
     "ListServiceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceProfileList": List[ServiceProfileTypeDef],
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
 
 LoRaWANDeviceMetadataTypeDef = TypedDict(
     "LoRaWANDeviceMetadataTypeDef",
     {
         "DevEui": str,
@@ -3226,44 +2919,33 @@
     },
     total=False,
 )
 
 LoRaWANGatewayCurrentVersionTypeDef = TypedDict(
     "LoRaWANGatewayCurrentVersionTypeDef",
     {
-        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
-LoRaWANUpdateGatewayTaskCreateOutputTypeDef = TypedDict(
-    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
+LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
+    "LoRaWANUpdateGatewayTaskCreateTypeDef",
     {
         "UpdateSignature": str,
         "SigKeyCrc": int,
-        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
-        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
+        "UpdateVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
 LoRaWANUpdateGatewayTaskEntryTypeDef = TypedDict(
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     {
-        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
-        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
-    },
-    total=False,
-)
-
-LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
-    "LoRaWANUpdateGatewayTaskCreateTypeDef",
-    {
-        "UpdateSignature": str,
-        "SigKeyCrc": int,
         "CurrentVersion": LoRaWANGatewayVersionTypeDef,
         "UpdateVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
 MulticastWirelessMetadataTypeDef = TypedDict(
@@ -3469,15 +3151,15 @@
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionOutputTypeDef",
     {
-        "Events": List[WirelessDeviceEventLogOptionOutputTypeDef],
+        "Events": List[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
 
 class WirelessDeviceLogOptionOutputTypeDef(
     _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
@@ -3513,15 +3195,15 @@
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
     "_OptionalWirelessGatewayLogOptionOutputTypeDef",
     {
-        "Events": List[WirelessGatewayEventLogOptionOutputTypeDef],
+        "Events": List[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
 
 class WirelessGatewayLogOptionOutputTypeDef(
     _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
@@ -3557,15 +3239,15 @@
         "Name": str,
         "Id": str,
         "Description": str,
         "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
@@ -3625,28 +3307,28 @@
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoRaWANDeviceOutputTypeDef = TypedDict(
     "LoRaWANDeviceOutputTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
-        "OtaaV1_1": OtaaV11OutputTypeDef,
-        "OtaaV1_0_x": OtaaV10XOutputTypeDef,
-        "AbpV1_1": AbpV11OutputTypeDef,
-        "AbpV1_0_x": AbpV10XOutputTypeDef,
+        "OtaaV1_1": OtaaV11TypeDef,
+        "OtaaV1_0_x": OtaaV10XTypeDef,
+        "AbpV1_1": AbpV11TypeDef,
+        "AbpV1_0_x": AbpV10XTypeDef,
         "FPorts": FPortsOutputTypeDef,
     },
     total=False,
 )
 
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
@@ -3694,15 +3376,15 @@
 )
 
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGsmObjTypeDef = TypedDict(
     "_RequiredGsmObjTypeDef",
     {
         "Mcc": int,
@@ -3729,39 +3411,39 @@
 
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventNotificationItemConfigurationsTypeDef = TypedDict(
     "EventNotificationItemConfigurationsTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
-        "Proximity": ProximityEventConfigurationOutputTypeDef,
-        "Join": JoinEventConfigurationOutputTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
+        "Proximity": ProximityEventConfigurationTypeDef,
+        "Join": JoinEventConfigurationTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
     },
     total=False,
 )
 
 GetResourceEventConfigurationResponseTypeDef = TypedDict(
     "GetResourceEventConfigurationResponseTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
-        "Proximity": ProximityEventConfigurationOutputTypeDef,
-        "Join": JoinEventConfigurationOutputTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
+        "Proximity": ProximityEventConfigurationTypeDef,
+        "Join": JoinEventConfigurationTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceEventConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -3788,22 +3470,20 @@
 ):
     pass
 
 
 GetEventConfigurationByResourceTypesResponseTypeDef = TypedDict(
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
-        "DeviceRegistrationState": (
-            DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef
-        ),
-        "Proximity": ProximityResourceTypeEventConfigurationOutputTypeDef,
-        "Join": JoinResourceTypeEventConfigurationOutputTypeDef,
-        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
+        "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
+        "Join": JoinResourceTypeEventConfigurationTypeDef,
+        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
@@ -3818,56 +3498,46 @@
 GetWirelessDeviceStatisticsResponseTypeDef = TypedDict(
     "GetWirelessDeviceStatisticsResponseTypeDef",
     {
         "WirelessDeviceId": str,
         "LastUplinkReceivedAt": str,
         "LoRaWAN": LoRaWANDeviceMetadataTypeDef,
         "Sidewalk": SidewalkDeviceMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessGatewayFirmwareInformationResponseTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     {
         "LoRaWAN": LoRaWANGatewayCurrentVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWirelessGatewayTaskCreateOutputTypeDef = TypedDict(
-    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
+UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
+    "UpdateWirelessGatewayTaskCreateTypeDef",
     {
         "UpdateDataSource": str,
         "UpdateDataRole": str,
-        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
+        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
     },
     total=False,
 )
 
 UpdateWirelessGatewayTaskEntryTypeDef = TypedDict(
     "UpdateWirelessGatewayTaskEntryTypeDef",
     {
         "Id": str,
         "LoRaWAN": LoRaWANUpdateGatewayTaskEntryTypeDef,
         "Arn": str,
     },
     total=False,
 )
 
-UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
-    "UpdateWirelessGatewayTaskCreateTypeDef",
-    {
-        "UpdateDataSource": str,
-        "UpdateDataRole": str,
-        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
-    },
-    total=False,
-)
-
 SendDataToMulticastGroupRequestRequestTypeDef = TypedDict(
     "SendDataToMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
         "PayloadData": str,
         "WirelessMetadata": MulticastWirelessMetadataTypeDef,
     },
@@ -3898,15 +3568,15 @@
 
 
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PositionConfigurationItemTypeDef = TypedDict(
     "PositionConfigurationItemTypeDef",
     {
         "ResourceIdentifier": str,
@@ -3919,15 +3589,15 @@
 
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
         "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
         "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
@@ -3938,24 +3608,24 @@
 )
 
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWirelessDevicesResponseTypeDef = TypedDict(
     "ListWirelessDevicesResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessDeviceResponseTypeDef = TypedDict(
     "GetWirelessDeviceResponseTypeDef",
     {
         "Type": WirelessDeviceTypeType,
@@ -3965,15 +3635,15 @@
         "Id": str,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
         "LoRaWAN": LoRaWANDeviceOutputTypeDef,
         "Sidewalk": SidewalkDeviceTypeDef,
         "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
@@ -4067,34 +3737,14 @@
         "IdentifierType": IdentifierTypeType,
         "PartnerType": Literal["Sidewalk"],
         "Events": EventNotificationItemConfigurationsTypeDef,
     },
     total=False,
 )
 
-GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "AutoCreateTasks": bool,
-        "Name": str,
-        "Update": UpdateWirelessGatewayTaskCreateOutputTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "AutoCreateTasks": bool,
     },
 )
 _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
@@ -4112,29 +3762,49 @@
 class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
+GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "AutoCreateTasks": bool,
+        "Name": str,
+        "Update": UpdateWirelessGatewayTaskCreateTypeDef,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPositionConfigurationsResponseTypeDef = TypedDict(
     "ListPositionConfigurationsResponseTypeDef",
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendDataToWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
@@ -4171,10 +3841,10 @@
 )
 
 ListEventConfigurationsResponseTypeDef = TypedDict(
     "ListEventConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "EventConfigurationsList": List[EventConfigurationItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.pyi` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotwireless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XOutputTypeDef
+    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
 
-    data: SessionKeysAbpV10XOutputTypeDef = {...}
+    data: SessionKeysAbpV10XTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -59,58 +59,42 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "SessionKeysAbpV10XOutputTypeDef",
     "SessionKeysAbpV10XTypeDef",
-    "SessionKeysAbpV11OutputTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
-    "ApplicationConfigOutputTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
-    "SidewalkAccountInfoOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
-    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
-    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
-    "CreateDestinationResponseTypeDef",
     "LoRaWANDeviceProfileTypeDef",
-    "CreateDeviceProfileResponseTypeDef",
     "LoRaWANFuotaTaskTypeDef",
-    "CreateFuotaTaskResponseTypeDef",
     "LoRaWANMulticastTypeDef",
-    "CreateMulticastGroupResponseTypeDef",
     "TraceContentTypeDef",
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
     "LoRaWANServiceProfileTypeDef",
-    "CreateServiceProfileResponseTypeDef",
     "SidewalkCreateWirelessDeviceTypeDef",
-    "CreateWirelessDeviceResponseTypeDef",
-    "CreateWirelessGatewayResponseTypeDef",
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
-    "CreateWirelessGatewayTaskResponseTypeDef",
     "DakCertificateMetadataTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteDeviceProfileRequestRequestTypeDef",
     "DeleteFuotaTaskRequestRequestTypeDef",
     "DeleteMulticastGroupRequestRequestTypeDef",
     "DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "DeleteQueuedMessagesRequestRequestTypeDef",
@@ -119,79 +103,64 @@
     "DeleteWirelessDeviceRequestRequestTypeDef",
     "DeleteWirelessGatewayRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskRequestRequestTypeDef",
     "DeregisterWirelessDeviceRequestRequestTypeDef",
     "DestinationsTypeDef",
     "DeviceProfileTypeDef",
-    "SidewalkEventNotificationConfigurationsOutputTypeDef",
     "SidewalkEventNotificationConfigurationsTypeDef",
-    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
     "SidewalkResourceTypeEventConfigurationTypeDef",
     "DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef",
     "DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromThingRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
-    "PositioningOutputTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
-    "GatewayListItemOutputTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
     "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
     "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
-    "TraceContentOutputTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
     "WiFiAccessPointTypeDef",
-    "GetPositionEstimateResponseTypeDef",
     "GetPositionRequestRequestTypeDef",
     "GetResourceEventConfigurationRequestRequestTypeDef",
     "GetResourceLogLevelRequestRequestTypeDef",
-    "GetResourceLogLevelResponseTypeDef",
     "GetResourcePositionRequestRequestTypeDef",
-    "GetResourcePositionResponseTypeDef",
     "GetServiceEndpointRequestRequestTypeDef",
-    "GetServiceEndpointResponseTypeDef",
     "GetServiceProfileRequestRequestTypeDef",
     "LoRaWANGetServiceProfileInfoTypeDef",
     "GetWirelessDeviceImportTaskRequestRequestTypeDef",
     "SidewalkGetStartImportInfoTypeDef",
     "GetWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsRequestRequestTypeDef",
     "SidewalkDeviceMetadataTypeDef",
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
-    "GetWirelessGatewayCertificateResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     "GetWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
-    "GetWirelessGatewayStatisticsResponseTypeDef",
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskRequestRequestTypeDef",
-    "GetWirelessGatewayTaskResponseTypeDef",
     "GlobalIdentityTypeDef",
     "GsmLocalIdTypeDef",
     "ImportedSidewalkDeviceTypeDef",
-    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
-    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListDeviceProfilesRequestRequestTypeDef",
     "ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef",
     "ListEventConfigurationsRequestRequestTypeDef",
     "ListFuotaTasksRequestRequestTypeDef",
     "ListMulticastGroupsByFuotaTaskRequestRequestTypeDef",
@@ -202,137 +171,136 @@
     "NetworkAnalyzerConfigurationsTypeDef",
     "ListPartnerAccountsRequestRequestTypeDef",
     "ListPositionConfigurationsRequestRequestTypeDef",
     "ListQueuedMessagesRequestRequestTypeDef",
     "ListServiceProfilesRequestRequestTypeDef",
     "ServiceProfileTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     "ListWirelessDevicesRequestRequestTypeDef",
     "ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef",
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
-    "OtaaV10XOutputTypeDef",
-    "OtaaV11OutputTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
-    "LoRaWANGatewayVersionOutputTypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
     "LoRaWANMulticastSessionTypeDef",
     "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
     "PutResourceLogLevelRequestRequestTypeDef",
     "ResetResourceLogLevelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendDataToMulticastGroupResponseTypeDef",
-    "SendDataToWirelessDeviceResponseTypeDef",
     "SidewalkSendDataToDeviceTypeDef",
     "SidewalkSingleStartImportInfoTypeDef",
     "SidewalkStartImportInfoTypeDef",
     "SidewalkUpdateAccountTypeDef",
     "SidewalkUpdateImportInfoTypeDef",
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    "StartWirelessDeviceImportTaskResponseTypeDef",
     "TdscdmaLocalIdTypeDef",
     "TdscdmaNmrObjTypeDef",
     "TestWirelessDeviceRequestRequestTypeDef",
-    "TestWirelessDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
     "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
-    "WirelessDeviceEventLogOptionOutputTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
-    "WirelessGatewayEventLogOptionOutputTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
-    "AbpV10XOutputTypeDef",
     "AbpV10XTypeDef",
-    "AbpV11OutputTypeDef",
     "AbpV11TypeDef",
-    "GetPositionResponseTypeDef",
     "AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     "CreateDestinationRequestRequestTypeDef",
     "StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateDeviceProfileResponseTypeDef",
+    "CreateFuotaTaskResponseTypeDef",
+    "CreateMulticastGroupResponseTypeDef",
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    "CreateServiceProfileResponseTypeDef",
+    "CreateWirelessDeviceResponseTypeDef",
+    "CreateWirelessGatewayResponseTypeDef",
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetPositionEstimateResponseTypeDef",
+    "GetPositionResponseTypeDef",
+    "GetResourceLogLevelResponseTypeDef",
+    "GetResourcePositionResponseTypeDef",
+    "GetServiceEndpointResponseTypeDef",
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    "GetWirelessGatewayTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SendDataToMulticastGroupResponseTypeDef",
+    "SendDataToWirelessDeviceResponseTypeDef",
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    "TestWirelessDeviceResponseTypeDef",
     "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
-    "ConnectionStatusEventConfigurationOutputTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
-    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
     "UpdateFuotaTaskRequestRequestTypeDef",
     "CreateMulticastGroupRequestRequestTypeDef",
     "UpdateMulticastGroupRequestRequestTypeDef",
     "CreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "CreateServiceProfileRequestRequestTypeDef",
     "SidewalkGetDeviceProfileTypeDef",
     "ListDestinationsResponseTypeDef",
     "ListDeviceProfilesResponseTypeDef",
-    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
-    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
-    "ProximityEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
-    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
-    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
-    "ProximityResourceTypeEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
     "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
     "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
-    "JoinEventConfigurationOutputTypeDef",
     "JoinEventConfigurationTypeDef",
-    "JoinResourceTypeEventConfigurationOutputTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     "ListMulticastGroupsResponseTypeDef",
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
-    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
-    "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "LoRaWANUpdateGatewayTaskCreateTypeDef",
+    "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "MulticastWirelessMetadataTypeDef",
     "StartMulticastGroupSessionRequestRequestTypeDef",
     "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
@@ -361,17 +329,16 @@
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
-    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
-    "UpdateWirelessGatewayTaskEntryTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
+    "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
@@ -379,53 +346,33 @@
     "GetWirelessDeviceResponseTypeDef",
     "CreateWirelessDeviceRequestRequestTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
+    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
-    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
-SessionKeysAbpV10XOutputTypeDef = TypedDict(
-    "SessionKeysAbpV10XOutputTypeDef",
-    {
-        "NwkSKey": str,
-        "AppSKey": str,
-    },
-    total=False,
-)
-
 SessionKeysAbpV10XTypeDef = TypedDict(
     "SessionKeysAbpV10XTypeDef",
     {
         "NwkSKey": str,
         "AppSKey": str,
     },
     total=False,
 )
 
-SessionKeysAbpV11OutputTypeDef = TypedDict(
-    "SessionKeysAbpV11OutputTypeDef",
-    {
-        "FNwkSIntKey": str,
-        "SNwkSIntKey": str,
-        "NwkSEncKey": str,
-        "AppSKey": str,
-    },
-    total=False,
-)
-
 SessionKeysAbpV11TypeDef = TypedDict(
     "SessionKeysAbpV11TypeDef",
     {
         "FNwkSIntKey": str,
         "SNwkSIntKey": str,
         "NwkSEncKey": str,
         "AppSKey": str,
@@ -438,24 +385,14 @@
     {
         "HorizontalAccuracy": float,
         "VerticalAccuracy": float,
     },
     total=False,
 )
 
-ApplicationConfigOutputTypeDef = TypedDict(
-    "ApplicationConfigOutputTypeDef",
-    {
-        "FPort": int,
-        "Type": Literal["SemtechGeolocation"],
-        "DestinationName": str,
-    },
-    total=False,
-)
-
 ApplicationConfigTypeDef = TypedDict(
     "ApplicationConfigTypeDef",
     {
         "FPort": int,
         "Type": Literal["SemtechGeolocation"],
         "DestinationName": str,
     },
@@ -475,21 +412,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-SidewalkAccountInfoOutputTypeDef = TypedDict(
-    "SidewalkAccountInfoOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AmazonId": str,
-        "AppServerPrivateKey": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = TypedDict(
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
         "MulticastGroupId": str,
@@ -524,22 +463,14 @@
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     {
         "Id": str,
         "IotCertificateId": str,
     },
 )
 
-AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateWirelessGatewayWithThingRequestRequestTypeDef = TypedDict(
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
@@ -600,55 +531,30 @@
     "CertificateListTypeDef",
     {
         "SigningAlg": SigningAlgType,
         "Value": str,
     },
 )
 
-LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef = TypedDict(
-    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
-    {
-        "GatewayEuiEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     {
         "GatewayEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANDeviceProfileTypeDef = TypedDict(
     "LoRaWANDeviceProfileTypeDef",
     {
         "SupportsClassB": bool,
         "ClassBTimeout": int,
         "PingSlotPeriod": int,
         "PingSlotDr": int,
@@ -667,150 +573,69 @@
         "RfRegion": str,
         "SupportsJoin": bool,
         "Supports32BitFCnt": bool,
     },
     total=False,
 )
 
-CreateDeviceProfileResponseTypeDef = TypedDict(
-    "CreateDeviceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANFuotaTaskTypeDef = TypedDict(
     "LoRaWANFuotaTaskTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
     },
     total=False,
 )
 
-CreateFuotaTaskResponseTypeDef = TypedDict(
-    "CreateFuotaTaskResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANMulticastTypeDef = TypedDict(
     "LoRaWANMulticastTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
         "DlClass": DlClassType,
     },
     total=False,
 )
 
-CreateMulticastGroupResponseTypeDef = TypedDict(
-    "CreateMulticastGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TraceContentTypeDef = TypedDict(
     "TraceContentTypeDef",
     {
         "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
         "LogLevel": LogLevelType,
         "MulticastFrameInfo": MulticastFrameInfoType,
     },
     total=False,
 )
 
-CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANServiceProfileTypeDef = TypedDict(
     "LoRaWANServiceProfileTypeDef",
     {
         "AddGwMetadata": bool,
         "DrMin": int,
         "DrMax": int,
         "PrAllowed": bool,
         "RaAllowed": bool,
     },
     total=False,
 )
 
-CreateServiceProfileResponseTypeDef = TypedDict(
-    "CreateServiceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkCreateWirelessDeviceTypeDef = TypedDict(
     "SidewalkCreateWirelessDeviceTypeDef",
     {
         "DeviceProfileId": str,
     },
     total=False,
 )
 
-CreateWirelessDeviceResponseTypeDef = TypedDict(
-    "CreateWirelessDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
         "WirelessGatewayTaskDefinitionId": str,
     },
 )
 
-CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayTaskDefinitionId": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDakCertificateMetadataTypeDef = TypedDict(
     "_RequiredDakCertificateMetadataTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalDakCertificateMetadataTypeDef = TypedDict(
@@ -966,38 +791,22 @@
         "Arn": str,
         "Name": str,
         "Id": str,
     },
     total=False,
 )
 
-SidewalkEventNotificationConfigurationsOutputTypeDef = TypedDict(
-    "SidewalkEventNotificationConfigurationsOutputTypeDef",
-    {
-        "AmazonIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 SidewalkEventNotificationConfigurationsTypeDef = TypedDict(
     "SidewalkEventNotificationConfigurationsTypeDef",
     {
         "AmazonIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-SidewalkResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 SidewalkResourceTypeEventConfigurationTypeDef = TypedDict(
     "SidewalkResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -1051,24 +860,14 @@
 DisassociateWirelessGatewayFromThingRequestRequestTypeDef = TypedDict(
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-PositioningOutputTypeDef = TypedDict(
-    "PositioningOutputTypeDef",
-    {
-        "ClockSync": int,
-        "Stream": int,
-        "Gnss": int,
-    },
-    total=False,
-)
-
 PositioningTypeDef = TypedDict(
     "PositioningTypeDef",
     {
         "ClockSync": int,
         "Stream": int,
         "Gnss": int,
     },
@@ -1081,22 +880,14 @@
         "Id": str,
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
-GatewayListItemOutputTypeDef = TypedDict(
-    "GatewayListItemOutputTypeDef",
-    {
-        "GatewayId": str,
-        "DownlinkFrequency": int,
-    },
-)
-
 GatewayListItemTypeDef = TypedDict(
     "GatewayListItemTypeDef",
     {
         "GatewayId": str,
         "DownlinkFrequency": int,
     },
 )
@@ -1104,27 +895,14 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Expression": str,
-        "ExpressionType": ExpressionTypeType,
-        "Description": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeviceProfileRequestRequestTypeDef = TypedDict(
     "GetDeviceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1210,24 +988,14 @@
 GetNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 
-TraceContentOutputTypeDef = TypedDict(
-    "TraceContentOutputTypeDef",
-    {
-        "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
-        "LogLevel": LogLevelType,
-        "MulticastFrameInfo": MulticastFrameInfoType,
-    },
-    total=False,
-)
-
 GetPartnerAccountRequestRequestTypeDef = TypedDict(
     "GetPartnerAccountRequestRequestTypeDef",
     {
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
 )
@@ -1282,22 +1050,14 @@
     "WiFiAccessPointTypeDef",
     {
         "MacAddress": str,
         "Rss": int,
     },
 )
 
-GetPositionEstimateResponseTypeDef = TypedDict(
-    "GetPositionEstimateResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPositionRequestRequestTypeDef = TypedDict(
     "GetPositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
@@ -1327,56 +1087,30 @@
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
 
-GetResourceLogLevelResponseTypeDef = TypedDict(
-    "GetResourceLogLevelResponseTypeDef",
-    {
-        "LogLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePositionRequestRequestTypeDef = TypedDict(
     "GetResourcePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
 
-GetResourcePositionResponseTypeDef = TypedDict(
-    "GetResourcePositionResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceEndpointRequestRequestTypeDef = TypedDict(
     "GetServiceEndpointRequestRequestTypeDef",
     {
         "ServiceType": WirelessGatewayServiceTypeType,
     },
     total=False,
 )
 
-GetServiceEndpointResponseTypeDef = TypedDict(
-    "GetServiceEndpointResponseTypeDef",
-    {
-        "ServiceType": WirelessGatewayServiceTypeType,
-        "ServiceEndpoint": str,
-        "ServerTrust": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceProfileRequestRequestTypeDef = TypedDict(
     "GetServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1451,23 +1185,14 @@
 GetWirelessGatewayCertificateRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
-    "GetWirelessGatewayCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "LoRaWANNetworkServerCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayFirmwareInformationRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1482,50 +1207,28 @@
 GetWirelessGatewayStatisticsRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
     {
         "WirelessGatewayId": str,
     },
 )
 
-GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
-    "GetWirelessGatewayStatisticsResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "LastUplinkReceivedAt": str,
-        "ConnectionStatus": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
 GetWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "WirelessGatewayTaskDefinitionId": str,
-        "LastUplinkReceivedAt": str,
-        "TaskCreatedAt": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GlobalIdentityTypeDef = TypedDict(
     "GlobalIdentityTypeDef",
     {
         "Lac": int,
         "GeranCid": int,
     },
 )
@@ -1545,38 +1248,22 @@
         "OnboardingStatus": OnboardStatusType,
         "OnboardingStatusReason": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-LoRaWANJoinEventNotificationConfigurationsOutputTypeDef = TypedDict(
-    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
-    {
-        "DevEuiEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANJoinEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
     {
         "DevEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 LoRaWANJoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -1781,22 +1468,14 @@
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
-)
-
 ListWirelessDeviceImportTasksRequestRequestTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1842,34 +1521,14 @@
         "GatewayEui": str,
         "Snr": float,
         "Rssi": float,
     },
     total=False,
 )
 
-OtaaV10XOutputTypeDef = TypedDict(
-    "OtaaV10XOutputTypeDef",
-    {
-        "AppKey": str,
-        "AppEui": str,
-        "GenAppKey": str,
-    },
-    total=False,
-)
-
-OtaaV11OutputTypeDef = TypedDict(
-    "OtaaV11OutputTypeDef",
-    {
-        "AppKey": str,
-        "NwkKey": str,
-        "JoinEui": str,
-    },
-    total=False,
-)
-
 OtaaV10XTypeDef = TypedDict(
     "OtaaV10XTypeDef",
     {
         "AppKey": str,
         "AppEui": str,
         "GenAppKey": str,
     },
@@ -1882,24 +1541,14 @@
         "AppKey": str,
         "NwkKey": str,
         "JoinEui": str,
     },
     total=False,
 )
 
-LoRaWANGatewayVersionOutputTypeDef = TypedDict(
-    "LoRaWANGatewayVersionOutputTypeDef",
-    {
-        "PackageVersion": str,
-        "Model": str,
-        "Station": str,
-    },
-    total=False,
-)
-
 LoRaWANGatewayVersionTypeDef = TypedDict(
     "LoRaWANGatewayVersionTypeDef",
     {
         "PackageVersion": str,
         "Model": str,
         "Station": str,
     },
@@ -2018,41 +1667,14 @@
     "ResetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
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
-SendDataToMulticastGroupResponseTypeDef = TypedDict(
-    "SendDataToMulticastGroupResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendDataToWirelessDeviceResponseTypeDef = TypedDict(
-    "SendDataToWirelessDeviceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkSendDataToDeviceTypeDef = TypedDict(
     "SidewalkSendDataToDeviceTypeDef",
     {
         "Seq": int,
         "MessageType": MessageTypeType,
         "AckModeRetryDurationSecs": int,
     },
@@ -2088,32 +1710,14 @@
     "SidewalkUpdateImportInfoTypeDef",
     {
         "DeviceCreationFile": str,
     },
     total=False,
 )
 
-StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TdscdmaLocalIdTypeDef = TypedDict(
     "TdscdmaLocalIdTypeDef",
     {
         "Uarfcn": int,
         "CellParams": int,
     },
 )
@@ -2141,22 +1745,14 @@
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-TestWirelessDeviceResponseTypeDef = TypedDict(
-    "TestWirelessDeviceResponseTypeDef",
-    {
-        "Result": str,
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
@@ -2261,99 +1857,50 @@
     },
     total=False,
 )
 
 class WcdmaNmrObjTypeDef(_RequiredWcdmaNmrObjTypeDef, _OptionalWcdmaNmrObjTypeDef):
     pass
 
-WirelessDeviceEventLogOptionOutputTypeDef = TypedDict(
-    "WirelessDeviceEventLogOptionOutputTypeDef",
-    {
-        "Event": WirelessDeviceEventType,
-        "LogLevel": LogLevelType,
-    },
-)
-
 WirelessDeviceEventLogOptionTypeDef = TypedDict(
     "WirelessDeviceEventLogOptionTypeDef",
     {
         "Event": WirelessDeviceEventType,
         "LogLevel": LogLevelType,
     },
 )
 
-WirelessGatewayEventLogOptionOutputTypeDef = TypedDict(
-    "WirelessGatewayEventLogOptionOutputTypeDef",
-    {
-        "Event": WirelessGatewayEventType,
-        "LogLevel": LogLevelType,
-    },
-)
-
 WirelessGatewayEventLogOptionTypeDef = TypedDict(
     "WirelessGatewayEventLogOptionTypeDef",
     {
         "Event": WirelessGatewayEventType,
         "LogLevel": LogLevelType,
     },
 )
 
-AbpV10XOutputTypeDef = TypedDict(
-    "AbpV10XOutputTypeDef",
-    {
-        "DevAddr": str,
-        "SessionKeys": SessionKeysAbpV10XOutputTypeDef,
-        "FCntStart": int,
-    },
-    total=False,
-)
-
 AbpV10XTypeDef = TypedDict(
     "AbpV10XTypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV10XTypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
-AbpV11OutputTypeDef = TypedDict(
-    "AbpV11OutputTypeDef",
-    {
-        "DevAddr": str,
-        "SessionKeys": SessionKeysAbpV11OutputTypeDef,
-        "FCntStart": int,
-    },
-    total=False,
-)
-
 AbpV11TypeDef = TypedDict(
     "AbpV11TypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV11TypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
-GetPositionResponseTypeDef = TypedDict(
-    "GetPositionResponseTypeDef",
-    {
-        "Position": List[float],
-        "Accuracy": AccuracyTypeDef,
-        "SolverType": Literal["GNSS"],
-        "SolverProvider": Literal["Semtech"],
-        "SolverVersion": str,
-        "Timestamp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoTypeDef,
     },
 )
 _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
@@ -2444,17 +1991,256 @@
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
     "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
     {
-        "Sidewalk": SidewalkAccountInfoOutputTypeDef,
+        "Sidewalk": SidewalkAccountInfoTypeDef,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceProfileResponseTypeDef = TypedDict(
+    "CreateDeviceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFuotaTaskResponseTypeDef = TypedDict(
+    "CreateFuotaTaskResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMulticastGroupResponseTypeDef = TypedDict(
+    "CreateMulticastGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateServiceProfileResponseTypeDef = TypedDict(
+    "CreateServiceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessDeviceResponseTypeDef = TypedDict(
+    "CreateWirelessDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayTaskDefinitionId": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Expression": str,
+        "ExpressionType": ExpressionTypeType,
+        "Description": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionEstimateResponseTypeDef = TypedDict(
+    "GetPositionEstimateResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionResponseTypeDef = TypedDict(
+    "GetPositionResponseTypeDef",
+    {
+        "Position": List[float],
+        "Accuracy": AccuracyTypeDef,
+        "SolverType": Literal["GNSS"],
+        "SolverProvider": Literal["Semtech"],
+        "SolverVersion": str,
+        "Timestamp": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourceLogLevelResponseTypeDef = TypedDict(
+    "GetResourceLogLevelResponseTypeDef",
+    {
+        "LogLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePositionResponseTypeDef = TypedDict(
+    "GetResourcePositionResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceEndpointResponseTypeDef = TypedDict(
+    "GetServiceEndpointResponseTypeDef",
+    {
+        "ServiceType": WirelessGatewayServiceTypeType,
+        "ServiceEndpoint": str,
+        "ServerTrust": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "LoRaWANNetworkServerCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "LastUplinkReceivedAt": str,
+        "ConnectionStatus": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "WirelessGatewayTaskDefinitionId": str,
+        "LastUplinkReceivedAt": str,
+        "TaskCreatedAt": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToMulticastGroupResponseTypeDef = TypedDict(
+    "SendDataToMulticastGroupResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToWirelessDeviceResponseTypeDef = TypedDict(
+    "SendDataToWirelessDeviceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestWirelessDeviceResponseTypeDef = TypedDict(
+    "TestWirelessDeviceResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoRaWANGatewayOutputTypeDef = TypedDict(
     "LoRaWANGatewayOutputTypeDef",
     {
         "GatewayEui": str,
@@ -2530,40 +2316,23 @@
         "DeviceCertificates": List[CertificateListTypeDef],
         "DeviceProfileId": str,
         "Status": WirelessDeviceSidewalkStatusType,
     },
     total=False,
 )
 
-ConnectionStatusEventConfigurationOutputTypeDef = TypedDict(
-    "ConnectionStatusEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
-        "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 ConnectionStatusEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
         "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-ConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2700,14 +2469,28 @@
 
 class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
+GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
+    {
+        "TraceContent": TraceContentTypeDef,
+        "WirelessDevices": List[str],
+        "WirelessGateways": List[str],
+        "Description": str,
+        "Arn": str,
+        "Name": str,
+        "MulticastGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2753,54 +2536,27 @@
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "NextToken": str,
         "DestinationList": List[DestinationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceProfilesResponseTypeDef = TypedDict(
     "ListDeviceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "DeviceProfileList": List[DeviceProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeviceRegistrationStateEventConfigurationOutputTypeDef = TypedDict(
-    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
-MessageDeliveryStatusEventConfigurationOutputTypeDef = TypedDict(
-    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
-ProximityEventConfigurationOutputTypeDef = TypedDict(
-    "ProximityEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 DeviceRegistrationStateEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
@@ -2820,38 +2576,14 @@
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ProximityResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "ProximityResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2874,16 +2606,16 @@
 
 FPortsOutputTypeDef = TypedDict(
     "FPortsOutputTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
-        "Positioning": PositioningOutputTypeDef,
-        "Applications": List[ApplicationConfigOutputTypeDef],
+        "Positioning": PositioningTypeDef,
+        "Applications": List[ApplicationConfigTypeDef],
     },
     total=False,
 )
 
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
@@ -2906,23 +2638,23 @@
 )
 
 ListFuotaTasksResponseTypeDef = TypedDict(
     "ListFuotaTasksResponseTypeDef",
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParticipatingGatewaysOutputTypeDef = TypedDict(
     "ParticipatingGatewaysOutputTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemOutputTypeDef],
+        "GatewayList": List[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
@@ -2943,80 +2675,66 @@
         "LoRaWAN": LoRaWANFuotaTaskGetInfoTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
         "CreatedAt": datetime,
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupResponseTypeDef = TypedDict(
     "GetMulticastGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": str,
         "LoRaWAN": LoRaWANMulticastGetTypeDef,
         "CreatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "TraceContent": TraceContentOutputTypeDef,
-        "WirelessDevices": List[str],
-        "WirelessGateways": List[str],
-        "Description": str,
-        "Arn": str,
-        "Name": str,
-        "MulticastGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
         "AccountLinked": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartnerAccountsResponseTypeDef = TypedDict(
     "ListPartnerAccountsResponseTypeDef",
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceProfileResponseTypeDef = TypedDict(
     "GetServiceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANGetServiceProfileInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "GetWirelessDeviceImportTaskResponseTypeDef",
     {
         "Id": str,
@@ -3026,15 +2744,15 @@
         "CreationTime": datetime,
         "Status": ImportTaskStatusType,
         "StatusReason": str,
         "InitializedImportedDeviceCount": int,
         "PendingImportedDeviceCount": int,
         "OnboardedImportedDeviceCount": int,
         "FailedImportedDeviceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessDeviceImportTaskTypeDef = TypedDict(
     "WirelessDeviceImportTaskTypeDef",
     {
         "Id": str,
@@ -3075,89 +2793,64 @@
     "ImportedWirelessDeviceTypeDef",
     {
         "Sidewalk": ImportedSidewalkDeviceTypeDef,
     },
     total=False,
 )
 
-JoinEventConfigurationOutputTypeDef = TypedDict(
-    "JoinEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
-        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
-    },
-    total=False,
-)
-
 JoinEventConfigurationTypeDef = TypedDict(
     "JoinEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-JoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
-    "JoinResourceTypeEventConfigurationOutputTypeDef",
-    {
-        "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 JoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "JoinResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
 ListMulticastGroupsByFuotaTaskResponseTypeDef = TypedDict(
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupByFuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMulticastGroupsResponseTypeDef = TypedDict(
     "ListMulticastGroupsResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkAnalyzerConfigurationsResponseTypeDef = TypedDict(
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "NetworkAnalyzerConfigurationList": List[NetworkAnalyzerConfigurationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceProfilesResponseTypeDef = TypedDict(
     "ListServiceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceProfileList": List[ServiceProfileTypeDef],
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
 
 LoRaWANDeviceMetadataTypeDef = TypedDict(
     "LoRaWANDeviceMetadataTypeDef",
     {
         "DevEui": str,
@@ -3169,44 +2862,33 @@
     },
     total=False,
 )
 
 LoRaWANGatewayCurrentVersionTypeDef = TypedDict(
     "LoRaWANGatewayCurrentVersionTypeDef",
     {
-        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
-LoRaWANUpdateGatewayTaskCreateOutputTypeDef = TypedDict(
-    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
+LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
+    "LoRaWANUpdateGatewayTaskCreateTypeDef",
     {
         "UpdateSignature": str,
         "SigKeyCrc": int,
-        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
-        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
+        "UpdateVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
 LoRaWANUpdateGatewayTaskEntryTypeDef = TypedDict(
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     {
-        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
-        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
-    },
-    total=False,
-)
-
-LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
-    "LoRaWANUpdateGatewayTaskCreateTypeDef",
-    {
-        "UpdateSignature": str,
-        "SigKeyCrc": int,
         "CurrentVersion": LoRaWANGatewayVersionTypeDef,
         "UpdateVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
 MulticastWirelessMetadataTypeDef = TypedDict(
@@ -3400,15 +3082,15 @@
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionOutputTypeDef",
     {
-        "Events": List[WirelessDeviceEventLogOptionOutputTypeDef],
+        "Events": List[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
 class WirelessDeviceLogOptionOutputTypeDef(
     _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
 ):
@@ -3440,15 +3122,15 @@
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
     "_OptionalWirelessGatewayLogOptionOutputTypeDef",
     {
-        "Events": List[WirelessGatewayEventLogOptionOutputTypeDef],
+        "Events": List[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
 class WirelessGatewayLogOptionOutputTypeDef(
     _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
 ):
@@ -3480,15 +3162,15 @@
         "Name": str,
         "Id": str,
         "Description": str,
         "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
@@ -3546,28 +3228,28 @@
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoRaWANDeviceOutputTypeDef = TypedDict(
     "LoRaWANDeviceOutputTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
-        "OtaaV1_1": OtaaV11OutputTypeDef,
-        "OtaaV1_0_x": OtaaV10XOutputTypeDef,
-        "AbpV1_1": AbpV11OutputTypeDef,
-        "AbpV1_0_x": AbpV10XOutputTypeDef,
+        "OtaaV1_1": OtaaV11TypeDef,
+        "OtaaV1_0_x": OtaaV10XTypeDef,
+        "AbpV1_1": AbpV11TypeDef,
+        "AbpV1_0_x": AbpV10XTypeDef,
         "FPorts": FPortsOutputTypeDef,
     },
     total=False,
 )
 
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
@@ -3615,15 +3297,15 @@
 )
 
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGsmObjTypeDef = TypedDict(
     "_RequiredGsmObjTypeDef",
     {
         "Mcc": int,
@@ -3648,39 +3330,39 @@
 
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventNotificationItemConfigurationsTypeDef = TypedDict(
     "EventNotificationItemConfigurationsTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
-        "Proximity": ProximityEventConfigurationOutputTypeDef,
-        "Join": JoinEventConfigurationOutputTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
+        "Proximity": ProximityEventConfigurationTypeDef,
+        "Join": JoinEventConfigurationTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
     },
     total=False,
 )
 
 GetResourceEventConfigurationResponseTypeDef = TypedDict(
     "GetResourceEventConfigurationResponseTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
-        "Proximity": ProximityEventConfigurationOutputTypeDef,
-        "Join": JoinEventConfigurationOutputTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
+        "Proximity": ProximityEventConfigurationTypeDef,
+        "Join": JoinEventConfigurationTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceEventConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -3705,22 +3387,20 @@
     _OptionalUpdateResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
 GetEventConfigurationByResourceTypesResponseTypeDef = TypedDict(
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
-        "DeviceRegistrationState": (
-            DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef
-        ),
-        "Proximity": ProximityResourceTypeEventConfigurationOutputTypeDef,
-        "Join": JoinResourceTypeEventConfigurationOutputTypeDef,
-        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
+        "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
+        "Join": JoinResourceTypeEventConfigurationTypeDef,
+        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
@@ -3735,56 +3415,46 @@
 GetWirelessDeviceStatisticsResponseTypeDef = TypedDict(
     "GetWirelessDeviceStatisticsResponseTypeDef",
     {
         "WirelessDeviceId": str,
         "LastUplinkReceivedAt": str,
         "LoRaWAN": LoRaWANDeviceMetadataTypeDef,
         "Sidewalk": SidewalkDeviceMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessGatewayFirmwareInformationResponseTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     {
         "LoRaWAN": LoRaWANGatewayCurrentVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWirelessGatewayTaskCreateOutputTypeDef = TypedDict(
-    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
+UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
+    "UpdateWirelessGatewayTaskCreateTypeDef",
     {
         "UpdateDataSource": str,
         "UpdateDataRole": str,
-        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
+        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
     },
     total=False,
 )
 
 UpdateWirelessGatewayTaskEntryTypeDef = TypedDict(
     "UpdateWirelessGatewayTaskEntryTypeDef",
     {
         "Id": str,
         "LoRaWAN": LoRaWANUpdateGatewayTaskEntryTypeDef,
         "Arn": str,
     },
     total=False,
 )
 
-UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
-    "UpdateWirelessGatewayTaskCreateTypeDef",
-    {
-        "UpdateDataSource": str,
-        "UpdateDataRole": str,
-        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
-    },
-    total=False,
-)
-
 SendDataToMulticastGroupRequestRequestTypeDef = TypedDict(
     "SendDataToMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
         "PayloadData": str,
         "WirelessMetadata": MulticastWirelessMetadataTypeDef,
     },
@@ -3813,15 +3483,15 @@
     pass
 
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PositionConfigurationItemTypeDef = TypedDict(
     "PositionConfigurationItemTypeDef",
     {
         "ResourceIdentifier": str,
@@ -3834,15 +3504,15 @@
 
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
         "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
         "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
@@ -3853,24 +3523,24 @@
 )
 
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWirelessDevicesResponseTypeDef = TypedDict(
     "ListWirelessDevicesResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessDeviceResponseTypeDef = TypedDict(
     "GetWirelessDeviceResponseTypeDef",
     {
         "Type": WirelessDeviceTypeType,
@@ -3880,15 +3550,15 @@
         "Id": str,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
         "LoRaWAN": LoRaWANDeviceOutputTypeDef,
         "Sidewalk": SidewalkDeviceTypeDef,
         "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
@@ -3978,34 +3648,14 @@
         "IdentifierType": IdentifierTypeType,
         "PartnerType": Literal["Sidewalk"],
         "Events": EventNotificationItemConfigurationsTypeDef,
     },
     total=False,
 )
 
-GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "AutoCreateTasks": bool,
-        "Name": str,
-        "Update": UpdateWirelessGatewayTaskCreateOutputTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "AutoCreateTasks": bool,
     },
 )
 _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
@@ -4021,29 +3671,49 @@
 
 class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
+GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "AutoCreateTasks": bool,
+        "Name": str,
+        "Update": UpdateWirelessGatewayTaskCreateTypeDef,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPositionConfigurationsResponseTypeDef = TypedDict(
     "ListPositionConfigurationsResponseTypeDef",
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendDataToWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
@@ -4078,10 +3748,10 @@
 )
 
 ListEventConfigurationsResponseTypeDef = TypedDict(
     "ListEventConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "EventConfigurationsList": List[EventConfigurationItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/PKG-INFO` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTWireless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,58 +335,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
-    SessionKeysAbpV10XOutputTypeDef,
     SessionKeysAbpV10XTypeDef,
-    SessionKeysAbpV11OutputTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
-    ApplicationConfigOutputTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
-    SidewalkAccountInfoOutputTypeDef,
+    ResponseMetadataTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
-    AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
     BeaconingOutputTypeDef,
     BeaconingTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
-    LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
-    LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
-    CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
-    CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
-    CreateMulticastGroupResponseTypeDef,
     TraceContentTypeDef,
-    CreateNetworkAnalyzerConfigurationResponseTypeDef,
     LoRaWANServiceProfileTypeDef,
-    CreateServiceProfileResponseTypeDef,
     SidewalkCreateWirelessDeviceTypeDef,
-    CreateWirelessDeviceResponseTypeDef,
-    CreateWirelessGatewayResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
     CreateWirelessGatewayTaskRequestRequestTypeDef,
-    CreateWirelessGatewayTaskResponseTypeDef,
     DakCertificateMetadataTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteDeviceProfileRequestRequestTypeDef,
     DeleteFuotaTaskRequestRequestTypeDef,
     DeleteMulticastGroupRequestRequestTypeDef,
     DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef,
     DeleteQueuedMessagesRequestRequestTypeDef,
@@ -395,79 +379,64 @@
     DeleteWirelessDeviceRequestRequestTypeDef,
     DeleteWirelessGatewayRequestRequestTypeDef,
     DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     DeleteWirelessGatewayTaskRequestRequestTypeDef,
     DeregisterWirelessDeviceRequestRequestTypeDef,
     DestinationsTypeDef,
     DeviceProfileTypeDef,
-    SidewalkEventNotificationConfigurationsOutputTypeDef,
     SidewalkEventNotificationConfigurationsTypeDef,
-    SidewalkResourceTypeEventConfigurationOutputTypeDef,
     SidewalkResourceTypeEventConfigurationTypeDef,
     DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef,
     DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
-    PositioningOutputTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
-    GatewayListItemOutputTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
     LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
     LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
-    TraceContentOutputTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
     WiFiAccessPointTypeDef,
-    GetPositionEstimateResponseTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
-    GetResourceLogLevelResponseTypeDef,
     GetResourcePositionRequestRequestTypeDef,
-    GetResourcePositionResponseTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
-    GetServiceEndpointResponseTypeDef,
     GetServiceProfileRequestRequestTypeDef,
     LoRaWANGetServiceProfileInfoTypeDef,
     GetWirelessDeviceImportTaskRequestRequestTypeDef,
     SidewalkGetStartImportInfoTypeDef,
     GetWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceStatisticsRequestRequestTypeDef,
     SidewalkDeviceMetadataTypeDef,
     GetWirelessGatewayCertificateRequestRequestTypeDef,
-    GetWirelessGatewayCertificateResponseTypeDef,
     GetWirelessGatewayFirmwareInformationRequestRequestTypeDef,
     GetWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayStatisticsRequestRequestTypeDef,
-    GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
-    GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
-    LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
-    LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
     ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     ListEventConfigurationsRequestRequestTypeDef,
     ListFuotaTasksRequestRequestTypeDef,
     ListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
@@ -478,137 +447,136 @@
     NetworkAnalyzerConfigurationsTypeDef,
     ListPartnerAccountsRequestRequestTypeDef,
     ListPositionConfigurationsRequestRequestTypeDef,
     ListQueuedMessagesRequestRequestTypeDef,
     ListServiceProfilesRequestRequestTypeDef,
     ServiceProfileTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListWirelessDeviceImportTasksRequestRequestTypeDef,
     ListWirelessDevicesRequestRequestTypeDef,
     ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef,
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
-    OtaaV10XOutputTypeDef,
-    OtaaV11OutputTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
-    LoRaWANGatewayVersionOutputTypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
     LoRaWANMulticastSessionTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
     ResetResourceLogLevelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendDataToMulticastGroupResponseTypeDef,
-    SendDataToWirelessDeviceResponseTypeDef,
     SidewalkSendDataToDeviceTypeDef,
     SidewalkSingleStartImportInfoTypeDef,
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
-    StartSingleWirelessDeviceImportTaskResponseTypeDef,
-    StartWirelessDeviceImportTaskResponseTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
-    TestWirelessDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
     UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
-    WirelessDeviceEventLogOptionOutputTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
-    WirelessGatewayEventLogOptionOutputTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
-    AbpV10XOutputTypeDef,
     AbpV10XTypeDef,
-    AbpV11OutputTypeDef,
     AbpV11TypeDef,
-    GetPositionResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateDeviceProfileResponseTypeDef,
+    CreateFuotaTaskResponseTypeDef,
+    CreateMulticastGroupResponseTypeDef,
+    CreateNetworkAnalyzerConfigurationResponseTypeDef,
+    CreateServiceProfileResponseTypeDef,
+    CreateWirelessDeviceResponseTypeDef,
+    CreateWirelessGatewayResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
+    CreateWirelessGatewayTaskResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetPositionEstimateResponseTypeDef,
+    GetPositionResponseTypeDef,
+    GetResourceLogLevelResponseTypeDef,
+    GetResourcePositionResponseTypeDef,
+    GetServiceEndpointResponseTypeDef,
+    GetWirelessGatewayCertificateResponseTypeDef,
+    GetWirelessGatewayStatisticsResponseTypeDef,
+    GetWirelessGatewayTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendDataToMulticastGroupResponseTypeDef,
+    SendDataToWirelessDeviceResponseTypeDef,
+    StartSingleWirelessDeviceImportTaskResponseTypeDef,
+    StartWirelessDeviceImportTaskResponseTypeDef,
+    TestWirelessDeviceResponseTypeDef,
     LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
-    ConnectionStatusEventConfigurationOutputTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
-    ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
     UpdateFuotaTaskRequestRequestTypeDef,
     CreateMulticastGroupRequestRequestTypeDef,
     UpdateMulticastGroupRequestRequestTypeDef,
     CreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
+    GetNetworkAnalyzerConfigurationResponseTypeDef,
     UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     CreateServiceProfileRequestRequestTypeDef,
     SidewalkGetDeviceProfileTypeDef,
     ListDestinationsResponseTypeDef,
     ListDeviceProfilesResponseTypeDef,
-    DeviceRegistrationStateEventConfigurationOutputTypeDef,
-    MessageDeliveryStatusEventConfigurationOutputTypeDef,
-    ProximityEventConfigurationOutputTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
-    DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef,
-    MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
-    ProximityResourceTypeEventConfigurationOutputTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
     FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
     ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    GetNetworkAnalyzerConfigurationResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
-    JoinEventConfigurationOutputTypeDef,
     JoinEventConfigurationTypeDef,
-    JoinResourceTypeEventConfigurationOutputTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
     ListMulticastGroupsByFuotaTaskResponseTypeDef,
     ListMulticastGroupsResponseTypeDef,
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
-    LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
-    LoRaWANUpdateGatewayTaskEntryTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
+    LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
     StartMulticastGroupSessionRequestRequestTypeDef,
     StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
@@ -637,17 +605,16 @@
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
     UpdateEventConfigurationByResourceTypesRequestRequestTypeDef,
     GetWirelessDeviceStatisticsResponseTypeDef,
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
-    UpdateWirelessGatewayTaskCreateOutputTypeDef,
-    UpdateWirelessGatewayTaskEntryTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
+    UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
     UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListWirelessGatewaysResponseTypeDef,
@@ -655,26 +622,26 @@
     GetWirelessDeviceResponseTypeDef,
     CreateWirelessDeviceRequestRequestTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
+    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     ListPositionConfigurationsResponseTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XOutputTypeDef:
+def get_structure() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/SOURCES.txt` & `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.12/setup.py` & `mypy-boto3-iotwireless-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotwireless",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTWireless 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

