# Comparing `tmp/mypy-boto3-iotfleetwise-1.28.12.tar.gz` & `tmp/mypy-boto3-iotfleetwise-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iotfleetwise-1.28.12.tar` & `mypy-boto3-iotfleetwise-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.928481 mypy-boto3-iotfleetwise-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22130 2023-07-27 05:34:49.920481 mypy-boto3-iotfleetwise-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20623 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.920481 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40870 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40800 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-27 05:24:08.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67924 2023-07-27 05:24:08.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.920481 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22130 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.928481 mypy-boto3-iotfleetwise-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.549258 mypy-boto3-iotfleetwise-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-28 20:42:59.541258 mypy-boto3-iotfleetwise-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.529258 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40870 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40800 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-28 20:28:29.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60272 2023-07-28 20:28:31.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60166 2023-07-28 20:28:30.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.541258 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.549258 mypy-boto3-iotfleetwise-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/LICENSE` & `mypy-boto3-iotfleetwise-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTFleetWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,177 +399,159 @@
     ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
     AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
+    ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
-    BranchOutputTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
     CanDbcDefinitionTypeDef,
-    CanInterfaceOutputTypeDef,
     CanInterfaceTypeDef,
-    CanSignalOutputTypeDef,
     CanSignalTypeDef,
-    CloudWatchLogDeliveryOptionsOutputTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
-    ConditionBasedCollectionSchemeOutputTypeDef,
-    TimeBasedCollectionSchemeOutputTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDecoderManifestResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateModelManifestResponseTypeDef,
-    CreateSignalCatalogResponseTypeDef,
-    CreateVehicleResponseTypeDef,
-    S3ConfigOutputTypeDef,
-    TimestreamConfigOutputTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
-    DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
-    DeleteDecoderManifestResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
-    DeleteFleetResponseTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
-    DeleteModelManifestResponseTypeDef,
     DeleteSignalCatalogRequestRequestTypeDef,
-    DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
-    DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
-    SignalInformationOutputTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
-    GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
-    GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
-    GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
     TimestreamRegistrationResponseTypeDef,
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
-    GetVehicleResponseTypeDef,
-    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
-    IamResourcesOutputTypeDef,
     IamResourcesTypeDef,
-    ImportDecoderManifestResponseTypeDef,
-    ImportSignalCatalogResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
-    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
-    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
     ListDecoderManifestSignalsRequestRequestTypeDef,
-    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
     ListDecoderManifestsRequestRequestTypeDef,
-    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
     ListFleetsForVehicleRequestRequestTypeDef,
-    ListFleetsForVehicleResponseTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
     ListModelManifestNodesRequestRequestTypeDef,
-    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
     ListModelManifestsRequestRequestTypeDef,
     ModelManifestSummaryTypeDef,
-    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
-    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
-    ListVehiclesInFleetResponseTypeDef,
-    ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
-    ObdInterfaceOutputTypeDef,
     ObdInterfaceTypeDef,
     SensorOutputTypeDef,
     SensorTypeDef,
-    ObdSignalOutputTypeDef,
     ObdSignalTypeDef,
-    PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
-    TimestreamResourcesOutputTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    UpdateFleetRequestRequestTypeDef,
+    UpdateModelManifestRequestRequestTypeDef,
+    UpdateVehicleRequestRequestTypeDef,
+    BatchCreateVehicleResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDecoderManifestResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateModelManifestResponseTypeDef,
+    CreateSignalCatalogResponseTypeDef,
+    CreateVehicleResponseTypeDef,
+    DeleteCampaignResponseTypeDef,
+    DeleteDecoderManifestResponseTypeDef,
+    DeleteFleetResponseTypeDef,
+    DeleteModelManifestResponseTypeDef,
+    DeleteSignalCatalogResponseTypeDef,
+    DeleteVehicleResponseTypeDef,
+    GetDecoderManifestResponseTypeDef,
+    GetFleetResponseTypeDef,
+    GetModelManifestResponseTypeDef,
+    GetVehicleResponseTypeDef,
+    ImportDecoderManifestResponseTypeDef,
+    ImportSignalCatalogResponseTypeDef,
+    ListFleetsForVehicleResponseTypeDef,
+    ListVehiclesInFleetResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
-    UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
-    UpdateModelManifestRequestRequestTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
-    UpdateVehicleRequestRequestTypeDef,
     UpdateVehicleResponseTypeDef,
-    BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
     ListCampaignsResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    CollectionSchemeOutputTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    DataDestinationConfigOutputTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
+    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
+    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
+    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
+    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
+    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    ListVehiclesRequestListVehiclesPaginateTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVehiclesResponseTypeDef,
-    NetworkInterfaceOutputTypeDef,
     NetworkInterfaceTypeDef,
     NodeOutputTypeDef,
     NodeTypeDef,
-    SignalDecoderOutputTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
     ImportDecoderManifestRequestRequestTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
-    GetCampaignResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
+    GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
     CreateSignalCatalogRequestRequestTypeDef,
     UpdateSignalCatalogRequestRequestTypeDef,
-    ListDecoderManifestSignalsResponseTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
+    ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ActuatorOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/README.md` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iotfleetwise
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotfleetwise"></a>
 
 # mypy-boto3-iotfleetwise
 
 [![PyPI - mypy-boto3-iotfleetwise](https://img.shields.io/pypi/v/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,177 +399,159 @@
     ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
     AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
+    ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
-    BranchOutputTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
     CanDbcDefinitionTypeDef,
-    CanInterfaceOutputTypeDef,
     CanInterfaceTypeDef,
-    CanSignalOutputTypeDef,
     CanSignalTypeDef,
-    CloudWatchLogDeliveryOptionsOutputTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
-    ConditionBasedCollectionSchemeOutputTypeDef,
-    TimeBasedCollectionSchemeOutputTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDecoderManifestResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateModelManifestResponseTypeDef,
-    CreateSignalCatalogResponseTypeDef,
-    CreateVehicleResponseTypeDef,
-    S3ConfigOutputTypeDef,
-    TimestreamConfigOutputTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
-    DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
-    DeleteDecoderManifestResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
-    DeleteFleetResponseTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
-    DeleteModelManifestResponseTypeDef,
     DeleteSignalCatalogRequestRequestTypeDef,
-    DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
-    DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
-    SignalInformationOutputTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
-    GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
-    GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
-    GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
     TimestreamRegistrationResponseTypeDef,
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
-    GetVehicleResponseTypeDef,
-    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
-    IamResourcesOutputTypeDef,
     IamResourcesTypeDef,
-    ImportDecoderManifestResponseTypeDef,
-    ImportSignalCatalogResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
-    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
-    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
     ListDecoderManifestSignalsRequestRequestTypeDef,
-    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
     ListDecoderManifestsRequestRequestTypeDef,
-    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
     ListFleetsForVehicleRequestRequestTypeDef,
-    ListFleetsForVehicleResponseTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
     ListModelManifestNodesRequestRequestTypeDef,
-    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
     ListModelManifestsRequestRequestTypeDef,
     ModelManifestSummaryTypeDef,
-    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
-    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
-    ListVehiclesInFleetResponseTypeDef,
-    ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
-    ObdInterfaceOutputTypeDef,
     ObdInterfaceTypeDef,
     SensorOutputTypeDef,
     SensorTypeDef,
-    ObdSignalOutputTypeDef,
     ObdSignalTypeDef,
-    PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
-    TimestreamResourcesOutputTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    UpdateFleetRequestRequestTypeDef,
+    UpdateModelManifestRequestRequestTypeDef,
+    UpdateVehicleRequestRequestTypeDef,
+    BatchCreateVehicleResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDecoderManifestResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateModelManifestResponseTypeDef,
+    CreateSignalCatalogResponseTypeDef,
+    CreateVehicleResponseTypeDef,
+    DeleteCampaignResponseTypeDef,
+    DeleteDecoderManifestResponseTypeDef,
+    DeleteFleetResponseTypeDef,
+    DeleteModelManifestResponseTypeDef,
+    DeleteSignalCatalogResponseTypeDef,
+    DeleteVehicleResponseTypeDef,
+    GetDecoderManifestResponseTypeDef,
+    GetFleetResponseTypeDef,
+    GetModelManifestResponseTypeDef,
+    GetVehicleResponseTypeDef,
+    ImportDecoderManifestResponseTypeDef,
+    ImportSignalCatalogResponseTypeDef,
+    ListFleetsForVehicleResponseTypeDef,
+    ListVehiclesInFleetResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
-    UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
-    UpdateModelManifestRequestRequestTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
-    UpdateVehicleRequestRequestTypeDef,
     UpdateVehicleResponseTypeDef,
-    BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
     ListCampaignsResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    CollectionSchemeOutputTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    DataDestinationConfigOutputTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
+    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
+    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
+    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
+    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
+    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    ListVehiclesRequestListVehiclesPaginateTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVehiclesResponseTypeDef,
-    NetworkInterfaceOutputTypeDef,
     NetworkInterfaceTypeDef,
     NodeOutputTypeDef,
     NodeTypeDef,
-    SignalDecoderOutputTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
     ImportDecoderManifestRequestRequestTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
-    GetCampaignResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
+    GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
     CreateSignalCatalogRequestRequestTypeDef,
     UpdateSignalCatalogRequestRequestTypeDef,
-    ListDecoderManifestSignalsResponseTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
+    ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ActuatorOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.py` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.pyi` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__main__.py` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetWise 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTFleetWise 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.py` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.pyi` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.py` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.pyi` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.py` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,211 +76,196 @@
     "ListModelManifestsPaginator",
     "ListSignalCatalogNodesPaginator",
     "ListSignalCatalogsPaginator",
     "ListVehiclesPaginator",
     "ListVehiclesInFleetPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetVehicleStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#getvehiclestatuspaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetVehicleStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#getvehiclestatuspaginator)
         """
 
-
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listcampaignspaginator)
     """
 
     def paginate(
-        self, *, status: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listcampaignspaginator)
         """
 
-
 class ListDecoderManifestNetworkInterfacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
         """
 
-
 class ListDecoderManifestSignalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDecoderManifestSignalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
         """
 
-
 class ListDecoderManifestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestspaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDecoderManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestspaginator)
         """
 
-
 class ListFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetspaginator)
         """
 
-
 class ListFleetsForVehiclePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetsForVehicleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
         """
 
-
 class ListModelManifestNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelManifestNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
         """
 
-
 class ListModelManifestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestspaginator)
     """
 
     def paginate(
-        self, *, signalCatalogArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, signalCatalogArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestspaginator)
         """
 
-
 class ListSignalCatalogNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSignalCatalogNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
         """
 
-
 class ListSignalCatalogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSignalCatalogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalogspaginator)
         """
 
-
 class ListVehiclesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclespaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVehiclesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclespaginator)
         """
 
-
 class ListVehiclesInFleetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
     """
 
     def paginate(
-        self, *, fleetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, fleetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVehiclesInFleetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
         """
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.pyi` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,196 +76,211 @@
     "ListModelManifestsPaginator",
     "ListSignalCatalogNodesPaginator",
     "ListSignalCatalogsPaginator",
     "ListVehiclesPaginator",
     "ListVehiclesInFleetPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetVehicleStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#getvehiclestatuspaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetVehicleStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#getvehiclestatuspaginator)
         """
 
+
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listcampaignspaginator)
     """
 
     def paginate(
-        self, *, status: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listcampaignspaginator)
         """
 
+
 class ListDecoderManifestNetworkInterfacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
         """
 
+
 class ListDecoderManifestSignalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDecoderManifestSignalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
         """
 
+
 class ListDecoderManifestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestspaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDecoderManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listdecodermanifestspaginator)
         """
 
+
 class ListFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetspaginator)
         """
 
+
 class ListFleetsForVehiclePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetsForVehicleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
         """
 
+
 class ListModelManifestNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelManifestNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
         """
 
+
 class ListModelManifestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestspaginator)
     """
 
     def paginate(
-        self, *, signalCatalogArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, signalCatalogArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listmodelmanifestspaginator)
         """
 
+
 class ListSignalCatalogNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSignalCatalogNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
         """
 
+
 class ListSignalCatalogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSignalCatalogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalogspaginator)
         """
 
+
 class ListVehiclesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclespaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVehiclesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclespaginator)
         """
 
+
 class ListVehiclesInFleetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
     """
 
     def paginate(
-        self, *, fleetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, fleetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVehiclesInFleetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
         """
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.py` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -38,186 +38,167 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
     "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
-    "BranchOutputTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
     "CanDbcDefinitionTypeDef",
-    "CanInterfaceOutputTypeDef",
     "CanInterfaceTypeDef",
-    "CanSignalOutputTypeDef",
     "CanSignalTypeDef",
-    "CloudWatchLogDeliveryOptionsOutputTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
-    "ConditionBasedCollectionSchemeOutputTypeDef",
-    "TimeBasedCollectionSchemeOutputTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDecoderManifestResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "CreateModelManifestResponseTypeDef",
-    "CreateSignalCatalogResponseTypeDef",
-    "CreateVehicleResponseTypeDef",
-    "S3ConfigOutputTypeDef",
-    "TimestreamConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
-    "DeleteCampaignResponseTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
-    "DeleteDecoderManifestResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
-    "DeleteFleetResponseTypeDef",
     "DeleteModelManifestRequestRequestTypeDef",
-    "DeleteModelManifestResponseTypeDef",
     "DeleteSignalCatalogRequestRequestTypeDef",
-    "DeleteSignalCatalogResponseTypeDef",
     "DeleteVehicleRequestRequestTypeDef",
-    "DeleteVehicleResponseTypeDef",
     "DisassociateVehicleFleetRequestRequestTypeDef",
     "FleetSummaryTypeDef",
     "FormattedVssTypeDef",
     "GetCampaignRequestRequestTypeDef",
-    "SignalInformationOutputTypeDef",
     "GetDecoderManifestRequestRequestTypeDef",
-    "GetDecoderManifestResponseTypeDef",
     "GetFleetRequestRequestTypeDef",
-    "GetFleetResponseTypeDef",
     "GetModelManifestRequestRequestTypeDef",
-    "GetModelManifestResponseTypeDef",
     "IamRegistrationResponseTypeDef",
     "TimestreamRegistrationResponseTypeDef",
     "GetSignalCatalogRequestRequestTypeDef",
     "NodeCountsTypeDef",
     "GetVehicleRequestRequestTypeDef",
-    "GetVehicleResponseTypeDef",
-    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetVehicleStatusRequestRequestTypeDef",
     "VehicleStatusTypeDef",
-    "IamResourcesOutputTypeDef",
     "IamResourcesTypeDef",
-    "ImportDecoderManifestResponseTypeDef",
-    "ImportSignalCatalogResponseTypeDef",
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
-    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
-    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
     "ListDecoderManifestSignalsRequestRequestTypeDef",
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
     "ListDecoderManifestsRequestRequestTypeDef",
-    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
     "ListFleetsForVehicleRequestRequestTypeDef",
-    "ListFleetsForVehicleResponseTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
     "ListModelManifestNodesRequestRequestTypeDef",
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
     "ListModelManifestsRequestRequestTypeDef",
     "ModelManifestSummaryTypeDef",
-    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     "ListSignalCatalogNodesRequestRequestTypeDef",
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
-    "ListVehiclesInFleetResponseTypeDef",
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
-    "ObdInterfaceOutputTypeDef",
     "ObdInterfaceTypeDef",
     "SensorOutputTypeDef",
     "SensorTypeDef",
-    "ObdSignalOutputTypeDef",
     "ObdSignalTypeDef",
-    "PaginatorConfigTypeDef",
     "TimestreamResourcesTypeDef",
-    "TimestreamResourcesOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
+    "UpdateFleetRequestRequestTypeDef",
+    "UpdateModelManifestRequestRequestTypeDef",
+    "UpdateVehicleRequestRequestTypeDef",
+    "BatchCreateVehicleResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDecoderManifestResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateModelManifestResponseTypeDef",
+    "CreateSignalCatalogResponseTypeDef",
+    "CreateVehicleResponseTypeDef",
+    "DeleteCampaignResponseTypeDef",
+    "DeleteDecoderManifestResponseTypeDef",
+    "DeleteFleetResponseTypeDef",
+    "DeleteModelManifestResponseTypeDef",
+    "DeleteSignalCatalogResponseTypeDef",
+    "DeleteVehicleResponseTypeDef",
+    "GetDecoderManifestResponseTypeDef",
+    "GetFleetResponseTypeDef",
+    "GetModelManifestResponseTypeDef",
+    "GetVehicleResponseTypeDef",
+    "ImportDecoderManifestResponseTypeDef",
+    "ImportSignalCatalogResponseTypeDef",
+    "ListFleetsForVehicleResponseTypeDef",
+    "ListVehiclesInFleetResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDecoderManifestResponseTypeDef",
-    "UpdateFleetRequestRequestTypeDef",
     "UpdateFleetResponseTypeDef",
-    "UpdateModelManifestRequestRequestTypeDef",
     "UpdateModelManifestResponseTypeDef",
     "UpdateSignalCatalogResponseTypeDef",
-    "UpdateVehicleRequestRequestTypeDef",
     "UpdateVehicleResponseTypeDef",
-    "BatchCreateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
-    "CollectionSchemeOutputTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "DataDestinationConfigOutputTypeDef",
     "DataDestinationConfigTypeDef",
     "ListDecoderManifestsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ImportSignalCatalogRequestRequestTypeDef",
     "GetRegisterAccountStatusResponseTypeDef",
     "GetSignalCatalogResponseTypeDef",
+    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVehiclesResponseTypeDef",
-    "NetworkInterfaceOutputTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeOutputTypeDef",
     "NodeTypeDef",
-    "SignalDecoderOutputTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
     "ImportDecoderManifestRequestRequestTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
-    "GetCampaignResponseTypeDef",
     "CreateCampaignRequestRequestTypeDef",
+    "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
     "CreateSignalCatalogRequestRequestTypeDef",
     "UpdateSignalCatalogRequestRequestTypeDef",
-    "ListDecoderManifestSignalsResponseTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
+    "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
 )
 
 _RequiredActuatorOutputTypeDef = TypedDict(
     "_RequiredActuatorOutputTypeDef",
     {
         "fullyQualifiedName": str,
@@ -235,19 +216,17 @@
         "assignedValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
     pass
 
-
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -262,19 +241,17 @@
         "assignedValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class ActuatorTypeDef(_RequiredActuatorTypeDef, _OptionalActuatorTypeDef):
     pass
 
-
 AssociateVehicleFleetRequestRequestTypeDef = TypedDict(
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
@@ -298,19 +275,17 @@
         "defaultValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
     pass
 
-
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -326,19 +301,17 @@
         "defaultValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 CreateVehicleErrorTypeDef = TypedDict(
     "CreateVehicleErrorTypeDef",
     {
         "vehicleName": str,
         "code": str,
         "message": str,
     },
@@ -351,14 +324,25 @@
         "vehicleName": str,
         "arn": str,
         "thingArn": str,
     },
     total=False,
 )
 
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
 _RequiredUpdateVehicleRequestItemTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestItemTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalUpdateVehicleRequestItemTypeDef = TypedDict(
@@ -368,21 +352,19 @@
         "decoderManifestArn": str,
         "attributes": Mapping[str, str],
         "attributeUpdateMode": UpdateModeType,
     },
     total=False,
 )
 
-
 class UpdateVehicleRequestItemTypeDef(
     _RequiredUpdateVehicleRequestItemTypeDef, _OptionalUpdateVehicleRequestItemTypeDef
 ):
     pass
 
-
 UpdateVehicleErrorTypeDef = TypedDict(
     "UpdateVehicleErrorTypeDef",
     {
         "vehicleName": str,
         "code": int,
         "message": str,
     },
@@ -394,35 +376,14 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
-_RequiredBranchOutputTypeDef = TypedDict(
-    "_RequiredBranchOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-    },
-)
-_OptionalBranchOutputTypeDef = TypedDict(
-    "_OptionalBranchOutputTypeDef",
-    {
-        "description": str,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
-)
-
-
-class BranchOutputTypeDef(_RequiredBranchOutputTypeDef, _OptionalBranchOutputTypeDef):
-    pass
-
-
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -431,19 +392,17 @@
         "description": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class BranchTypeDef(_RequiredBranchTypeDef, _OptionalBranchTypeDef):
     pass
 
-
 _RequiredCampaignSummaryTypeDef = TypedDict(
     "_RequiredCampaignSummaryTypeDef",
     {
         "creationTime": datetime,
         "lastModificationTime": datetime,
     },
 )
@@ -456,19 +415,17 @@
         "signalCatalogArn": str,
         "targetArn": str,
         "status": CampaignStatusType,
     },
     total=False,
 )
 
-
 class CampaignSummaryTypeDef(_RequiredCampaignSummaryTypeDef, _OptionalCampaignSummaryTypeDef):
     pass
 
-
 _RequiredCanDbcDefinitionTypeDef = TypedDict(
     "_RequiredCanDbcDefinitionTypeDef",
     {
         "networkInterface": str,
         "canDbcFiles": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
 )
@@ -476,41 +433,17 @@
     "_OptionalCanDbcDefinitionTypeDef",
     {
         "signalsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
     pass
 
-
-_RequiredCanInterfaceOutputTypeDef = TypedDict(
-    "_RequiredCanInterfaceOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCanInterfaceOutputTypeDef = TypedDict(
-    "_OptionalCanInterfaceOutputTypeDef",
-    {
-        "protocolName": str,
-        "protocolVersion": str,
-    },
-    total=False,
-)
-
-
-class CanInterfaceOutputTypeDef(
-    _RequiredCanInterfaceOutputTypeDef, _OptionalCanInterfaceOutputTypeDef
-):
-    pass
-
-
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -518,44 +451,17 @@
     {
         "protocolName": str,
         "protocolVersion": str,
     },
     total=False,
 )
 
-
 class CanInterfaceTypeDef(_RequiredCanInterfaceTypeDef, _OptionalCanInterfaceTypeDef):
     pass
 
-
-_RequiredCanSignalOutputTypeDef = TypedDict(
-    "_RequiredCanSignalOutputTypeDef",
-    {
-        "messageId": int,
-        "isBigEndian": bool,
-        "isSigned": bool,
-        "startBit": int,
-        "offset": float,
-        "factor": float,
-        "length": int,
-    },
-)
-_OptionalCanSignalOutputTypeDef = TypedDict(
-    "_OptionalCanSignalOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-
-class CanSignalOutputTypeDef(_RequiredCanSignalOutputTypeDef, _OptionalCanSignalOutputTypeDef):
-    pass
-
-
 _RequiredCanSignalTypeDef = TypedDict(
     "_RequiredCanSignalTypeDef",
     {
         "messageId": int,
         "isBigEndian": bool,
         "isSigned": bool,
         "startBit": int,
@@ -568,93 +474,36 @@
     "_OptionalCanSignalTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-
 class CanSignalTypeDef(_RequiredCanSignalTypeDef, _OptionalCanSignalTypeDef):
     pass
 
-
-_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef",
-    {
-        "logType": LogTypeType,
-    },
-)
-_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef",
-    {
-        "logGroupName": str,
-    },
-    total=False,
-)
-
-
-class CloudWatchLogDeliveryOptionsOutputTypeDef(
-    _RequiredCloudWatchLogDeliveryOptionsOutputTypeDef,
-    _OptionalCloudWatchLogDeliveryOptionsOutputTypeDef,
-):
-    pass
-
-
 _RequiredCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
     "_RequiredCloudWatchLogDeliveryOptionsTypeDef",
     {
         "logType": LogTypeType,
     },
 )
 _OptionalCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
     "_OptionalCloudWatchLogDeliveryOptionsTypeDef",
     {
         "logGroupName": str,
     },
     total=False,
 )
 
-
 class CloudWatchLogDeliveryOptionsTypeDef(
     _RequiredCloudWatchLogDeliveryOptionsTypeDef, _OptionalCloudWatchLogDeliveryOptionsTypeDef
 ):
     pass
 
-
-_RequiredConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
-    "_RequiredConditionBasedCollectionSchemeOutputTypeDef",
-    {
-        "expression": str,
-    },
-)
-_OptionalConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
-    "_OptionalConditionBasedCollectionSchemeOutputTypeDef",
-    {
-        "minimumTriggerIntervalMs": int,
-        "triggerMode": TriggerModeType,
-        "conditionLanguageVersion": int,
-    },
-    total=False,
-)
-
-
-class ConditionBasedCollectionSchemeOutputTypeDef(
-    _RequiredConditionBasedCollectionSchemeOutputTypeDef,
-    _OptionalConditionBasedCollectionSchemeOutputTypeDef,
-):
-    pass
-
-
-TimeBasedCollectionSchemeOutputTypeDef = TypedDict(
-    "TimeBasedCollectionSchemeOutputTypeDef",
-    {
-        "periodMs": int,
-    },
-)
-
 _RequiredConditionBasedCollectionSchemeTypeDef = TypedDict(
     "_RequiredConditionBasedCollectionSchemeTypeDef",
     {
         "expression": str,
     },
 )
 _OptionalConditionBasedCollectionSchemeTypeDef = TypedDict(
@@ -663,21 +512,19 @@
         "minimumTriggerIntervalMs": int,
         "triggerMode": TriggerModeType,
         "conditionLanguageVersion": int,
     },
     total=False,
 )
 
-
 class ConditionBasedCollectionSchemeTypeDef(
     _RequiredConditionBasedCollectionSchemeTypeDef, _OptionalConditionBasedCollectionSchemeTypeDef
 ):
     pass
 
-
 TimeBasedCollectionSchemeTypeDef = TypedDict(
     "TimeBasedCollectionSchemeTypeDef",
     {
         "periodMs": int,
     },
 )
 
@@ -692,113 +539,27 @@
     {
         "maxSampleCount": int,
         "minimumSamplingIntervalMs": int,
     },
     total=False,
 )
 
-
 class SignalInformationTypeDef(
     _RequiredSignalInformationTypeDef, _OptionalSignalInformationTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDecoderManifestResponseTypeDef = TypedDict(
-    "CreateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateModelManifestResponseTypeDef = TypedDict(
-    "CreateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSignalCatalogResponseTypeDef = TypedDict(
-    "CreateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVehicleResponseTypeDef = TypedDict(
-    "CreateVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "thingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3ConfigOutputTypeDef = TypedDict(
-    "_RequiredS3ConfigOutputTypeDef",
-    {
-        "bucketArn": str,
-    },
-)
-_OptionalS3ConfigOutputTypeDef = TypedDict(
-    "_OptionalS3ConfigOutputTypeDef",
-    {
-        "dataFormat": DataFormatType,
-        "storageCompressionFormat": StorageCompressionFormatType,
-        "prefix": str,
-    },
-    total=False,
-)
-
-
-class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
-    pass
-
-
-TimestreamConfigOutputTypeDef = TypedDict(
-    "TimestreamConfigOutputTypeDef",
-    {
-        "timestreamTableArn": str,
-        "executionRoleArn": str,
-    },
-)
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -807,19 +568,17 @@
         "dataFormat": DataFormatType,
         "storageCompressionFormat": StorageCompressionFormatType,
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
-
 TimestreamConfigTypeDef = TypedDict(
     "TimestreamConfigTypeDef",
     {
         "timestreamTableArn": str,
         "executionRoleArn": str,
     },
 )
@@ -839,117 +598,61 @@
         "modelManifestArn": str,
         "description": str,
         "status": ManifestStatusType,
     },
     total=False,
 )
 
-
 class DecoderManifestSummaryTypeDef(
     _RequiredDecoderManifestSummaryTypeDef, _OptionalDecoderManifestSummaryTypeDef
 ):
     pass
 
-
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteCampaignResponseTypeDef = TypedDict(
-    "DeleteCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDecoderManifestRequestRequestTypeDef = TypedDict(
     "DeleteDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteDecoderManifestResponseTypeDef = TypedDict(
-    "DeleteDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-DeleteFleetResponseTypeDef = TypedDict(
-    "DeleteFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteModelManifestRequestRequestTypeDef = TypedDict(
     "DeleteModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteModelManifestResponseTypeDef = TypedDict(
-    "DeleteModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSignalCatalogRequestRequestTypeDef = TypedDict(
     "DeleteSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteSignalCatalogResponseTypeDef = TypedDict(
-    "DeleteSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVehicleRequestRequestTypeDef = TypedDict(
     "DeleteVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-DeleteVehicleResponseTypeDef = TypedDict(
-    "DeleteVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateVehicleFleetRequestRequestTypeDef = TypedDict(
     "DisassociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
@@ -968,19 +671,17 @@
     {
         "description": str,
         "lastModificationTime": datetime,
     },
     total=False,
 )
 
-
 class FleetSummaryTypeDef(_RequiredFleetSummaryTypeDef, _OptionalFleetSummaryTypeDef):
     pass
 
-
 FormattedVssTypeDef = TypedDict(
     "FormattedVssTypeDef",
     {
         "vssJson": str,
     },
     total=False,
 )
@@ -988,98 +689,35 @@
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredSignalInformationOutputTypeDef = TypedDict(
-    "_RequiredSignalInformationOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalSignalInformationOutputTypeDef = TypedDict(
-    "_OptionalSignalInformationOutputTypeDef",
-    {
-        "maxSampleCount": int,
-        "minimumSamplingIntervalMs": int,
-    },
-    total=False,
-)
-
-
-class SignalInformationOutputTypeDef(
-    _RequiredSignalInformationOutputTypeDef, _OptionalSignalInformationOutputTypeDef
-):
-    pass
-
-
 GetDecoderManifestRequestRequestTypeDef = TypedDict(
     "GetDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetDecoderManifestResponseTypeDef = TypedDict(
-    "GetDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "modelManifestArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFleetRequestRequestTypeDef = TypedDict(
     "GetFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-GetFleetResponseTypeDef = TypedDict(
-    "GetFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelManifestRequestRequestTypeDef = TypedDict(
     "GetModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetModelManifestResponseTypeDef = TypedDict(
-    "GetModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIamRegistrationResponseTypeDef = TypedDict(
     "_RequiredIamRegistrationResponseTypeDef",
     {
         "roleArn": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1087,21 +725,19 @@
     "_OptionalIamRegistrationResponseTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
-
 class IamRegistrationResponseTypeDef(
     _RequiredIamRegistrationResponseTypeDef, _OptionalIamRegistrationResponseTypeDef
 ):
     pass
 
-
 _RequiredTimestreamRegistrationResponseTypeDef = TypedDict(
     "_RequiredTimestreamRegistrationResponseTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
         "registrationStatus": RegistrationStatusType,
     },
@@ -1112,21 +748,19 @@
         "timestreamDatabaseArn": str,
         "timestreamTableArn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-
 class TimestreamRegistrationResponseTypeDef(
     _RequiredTimestreamRegistrationResponseTypeDef, _OptionalTimestreamRegistrationResponseTypeDef
 ):
     pass
 
-
 GetSignalCatalogRequestRequestTypeDef = TypedDict(
     "GetSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -1145,50 +779,24 @@
 GetVehicleRequestRequestTypeDef = TypedDict(
     "GetVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-GetVehicleResponseTypeDef = TypedDict(
-    "GetVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "modelManifestArn": str,
-        "decoderManifestArn": str,
-        "attributes": Dict[str, str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
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
-class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
-    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetVehicleStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetVehicleStatusRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalGetVehicleStatusRequestRequestTypeDef = TypedDict(
@@ -1196,104 +804,46 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetVehicleStatusRequestRequestTypeDef(
     _RequiredGetVehicleStatusRequestRequestTypeDef, _OptionalGetVehicleStatusRequestRequestTypeDef
 ):
     pass
 
-
 VehicleStatusTypeDef = TypedDict(
     "VehicleStatusTypeDef",
     {
         "campaignName": str,
         "vehicleName": str,
         "status": VehicleStateType,
     },
     total=False,
 )
 
-IamResourcesOutputTypeDef = TypedDict(
-    "IamResourcesOutputTypeDef",
-    {
-        "roleArn": str,
-    },
-)
-
 IamResourcesTypeDef = TypedDict(
     "IamResourcesTypeDef",
     {
         "roleArn": str,
     },
 )
 
-ImportDecoderManifestResponseTypeDef = TypedDict(
-    "ImportDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportSignalCatalogResponseTypeDef = TypedDict(
-    "ImportSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    {
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": str,
     },
     total=False,
 )
 
-_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
-    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
@@ -1301,44 +851,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListDecoderManifestNetworkInterfacesRequestRequestTypeDef(
     _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
     _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
-    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestSignalsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
@@ -1346,63 +872,30 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListDecoderManifestSignalsRequestRequestTypeDef(
     _RequiredListDecoderManifestSignalsRequestRequestTypeDef,
     _OptionalListDecoderManifestSignalsRequestRequestTypeDef,
 ):
     pass
 
-
-ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDecoderManifestsRequestRequestTypeDef = TypedDict(
     "ListDecoderManifestsRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
-    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFleetsForVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredListFleetsForVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalListFleetsForVehicleRequestRequestTypeDef = TypedDict(
@@ -1410,70 +903,29 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListFleetsForVehicleRequestRequestTypeDef(
     _RequiredListFleetsForVehicleRequestRequestTypeDef,
     _OptionalListFleetsForVehicleRequestRequestTypeDef,
 ):
     pass
 
-
-ListFleetsForVehicleResponseTypeDef = TypedDict(
-    "ListFleetsForVehicleResponseTypeDef",
-    {
-        "fleets": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetsRequestRequestTypeDef = TypedDict(
     "ListFleetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
-    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListModelManifestNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListModelManifestNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListModelManifestNodesRequestRequestTypeDef = TypedDict(
@@ -1481,31 +933,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListModelManifestNodesRequestRequestTypeDef(
     _RequiredListModelManifestNodesRequestRequestTypeDef,
     _OptionalListModelManifestNodesRequestRequestTypeDef,
 ):
     pass
 
-
-ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
-    {
-        "signalCatalogArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListModelManifestsRequestRequestTypeDef = TypedDict(
     "ListModelManifestsRequestRequestTypeDef",
     {
         "signalCatalogArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1527,43 +968,19 @@
         "signalCatalogArn": str,
         "description": str,
         "status": ManifestStatusType,
     },
     total=False,
 )
 
-
 class ModelManifestSummaryTypeDef(
     _RequiredModelManifestSummaryTypeDef, _OptionalModelManifestSummaryTypeDef
 ):
     pass
 
-
-_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
-    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListSignalCatalogNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
@@ -1571,30 +988,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListSignalCatalogNodesRequestRequestTypeDef(
     _RequiredListSignalCatalogNodesRequestRequestTypeDef,
     _OptionalListSignalCatalogNodesRequestRequestTypeDef,
 ):
     pass
 
-
-ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSignalCatalogsRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1614,44 +1021,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
-_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "fleetId": str,
-    },
-)
-_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
-    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVehiclesInFleetRequestRequestTypeDef = TypedDict(
     "_RequiredListVehiclesInFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalListVehiclesInFleetRequestRequestTypeDef = TypedDict(
@@ -1659,40 +1036,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListVehiclesInFleetRequestRequestTypeDef(
     _RequiredListVehiclesInFleetRequestRequestTypeDef,
     _OptionalListVehiclesInFleetRequestRequestTypeDef,
 ):
     pass
 
-
-ListVehiclesInFleetResponseTypeDef = TypedDict(
-    "ListVehiclesInFleetResponseTypeDef",
-    {
-        "vehicles": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVehiclesRequestRequestTypeDef = TypedDict(
     "ListVehiclesRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1707,40 +1064,14 @@
         "modelManifestArn": str,
         "decoderManifestArn": str,
         "creationTime": datetime,
         "lastModificationTime": datetime,
     },
 )
 
-_RequiredObdInterfaceOutputTypeDef = TypedDict(
-    "_RequiredObdInterfaceOutputTypeDef",
-    {
-        "name": str,
-        "requestMessageId": int,
-    },
-)
-_OptionalObdInterfaceOutputTypeDef = TypedDict(
-    "_OptionalObdInterfaceOutputTypeDef",
-    {
-        "obdStandard": str,
-        "pidRequestIntervalSeconds": int,
-        "dtcRequestIntervalSeconds": int,
-        "useExtendedIds": bool,
-        "hasTransmissionEcu": bool,
-    },
-    total=False,
-)
-
-
-class ObdInterfaceOutputTypeDef(
-    _RequiredObdInterfaceOutputTypeDef, _OptionalObdInterfaceOutputTypeDef
-):
-    pass
-
-
 _RequiredObdInterfaceTypeDef = TypedDict(
     "_RequiredObdInterfaceTypeDef",
     {
         "name": str,
         "requestMessageId": int,
     },
 )
@@ -1752,19 +1083,17 @@
         "dtcRequestIntervalSeconds": int,
         "useExtendedIds": bool,
         "hasTransmissionEcu": bool,
     },
     total=False,
 )
 
-
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
-
 _RequiredSensorOutputTypeDef = TypedDict(
     "_RequiredSensorOutputTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1778,19 +1107,17 @@
         "max": float,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
     pass
 
-
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1804,45 +1131,17 @@
         "max": float,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
-
 class SensorTypeDef(_RequiredSensorTypeDef, _OptionalSensorTypeDef):
     pass
 
-
-_RequiredObdSignalOutputTypeDef = TypedDict(
-    "_RequiredObdSignalOutputTypeDef",
-    {
-        "pidResponseLength": int,
-        "serviceMode": int,
-        "pid": int,
-        "scaling": float,
-        "offset": float,
-        "startByte": int,
-        "byteLength": int,
-    },
-)
-_OptionalObdSignalOutputTypeDef = TypedDict(
-    "_OptionalObdSignalOutputTypeDef",
-    {
-        "bitRightShift": int,
-        "bitMaskLength": int,
-    },
-    total=False,
-)
-
-
-class ObdSignalOutputTypeDef(_RequiredObdSignalOutputTypeDef, _OptionalObdSignalOutputTypeDef):
-    pass
-
-
 _RequiredObdSignalTypeDef = TypedDict(
     "_RequiredObdSignalTypeDef",
     {
         "pidResponseLength": int,
         "serviceMode": int,
         "pid": int,
         "scaling": float,
@@ -1856,56 +1155,25 @@
     {
         "bitRightShift": int,
         "bitMaskLength": int,
     },
     total=False,
 )
 
-
 class ObdSignalTypeDef(_RequiredObdSignalTypeDef, _OptionalObdSignalTypeDef):
     pass
 
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
 TimestreamResourcesTypeDef = TypedDict(
     "TimestreamResourcesTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
     },
 )
 
-TimestreamResourcesOutputTypeDef = TypedDict(
-    "TimestreamResourcesOutputTypeDef",
-    {
-        "timestreamDatabaseName": str,
-        "timestreamTableName": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1922,70 +1190,38 @@
     {
         "description": str,
         "dataExtraDimensions": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
-
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "status": CampaignStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDecoderManifestResponseTypeDef = TypedDict(
-    "UpdateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalUpdateFleetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFleetRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateFleetRequestRequestTypeDef(
     _RequiredUpdateFleetRequestRequestTypeDef, _OptionalUpdateFleetRequestRequestTypeDef
 ):
     pass
 
-
-UpdateFleetResponseTypeDef = TypedDict(
-    "UpdateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateModelManifestRequestRequestTypeDef = TypedDict(
@@ -1995,79 +1231,303 @@
         "nodesToAdd": Sequence[str],
         "nodesToRemove": Sequence[str],
         "status": ManifestStatusType,
     },
     total=False,
 )
 
-
 class UpdateModelManifestRequestRequestTypeDef(
     _RequiredUpdateModelManifestRequestRequestTypeDef,
     _OptionalUpdateModelManifestRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateVehicleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVehicleRequestRequestTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalUpdateVehicleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVehicleRequestRequestTypeDef",
+    {
+        "modelManifestArn": str,
+        "decoderManifestArn": str,
+        "attributes": Mapping[str, str],
+        "attributeUpdateMode": UpdateModeType,
+    },
+    total=False,
+)
 
-UpdateModelManifestResponseTypeDef = TypedDict(
-    "UpdateModelManifestResponseTypeDef",
+class UpdateVehicleRequestRequestTypeDef(
+    _RequiredUpdateVehicleRequestRequestTypeDef, _OptionalUpdateVehicleRequestRequestTypeDef
+):
+    pass
+
+BatchCreateVehicleResponseTypeDef = TypedDict(
+    "BatchCreateVehicleResponseTypeDef",
+    {
+        "vehicles": List[CreateVehicleResponseItemTypeDef],
+        "errors": List[CreateVehicleErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
     {
         "name": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSignalCatalogResponseTypeDef = TypedDict(
-    "UpdateSignalCatalogResponseTypeDef",
+CreateDecoderManifestResponseTypeDef = TypedDict(
+    "CreateDecoderManifestResponseTypeDef",
     {
         "name": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateVehicleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateVehicleRequestRequestTypeDef",
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelManifestResponseTypeDef = TypedDict(
+    "CreateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSignalCatalogResponseTypeDef = TypedDict(
+    "CreateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVehicleResponseTypeDef = TypedDict(
+    "CreateVehicleResponseTypeDef",
     {
         "vehicleName": str,
+        "arn": str,
+        "thingArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateVehicleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateVehicleRequestRequestTypeDef",
+
+DeleteCampaignResponseTypeDef = TypedDict(
+    "DeleteCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDecoderManifestResponseTypeDef = TypedDict(
+    "DeleteDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFleetResponseTypeDef = TypedDict(
+    "DeleteFleetResponseTypeDef",
     {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteModelManifestResponseTypeDef = TypedDict(
+    "DeleteModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSignalCatalogResponseTypeDef = TypedDict(
+    "DeleteSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVehicleResponseTypeDef = TypedDict(
+    "DeleteVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecoderManifestResponseTypeDef = TypedDict(
+    "GetDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "modelManifestArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFleetResponseTypeDef = TypedDict(
+    "GetFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelManifestResponseTypeDef = TypedDict(
+    "GetModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVehicleResponseTypeDef = TypedDict(
+    "GetVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
-        "attributes": Mapping[str, str],
-        "attributeUpdateMode": UpdateModeType,
+        "attributes": Dict[str, str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ImportDecoderManifestResponseTypeDef = TypedDict(
+    "ImportDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateVehicleRequestRequestTypeDef(
-    _RequiredUpdateVehicleRequestRequestTypeDef, _OptionalUpdateVehicleRequestRequestTypeDef
-):
-    pass
+ImportSignalCatalogResponseTypeDef = TypedDict(
+    "ImportSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFleetsForVehicleResponseTypeDef = TypedDict(
+    "ListFleetsForVehicleResponseTypeDef",
+    {
+        "fleets": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListVehiclesInFleetResponseTypeDef = TypedDict(
+    "ListVehiclesInFleetResponseTypeDef",
+    {
+        "vehicles": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateVehicleResponseTypeDef = TypedDict(
-    "UpdateVehicleResponseTypeDef",
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
     {
-        "vehicleName": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "status": CampaignStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCreateVehicleResponseTypeDef = TypedDict(
-    "BatchCreateVehicleResponseTypeDef",
+UpdateDecoderManifestResponseTypeDef = TypedDict(
+    "UpdateDecoderManifestResponseTypeDef",
     {
-        "vehicles": List[CreateVehicleResponseItemTypeDef],
-        "errors": List[CreateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFleetResponseTypeDef = TypedDict(
+    "UpdateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelManifestResponseTypeDef = TypedDict(
+    "UpdateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSignalCatalogResponseTypeDef = TypedDict(
+    "UpdateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVehicleResponseTypeDef = TypedDict(
+    "UpdateVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateVehicleRequestRequestTypeDef = TypedDict(
     "BatchUpdateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[UpdateVehicleRequestItemTypeDef],
@@ -2075,59 +1535,50 @@
 )
 
 BatchUpdateVehicleResponseTypeDef = TypedDict(
     "BatchUpdateVehicleResponseTypeDef",
     {
         "vehicles": List[UpdateVehicleResponseItemTypeDef],
         "errors": List[UpdateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaries": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFileDefinitionTypeDef = TypedDict(
     "NetworkFileDefinitionTypeDef",
     {
         "canDbc": CanDbcDefinitionTypeDef,
     },
     total=False,
 )
 
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
-        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
     },
 )
 
-CollectionSchemeOutputTypeDef = TypedDict(
-    "CollectionSchemeOutputTypeDef",
-    {
-        "timeBasedCollectionScheme": TimeBasedCollectionSchemeOutputTypeDef,
-        "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeOutputTypeDef,
-    },
-    total=False,
-)
-
 CollectionSchemeTypeDef = TypedDict(
     "CollectionSchemeTypeDef",
     {
         "timeBasedCollectionScheme": TimeBasedCollectionSchemeTypeDef,
         "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeTypeDef,
     },
     total=False,
@@ -2145,21 +1596,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateModelManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelManifestRequestRequestTypeDef",
     {
         "name": str,
         "nodes": Sequence[str],
         "signalCatalogArn": str,
     },
@@ -2169,22 +1618,20 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelManifestRequestRequestTypeDef(
     _RequiredCreateModelManifestRequestRequestTypeDef,
     _OptionalCreateModelManifestRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVehicleRequestItemTypeDef = TypedDict(
     "_RequiredCreateVehicleRequestItemTypeDef",
     {
         "vehicleName": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
     },
@@ -2195,21 +1642,19 @@
         "attributes": Mapping[str, str],
         "associationBehavior": VehicleAssociationBehaviorType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVehicleRequestItemTypeDef(
     _RequiredCreateVehicleRequestItemTypeDef, _OptionalCreateVehicleRequestItemTypeDef
 ):
     pass
 
-
 _RequiredCreateVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
     },
@@ -2220,62 +1665,59 @@
         "attributes": Mapping[str, str],
         "associationBehavior": VehicleAssociationBehaviorType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVehicleRequestRequestTypeDef(
     _RequiredCreateVehicleRequestRequestTypeDef, _OptionalCreateVehicleRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DataDestinationConfigOutputTypeDef = TypedDict(
-    "DataDestinationConfigOutputTypeDef",
-    {
-        "s3Config": S3ConfigOutputTypeDef,
-        "timestreamConfig": TimestreamConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 DataDestinationConfigTypeDef = TypedDict(
     "DataDestinationConfigTypeDef",
     {
         "s3Config": S3ConfigTypeDef,
         "timestreamConfig": TimestreamConfigTypeDef,
     },
     total=False,
 )
 
 ListDecoderManifestsResponseTypeDef = TypedDict(
     "ListDecoderManifestsResponseTypeDef",
     {
         "summaries": List[DecoderManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "fleetSummaries": List[FleetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredImportSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
@@ -2287,114 +1729,273 @@
         "description": str,
         "vss": FormattedVssTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportSignalCatalogRequestRequestTypeDef(
     _RequiredImportSignalCatalogRequestRequestTypeDef,
     _OptionalImportSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
-
 GetRegisterAccountStatusResponseTypeDef = TypedDict(
     "GetRegisterAccountStatusResponseTypeDef",
     {
         "customerAccountId": str,
         "accountStatus": RegistrationStatusType,
         "timestreamRegistrationResponse": TimestreamRegistrationResponseTypeDef,
         "iamRegistrationResponse": IamRegistrationResponseTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSignalCatalogResponseTypeDef = TypedDict(
     "GetSignalCatalogResponseTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "nodeCounts": NodeCountsTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetVehicleStatusResponseTypeDef = TypedDict(
-    "GetVehicleStatusResponseTypeDef",
+_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
     {
-        "campaigns": List[VehicleStatusTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "vehicleName": str,
     },
 )
+_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListModelManifestsResponseTypeDef = TypedDict(
-    "ListModelManifestsResponseTypeDef",
+class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
+    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+):
+    pass
+
+ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
-        "summaries": List[ModelManifestSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListSignalCatalogsResponseTypeDef = TypedDict(
-    "ListSignalCatalogsResponseTypeDef",
+_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     {
-        "summaries": List[SignalCatalogSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
     },
 )
+_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
+    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+):
+    pass
+
+_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListVehiclesResponseTypeDef = TypedDict(
-    "ListVehiclesResponseTypeDef",
+class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
+    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+):
+    pass
+
+ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
     {
-        "vehicleSummaries": List[VehicleSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredNetworkInterfaceOutputTypeDef = TypedDict(
-    "_RequiredNetworkInterfaceOutputTypeDef",
+_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
     {
-        "interfaceId": str,
-        "type": NetworkInterfaceTypeType,
+        "vehicleName": str,
+    },
+)
+_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
+    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+):
+    pass
+
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
+    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+):
+    pass
+
+ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    {
+        "signalCatalogArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalNetworkInterfaceOutputTypeDef = TypedDict(
-    "_OptionalNetworkInterfaceOutputTypeDef",
+
+_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
+    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+):
+    pass
+
+ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     {
-        "canInterface": CanInterfaceOutputTypeDef,
-        "obdInterface": ObdInterfaceOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "fleetId": str,
+    },
+)
+_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class NetworkInterfaceOutputTypeDef(
-    _RequiredNetworkInterfaceOutputTypeDef, _OptionalNetworkInterfaceOutputTypeDef
+class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
+    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
 ):
     pass
 
+ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetVehicleStatusResponseTypeDef = TypedDict(
+    "GetVehicleStatusResponseTypeDef",
+    {
+        "campaigns": List[VehicleStatusTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListModelManifestsResponseTypeDef = TypedDict(
+    "ListModelManifestsResponseTypeDef",
+    {
+        "summaries": List[ModelManifestSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSignalCatalogsResponseTypeDef = TypedDict(
+    "ListSignalCatalogsResponseTypeDef",
+    {
+        "summaries": List[SignalCatalogSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVehiclesResponseTypeDef = TypedDict(
+    "ListVehiclesResponseTypeDef",
+    {
+        "vehicleSummaries": List[VehicleSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredNetworkInterfaceTypeDef = TypedDict(
     "_RequiredNetworkInterfaceTypeDef",
     {
         "interfaceId": str,
         "type": NetworkInterfaceTypeType,
     },
@@ -2404,23 +2005,21 @@
     {
         "canInterface": CanInterfaceTypeDef,
         "obdInterface": ObdInterfaceTypeDef,
     },
     total=False,
 )
 
-
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
-
 NodeOutputTypeDef = TypedDict(
     "NodeOutputTypeDef",
     {
-        "branch": BranchOutputTypeDef,
+        "branch": BranchTypeDef,
         "sensor": SensorOutputTypeDef,
         "actuator": ActuatorOutputTypeDef,
         "attribute": AttributeOutputTypeDef,
     },
     total=False,
 )
 
@@ -2431,38 +2030,14 @@
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
     },
     total=False,
 )
 
-_RequiredSignalDecoderOutputTypeDef = TypedDict(
-    "_RequiredSignalDecoderOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "type": SignalDecoderTypeType,
-        "interfaceId": str,
-    },
-)
-_OptionalSignalDecoderOutputTypeDef = TypedDict(
-    "_OptionalSignalDecoderOutputTypeDef",
-    {
-        "canSignal": CanSignalOutputTypeDef,
-        "obdSignal": ObdSignalOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SignalDecoderOutputTypeDef(
-    _RequiredSignalDecoderOutputTypeDef, _OptionalSignalDecoderOutputTypeDef
-):
-    pass
-
-
 _RequiredSignalDecoderTypeDef = TypedDict(
     "_RequiredSignalDecoderTypeDef",
     {
         "fullyQualifiedName": str,
         "type": SignalDecoderTypeType,
         "interfaceId": str,
     },
@@ -2472,37 +2047,35 @@
     {
         "canSignal": CanSignalTypeDef,
         "obdSignal": ObdSignalTypeDef,
     },
     total=False,
 )
 
-
 class SignalDecoderTypeDef(_RequiredSignalDecoderTypeDef, _OptionalSignalDecoderTypeDef):
     pass
 
-
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "timestreamResources": TimestreamResourcesTypeDef,
         "iamResources": IamResourcesTypeDef,
     },
     total=False,
 )
 
 RegisterAccountResponseTypeDef = TypedDict(
     "RegisterAccountResponseTypeDef",
     {
         "registerAccountStatus": RegistrationStatusType,
-        "timestreamResources": TimestreamResourcesOutputTypeDef,
-        "iamResources": IamResourcesOutputTypeDef,
+        "timestreamResources": TimestreamResourcesTypeDef,
+        "iamResources": IamResourcesTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportDecoderManifestRequestRequestTypeDef = TypedDict(
     "ImportDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
@@ -2513,40 +2086,14 @@
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
 )
 
-GetCampaignResponseTypeDef = TypedDict(
-    "GetCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "targetArn": str,
-        "status": CampaignStatusType,
-        "startTime": datetime,
-        "expiryTime": datetime,
-        "postTriggerCollectionDuration": int,
-        "diagnosticsMode": DiagnosticsModeType,
-        "spoolingMode": SpoolingModeType,
-        "compression": CompressionType,
-        "priority": int,
-        "signalsToCollect": List[SignalInformationOutputTypeDef],
-        "collectionScheme": CollectionSchemeOutputTypeDef,
-        "dataExtraDimensions": List[str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "dataDestinationConfigs": List[DataDestinationConfigOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "name": str,
         "signalCatalogArn": str,
         "targetArn": str,
         "collectionScheme": CollectionSchemeTypeDef,
@@ -2567,45 +2114,69 @@
         "dataExtraDimensions": Sequence[str],
         "tags": Sequence[TagTypeDef],
         "dataDestinationConfigs": Sequence[DataDestinationConfigTypeDef],
     },
     total=False,
 )
 
-
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
+GetCampaignResponseTypeDef = TypedDict(
+    "GetCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "targetArn": str,
+        "status": CampaignStatusType,
+        "startTime": datetime,
+        "expiryTime": datetime,
+        "postTriggerCollectionDuration": int,
+        "diagnosticsMode": DiagnosticsModeType,
+        "spoolingMode": SpoolingModeType,
+        "compression": CompressionType,
+        "priority": int,
+        "signalsToCollect": List[SignalInformationTypeDef],
+        "collectionScheme": CollectionSchemeTypeDef,
+        "dataExtraDimensions": List[str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "dataDestinationConfigs": List[DataDestinationConfigTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     {
-        "networkInterfaces": List[NetworkInterfaceOutputTypeDef],
+        "networkInterfaces": List[NetworkInterfaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelManifestNodesResponseTypeDef = TypedDict(
     "ListModelManifestNodesResponseTypeDef",
     {
         "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogNodesResponseTypeDef = TypedDict(
     "ListSignalCatalogNodesResponseTypeDef",
     {
         "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
@@ -2617,22 +2188,20 @@
         "description": str,
         "nodes": Sequence[NodeTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSignalCatalogRequestRequestTypeDef(
     _RequiredCreateSignalCatalogRequestRequestTypeDef,
     _OptionalCreateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
@@ -2642,31 +2211,20 @@
         "nodesToAdd": Sequence[NodeTypeDef],
         "nodesToUpdate": Sequence[NodeTypeDef],
         "nodesToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateSignalCatalogRequestRequestTypeDef(
     _RequiredUpdateSignalCatalogRequestRequestTypeDef,
     _OptionalUpdateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
-
-ListDecoderManifestSignalsResponseTypeDef = TypedDict(
-    "ListDecoderManifestSignalsResponseTypeDef",
-    {
-        "signalDecoders": List[SignalDecoderOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2677,21 +2235,28 @@
         "signalDecoders": Sequence[SignalDecoderTypeDef],
         "networkInterfaces": Sequence[NetworkInterfaceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDecoderManifestRequestRequestTypeDef(
     _RequiredCreateDecoderManifestRequestRequestTypeDef,
     _OptionalCreateDecoderManifestRequestRequestTypeDef,
 ):
     pass
 
+ListDecoderManifestSignalsResponseTypeDef = TypedDict(
+    "ListDecoderManifestSignalsResponseTypeDef",
+    {
+        "signalDecoders": List[SignalDecoderTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -2706,13 +2271,12 @@
         "networkInterfacesToUpdate": Sequence[NetworkInterfaceTypeDef],
         "networkInterfacesToRemove": Sequence[str],
         "status": ManifestStatusType,
     },
     total=False,
 )
 
-
 class UpdateDecoderManifestRequestRequestTypeDef(
     _RequiredUpdateDecoderManifestRequestRequestTypeDef,
     _OptionalUpdateDecoderManifestRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.pyi` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,185 +38,168 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
     "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
-    "BranchOutputTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
     "CanDbcDefinitionTypeDef",
-    "CanInterfaceOutputTypeDef",
     "CanInterfaceTypeDef",
-    "CanSignalOutputTypeDef",
     "CanSignalTypeDef",
-    "CloudWatchLogDeliveryOptionsOutputTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
-    "ConditionBasedCollectionSchemeOutputTypeDef",
-    "TimeBasedCollectionSchemeOutputTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDecoderManifestResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "CreateModelManifestResponseTypeDef",
-    "CreateSignalCatalogResponseTypeDef",
-    "CreateVehicleResponseTypeDef",
-    "S3ConfigOutputTypeDef",
-    "TimestreamConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
-    "DeleteCampaignResponseTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
-    "DeleteDecoderManifestResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
-    "DeleteFleetResponseTypeDef",
     "DeleteModelManifestRequestRequestTypeDef",
-    "DeleteModelManifestResponseTypeDef",
     "DeleteSignalCatalogRequestRequestTypeDef",
-    "DeleteSignalCatalogResponseTypeDef",
     "DeleteVehicleRequestRequestTypeDef",
-    "DeleteVehicleResponseTypeDef",
     "DisassociateVehicleFleetRequestRequestTypeDef",
     "FleetSummaryTypeDef",
     "FormattedVssTypeDef",
     "GetCampaignRequestRequestTypeDef",
-    "SignalInformationOutputTypeDef",
     "GetDecoderManifestRequestRequestTypeDef",
-    "GetDecoderManifestResponseTypeDef",
     "GetFleetRequestRequestTypeDef",
-    "GetFleetResponseTypeDef",
     "GetModelManifestRequestRequestTypeDef",
-    "GetModelManifestResponseTypeDef",
     "IamRegistrationResponseTypeDef",
     "TimestreamRegistrationResponseTypeDef",
     "GetSignalCatalogRequestRequestTypeDef",
     "NodeCountsTypeDef",
     "GetVehicleRequestRequestTypeDef",
-    "GetVehicleResponseTypeDef",
-    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetVehicleStatusRequestRequestTypeDef",
     "VehicleStatusTypeDef",
-    "IamResourcesOutputTypeDef",
     "IamResourcesTypeDef",
-    "ImportDecoderManifestResponseTypeDef",
-    "ImportSignalCatalogResponseTypeDef",
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
-    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
-    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
     "ListDecoderManifestSignalsRequestRequestTypeDef",
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
     "ListDecoderManifestsRequestRequestTypeDef",
-    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
     "ListFleetsForVehicleRequestRequestTypeDef",
-    "ListFleetsForVehicleResponseTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
     "ListModelManifestNodesRequestRequestTypeDef",
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
     "ListModelManifestsRequestRequestTypeDef",
     "ModelManifestSummaryTypeDef",
-    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     "ListSignalCatalogNodesRequestRequestTypeDef",
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
-    "ListVehiclesInFleetResponseTypeDef",
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
-    "ObdInterfaceOutputTypeDef",
     "ObdInterfaceTypeDef",
     "SensorOutputTypeDef",
     "SensorTypeDef",
-    "ObdSignalOutputTypeDef",
     "ObdSignalTypeDef",
-    "PaginatorConfigTypeDef",
     "TimestreamResourcesTypeDef",
-    "TimestreamResourcesOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
+    "UpdateFleetRequestRequestTypeDef",
+    "UpdateModelManifestRequestRequestTypeDef",
+    "UpdateVehicleRequestRequestTypeDef",
+    "BatchCreateVehicleResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDecoderManifestResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateModelManifestResponseTypeDef",
+    "CreateSignalCatalogResponseTypeDef",
+    "CreateVehicleResponseTypeDef",
+    "DeleteCampaignResponseTypeDef",
+    "DeleteDecoderManifestResponseTypeDef",
+    "DeleteFleetResponseTypeDef",
+    "DeleteModelManifestResponseTypeDef",
+    "DeleteSignalCatalogResponseTypeDef",
+    "DeleteVehicleResponseTypeDef",
+    "GetDecoderManifestResponseTypeDef",
+    "GetFleetResponseTypeDef",
+    "GetModelManifestResponseTypeDef",
+    "GetVehicleResponseTypeDef",
+    "ImportDecoderManifestResponseTypeDef",
+    "ImportSignalCatalogResponseTypeDef",
+    "ListFleetsForVehicleResponseTypeDef",
+    "ListVehiclesInFleetResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDecoderManifestResponseTypeDef",
-    "UpdateFleetRequestRequestTypeDef",
     "UpdateFleetResponseTypeDef",
-    "UpdateModelManifestRequestRequestTypeDef",
     "UpdateModelManifestResponseTypeDef",
     "UpdateSignalCatalogResponseTypeDef",
-    "UpdateVehicleRequestRequestTypeDef",
     "UpdateVehicleResponseTypeDef",
-    "BatchCreateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
-    "CollectionSchemeOutputTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "DataDestinationConfigOutputTypeDef",
     "DataDestinationConfigTypeDef",
     "ListDecoderManifestsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ImportSignalCatalogRequestRequestTypeDef",
     "GetRegisterAccountStatusResponseTypeDef",
     "GetSignalCatalogResponseTypeDef",
+    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVehiclesResponseTypeDef",
-    "NetworkInterfaceOutputTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeOutputTypeDef",
     "NodeTypeDef",
-    "SignalDecoderOutputTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
     "ImportDecoderManifestRequestRequestTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
-    "GetCampaignResponseTypeDef",
     "CreateCampaignRequestRequestTypeDef",
+    "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
     "CreateSignalCatalogRequestRequestTypeDef",
     "UpdateSignalCatalogRequestRequestTypeDef",
-    "ListDecoderManifestSignalsResponseTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
+    "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
 )
 
 _RequiredActuatorOutputTypeDef = TypedDict(
     "_RequiredActuatorOutputTypeDef",
     {
         "fullyQualifiedName": str,
@@ -234,17 +217,19 @@
         "assignedValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
     pass
 
+
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -259,17 +244,19 @@
         "assignedValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class ActuatorTypeDef(_RequiredActuatorTypeDef, _OptionalActuatorTypeDef):
     pass
 
+
 AssociateVehicleFleetRequestRequestTypeDef = TypedDict(
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
@@ -293,17 +280,19 @@
         "defaultValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
     pass
 
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -319,17 +308,19 @@
         "defaultValue": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 CreateVehicleErrorTypeDef = TypedDict(
     "CreateVehicleErrorTypeDef",
     {
         "vehicleName": str,
         "code": str,
         "message": str,
     },
@@ -342,14 +333,25 @@
         "vehicleName": str,
         "arn": str,
         "thingArn": str,
     },
     total=False,
 )
 
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
 _RequiredUpdateVehicleRequestItemTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestItemTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalUpdateVehicleRequestItemTypeDef = TypedDict(
@@ -359,19 +361,21 @@
         "decoderManifestArn": str,
         "attributes": Mapping[str, str],
         "attributeUpdateMode": UpdateModeType,
     },
     total=False,
 )
 
+
 class UpdateVehicleRequestItemTypeDef(
     _RequiredUpdateVehicleRequestItemTypeDef, _OptionalUpdateVehicleRequestItemTypeDef
 ):
     pass
 
+
 UpdateVehicleErrorTypeDef = TypedDict(
     "UpdateVehicleErrorTypeDef",
     {
         "vehicleName": str,
         "code": int,
         "message": str,
     },
@@ -383,33 +387,14 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
-_RequiredBranchOutputTypeDef = TypedDict(
-    "_RequiredBranchOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-    },
-)
-_OptionalBranchOutputTypeDef = TypedDict(
-    "_OptionalBranchOutputTypeDef",
-    {
-        "description": str,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
-)
-
-class BranchOutputTypeDef(_RequiredBranchOutputTypeDef, _OptionalBranchOutputTypeDef):
-    pass
-
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -418,17 +403,19 @@
         "description": str,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class BranchTypeDef(_RequiredBranchTypeDef, _OptionalBranchTypeDef):
     pass
 
+
 _RequiredCampaignSummaryTypeDef = TypedDict(
     "_RequiredCampaignSummaryTypeDef",
     {
         "creationTime": datetime,
         "lastModificationTime": datetime,
     },
 )
@@ -441,17 +428,19 @@
         "signalCatalogArn": str,
         "targetArn": str,
         "status": CampaignStatusType,
     },
     total=False,
 )
 
+
 class CampaignSummaryTypeDef(_RequiredCampaignSummaryTypeDef, _OptionalCampaignSummaryTypeDef):
     pass
 
+
 _RequiredCanDbcDefinitionTypeDef = TypedDict(
     "_RequiredCanDbcDefinitionTypeDef",
     {
         "networkInterface": str,
         "canDbcFiles": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
 )
@@ -459,36 +448,18 @@
     "_OptionalCanDbcDefinitionTypeDef",
     {
         "signalsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
     pass
 
-_RequiredCanInterfaceOutputTypeDef = TypedDict(
-    "_RequiredCanInterfaceOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCanInterfaceOutputTypeDef = TypedDict(
-    "_OptionalCanInterfaceOutputTypeDef",
-    {
-        "protocolName": str,
-        "protocolVersion": str,
-    },
-    total=False,
-)
-
-class CanInterfaceOutputTypeDef(
-    _RequiredCanInterfaceOutputTypeDef, _OptionalCanInterfaceOutputTypeDef
-):
-    pass
 
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
@@ -497,39 +468,18 @@
     {
         "protocolName": str,
         "protocolVersion": str,
     },
     total=False,
 )
 
+
 class CanInterfaceTypeDef(_RequiredCanInterfaceTypeDef, _OptionalCanInterfaceTypeDef):
     pass
 
-_RequiredCanSignalOutputTypeDef = TypedDict(
-    "_RequiredCanSignalOutputTypeDef",
-    {
-        "messageId": int,
-        "isBigEndian": bool,
-        "isSigned": bool,
-        "startBit": int,
-        "offset": float,
-        "factor": float,
-        "length": int,
-    },
-)
-_OptionalCanSignalOutputTypeDef = TypedDict(
-    "_OptionalCanSignalOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-class CanSignalOutputTypeDef(_RequiredCanSignalOutputTypeDef, _OptionalCanSignalOutputTypeDef):
-    pass
 
 _RequiredCanSignalTypeDef = TypedDict(
     "_RequiredCanSignalTypeDef",
     {
         "messageId": int,
         "isBigEndian": bool,
         "isSigned": bool,
@@ -543,36 +493,18 @@
     "_OptionalCanSignalTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
+
 class CanSignalTypeDef(_RequiredCanSignalTypeDef, _OptionalCanSignalTypeDef):
     pass
 
-_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef",
-    {
-        "logType": LogTypeType,
-    },
-)
-_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef",
-    {
-        "logGroupName": str,
-    },
-    total=False,
-)
-
-class CloudWatchLogDeliveryOptionsOutputTypeDef(
-    _RequiredCloudWatchLogDeliveryOptionsOutputTypeDef,
-    _OptionalCloudWatchLogDeliveryOptionsOutputTypeDef,
-):
-    pass
 
 _RequiredCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
     "_RequiredCloudWatchLogDeliveryOptionsTypeDef",
     {
         "logType": LogTypeType,
     },
 )
@@ -580,47 +512,20 @@
     "_OptionalCloudWatchLogDeliveryOptionsTypeDef",
     {
         "logGroupName": str,
     },
     total=False,
 )
 
+
 class CloudWatchLogDeliveryOptionsTypeDef(
     _RequiredCloudWatchLogDeliveryOptionsTypeDef, _OptionalCloudWatchLogDeliveryOptionsTypeDef
 ):
     pass
 
-_RequiredConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
-    "_RequiredConditionBasedCollectionSchemeOutputTypeDef",
-    {
-        "expression": str,
-    },
-)
-_OptionalConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
-    "_OptionalConditionBasedCollectionSchemeOutputTypeDef",
-    {
-        "minimumTriggerIntervalMs": int,
-        "triggerMode": TriggerModeType,
-        "conditionLanguageVersion": int,
-    },
-    total=False,
-)
-
-class ConditionBasedCollectionSchemeOutputTypeDef(
-    _RequiredConditionBasedCollectionSchemeOutputTypeDef,
-    _OptionalConditionBasedCollectionSchemeOutputTypeDef,
-):
-    pass
-
-TimeBasedCollectionSchemeOutputTypeDef = TypedDict(
-    "TimeBasedCollectionSchemeOutputTypeDef",
-    {
-        "periodMs": int,
-    },
-)
 
 _RequiredConditionBasedCollectionSchemeTypeDef = TypedDict(
     "_RequiredConditionBasedCollectionSchemeTypeDef",
     {
         "expression": str,
     },
 )
@@ -630,19 +535,21 @@
         "minimumTriggerIntervalMs": int,
         "triggerMode": TriggerModeType,
         "conditionLanguageVersion": int,
     },
     total=False,
 )
 
+
 class ConditionBasedCollectionSchemeTypeDef(
     _RequiredConditionBasedCollectionSchemeTypeDef, _OptionalConditionBasedCollectionSchemeTypeDef
 ):
     pass
 
+
 TimeBasedCollectionSchemeTypeDef = TypedDict(
     "TimeBasedCollectionSchemeTypeDef",
     {
         "periodMs": int,
     },
 )
 
@@ -657,109 +564,29 @@
     {
         "maxSampleCount": int,
         "minimumSamplingIntervalMs": int,
     },
     total=False,
 )
 
+
 class SignalInformationTypeDef(
     _RequiredSignalInformationTypeDef, _OptionalSignalInformationTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDecoderManifestResponseTypeDef = TypedDict(
-    "CreateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateModelManifestResponseTypeDef = TypedDict(
-    "CreateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSignalCatalogResponseTypeDef = TypedDict(
-    "CreateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVehicleResponseTypeDef = TypedDict(
-    "CreateVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "thingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3ConfigOutputTypeDef = TypedDict(
-    "_RequiredS3ConfigOutputTypeDef",
-    {
-        "bucketArn": str,
-    },
-)
-_OptionalS3ConfigOutputTypeDef = TypedDict(
-    "_OptionalS3ConfigOutputTypeDef",
-    {
-        "dataFormat": DataFormatType,
-        "storageCompressionFormat": StorageCompressionFormatType,
-        "prefix": str,
-    },
-    total=False,
-)
-
-class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
-    pass
-
-TimestreamConfigOutputTypeDef = TypedDict(
-    "TimestreamConfigOutputTypeDef",
-    {
-        "timestreamTableArn": str,
-        "executionRoleArn": str,
-    },
-)
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -768,17 +595,19 @@
         "dataFormat": DataFormatType,
         "storageCompressionFormat": StorageCompressionFormatType,
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
+
 TimestreamConfigTypeDef = TypedDict(
     "TimestreamConfigTypeDef",
     {
         "timestreamTableArn": str,
         "executionRoleArn": str,
     },
 )
@@ -798,115 +627,63 @@
         "modelManifestArn": str,
         "description": str,
         "status": ManifestStatusType,
     },
     total=False,
 )
 
+
 class DecoderManifestSummaryTypeDef(
     _RequiredDecoderManifestSummaryTypeDef, _OptionalDecoderManifestSummaryTypeDef
 ):
     pass
 
+
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteCampaignResponseTypeDef = TypedDict(
-    "DeleteCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDecoderManifestRequestRequestTypeDef = TypedDict(
     "DeleteDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteDecoderManifestResponseTypeDef = TypedDict(
-    "DeleteDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-DeleteFleetResponseTypeDef = TypedDict(
-    "DeleteFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteModelManifestRequestRequestTypeDef = TypedDict(
     "DeleteModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteModelManifestResponseTypeDef = TypedDict(
-    "DeleteModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSignalCatalogRequestRequestTypeDef = TypedDict(
     "DeleteSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteSignalCatalogResponseTypeDef = TypedDict(
-    "DeleteSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVehicleRequestRequestTypeDef = TypedDict(
     "DeleteVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-DeleteVehicleResponseTypeDef = TypedDict(
-    "DeleteVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateVehicleFleetRequestRequestTypeDef = TypedDict(
     "DisassociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
@@ -925,17 +702,19 @@
     {
         "description": str,
         "lastModificationTime": datetime,
     },
     total=False,
 )
 
+
 class FleetSummaryTypeDef(_RequiredFleetSummaryTypeDef, _OptionalFleetSummaryTypeDef):
     pass
 
+
 FormattedVssTypeDef = TypedDict(
     "FormattedVssTypeDef",
     {
         "vssJson": str,
     },
     total=False,
 )
@@ -943,96 +722,35 @@
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredSignalInformationOutputTypeDef = TypedDict(
-    "_RequiredSignalInformationOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalSignalInformationOutputTypeDef = TypedDict(
-    "_OptionalSignalInformationOutputTypeDef",
-    {
-        "maxSampleCount": int,
-        "minimumSamplingIntervalMs": int,
-    },
-    total=False,
-)
-
-class SignalInformationOutputTypeDef(
-    _RequiredSignalInformationOutputTypeDef, _OptionalSignalInformationOutputTypeDef
-):
-    pass
-
 GetDecoderManifestRequestRequestTypeDef = TypedDict(
     "GetDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetDecoderManifestResponseTypeDef = TypedDict(
-    "GetDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "modelManifestArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFleetRequestRequestTypeDef = TypedDict(
     "GetFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-GetFleetResponseTypeDef = TypedDict(
-    "GetFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelManifestRequestRequestTypeDef = TypedDict(
     "GetModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetModelManifestResponseTypeDef = TypedDict(
-    "GetModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIamRegistrationResponseTypeDef = TypedDict(
     "_RequiredIamRegistrationResponseTypeDef",
     {
         "roleArn": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1040,19 +758,21 @@
     "_OptionalIamRegistrationResponseTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
+
 class IamRegistrationResponseTypeDef(
     _RequiredIamRegistrationResponseTypeDef, _OptionalIamRegistrationResponseTypeDef
 ):
     pass
 
+
 _RequiredTimestreamRegistrationResponseTypeDef = TypedDict(
     "_RequiredTimestreamRegistrationResponseTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
         "registrationStatus": RegistrationStatusType,
     },
@@ -1063,19 +783,21 @@
         "timestreamDatabaseArn": str,
         "timestreamTableArn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
+
 class TimestreamRegistrationResponseTypeDef(
     _RequiredTimestreamRegistrationResponseTypeDef, _OptionalTimestreamRegistrationResponseTypeDef
 ):
     pass
 
+
 GetSignalCatalogRequestRequestTypeDef = TypedDict(
     "GetSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -1094,48 +816,24 @@
 GetVehicleRequestRequestTypeDef = TypedDict(
     "GetVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-GetVehicleResponseTypeDef = TypedDict(
-    "GetVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "modelManifestArn": str,
-        "decoderManifestArn": str,
-        "attributes": Dict[str, str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
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
 
-class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
-    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredGetVehicleStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetVehicleStatusRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalGetVehicleStatusRequestRequestTypeDef = TypedDict(
@@ -1143,100 +841,48 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetVehicleStatusRequestRequestTypeDef(
     _RequiredGetVehicleStatusRequestRequestTypeDef, _OptionalGetVehicleStatusRequestRequestTypeDef
 ):
     pass
 
+
 VehicleStatusTypeDef = TypedDict(
     "VehicleStatusTypeDef",
     {
         "campaignName": str,
         "vehicleName": str,
         "status": VehicleStateType,
     },
     total=False,
 )
 
-IamResourcesOutputTypeDef = TypedDict(
-    "IamResourcesOutputTypeDef",
-    {
-        "roleArn": str,
-    },
-)
-
 IamResourcesTypeDef = TypedDict(
     "IamResourcesTypeDef",
     {
         "roleArn": str,
     },
 )
 
-ImportDecoderManifestResponseTypeDef = TypedDict(
-    "ImportDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportSignalCatalogResponseTypeDef = TypedDict(
-    "ImportSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    {
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": str,
     },
     total=False,
 )
 
-_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
-    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
@@ -1244,39 +890,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListDecoderManifestNetworkInterfacesRequestRequestTypeDef(
     _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
     _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
-    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-):
-    pass
 
 _RequiredListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestSignalsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -1285,59 +913,32 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListDecoderManifestSignalsRequestRequestTypeDef(
     _RequiredListDecoderManifestSignalsRequestRequestTypeDef,
     _OptionalListDecoderManifestSignalsRequestRequestTypeDef,
 ):
     pass
 
-ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDecoderManifestsRequestRequestTypeDef = TypedDict(
     "ListDecoderManifestsRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
-    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-):
-    pass
-
 _RequiredListFleetsForVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredListFleetsForVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalListFleetsForVehicleRequestRequestTypeDef = TypedDict(
@@ -1345,66 +946,31 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListFleetsForVehicleRequestRequestTypeDef(
     _RequiredListFleetsForVehicleRequestRequestTypeDef,
     _OptionalListFleetsForVehicleRequestRequestTypeDef,
 ):
     pass
 
-ListFleetsForVehicleResponseTypeDef = TypedDict(
-    "ListFleetsForVehicleResponseTypeDef",
-    {
-        "fleets": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListFleetsRequestRequestTypeDef = TypedDict(
     "ListFleetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
-    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-):
-    pass
-
 _RequiredListModelManifestNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListModelManifestNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListModelManifestNodesRequestRequestTypeDef = TypedDict(
@@ -1412,28 +978,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListModelManifestNodesRequestRequestTypeDef(
     _RequiredListModelManifestNodesRequestRequestTypeDef,
     _OptionalListModelManifestNodesRequestRequestTypeDef,
 ):
     pass
 
-ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
-    {
-        "signalCatalogArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListModelManifestsRequestRequestTypeDef = TypedDict(
     "ListModelManifestsRequestRequestTypeDef",
     {
         "signalCatalogArn": str,
         "nextToken": str,
         "maxResults": int,
@@ -1456,38 +1015,20 @@
         "signalCatalogArn": str,
         "description": str,
         "status": ManifestStatusType,
     },
     total=False,
 )
 
+
 class ModelManifestSummaryTypeDef(
     _RequiredModelManifestSummaryTypeDef, _OptionalModelManifestSummaryTypeDef
 ):
     pass
 
-_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
-    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-):
-    pass
 
 _RequiredListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListSignalCatalogNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -1496,27 +1037,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListSignalCatalogNodesRequestRequestTypeDef(
     _RequiredListSignalCatalogNodesRequestRequestTypeDef,
     _OptionalListSignalCatalogNodesRequestRequestTypeDef,
 ):
     pass
 
-ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListSignalCatalogsRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
@@ -1537,42 +1072,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
-_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "fleetId": str,
-    },
-)
-_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
-    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-):
-    pass
-
 _RequiredListVehiclesInFleetRequestRequestTypeDef = TypedDict(
     "_RequiredListVehiclesInFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalListVehiclesInFleetRequestRequestTypeDef = TypedDict(
@@ -1580,37 +1087,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListVehiclesInFleetRequestRequestTypeDef(
     _RequiredListVehiclesInFleetRequestRequestTypeDef,
     _OptionalListVehiclesInFleetRequestRequestTypeDef,
 ):
     pass
 
-ListVehiclesInFleetResponseTypeDef = TypedDict(
-    "ListVehiclesInFleetResponseTypeDef",
-    {
-        "vehicles": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListVehiclesRequestRequestTypeDef = TypedDict(
     "ListVehiclesRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
@@ -1626,38 +1117,14 @@
         "modelManifestArn": str,
         "decoderManifestArn": str,
         "creationTime": datetime,
         "lastModificationTime": datetime,
     },
 )
 
-_RequiredObdInterfaceOutputTypeDef = TypedDict(
-    "_RequiredObdInterfaceOutputTypeDef",
-    {
-        "name": str,
-        "requestMessageId": int,
-    },
-)
-_OptionalObdInterfaceOutputTypeDef = TypedDict(
-    "_OptionalObdInterfaceOutputTypeDef",
-    {
-        "obdStandard": str,
-        "pidRequestIntervalSeconds": int,
-        "dtcRequestIntervalSeconds": int,
-        "useExtendedIds": bool,
-        "hasTransmissionEcu": bool,
-    },
-    total=False,
-)
-
-class ObdInterfaceOutputTypeDef(
-    _RequiredObdInterfaceOutputTypeDef, _OptionalObdInterfaceOutputTypeDef
-):
-    pass
-
 _RequiredObdInterfaceTypeDef = TypedDict(
     "_RequiredObdInterfaceTypeDef",
     {
         "name": str,
         "requestMessageId": int,
     },
 )
@@ -1669,17 +1136,19 @@
         "dtcRequestIntervalSeconds": int,
         "useExtendedIds": bool,
         "hasTransmissionEcu": bool,
     },
     total=False,
 )
 
+
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
+
 _RequiredSensorOutputTypeDef = TypedDict(
     "_RequiredSensorOutputTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1693,17 +1162,19 @@
         "max": float,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
     pass
 
+
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1717,40 +1188,18 @@
         "max": float,
         "deprecationMessage": str,
         "comment": str,
     },
     total=False,
 )
 
+
 class SensorTypeDef(_RequiredSensorTypeDef, _OptionalSensorTypeDef):
     pass
 
-_RequiredObdSignalOutputTypeDef = TypedDict(
-    "_RequiredObdSignalOutputTypeDef",
-    {
-        "pidResponseLength": int,
-        "serviceMode": int,
-        "pid": int,
-        "scaling": float,
-        "offset": float,
-        "startByte": int,
-        "byteLength": int,
-    },
-)
-_OptionalObdSignalOutputTypeDef = TypedDict(
-    "_OptionalObdSignalOutputTypeDef",
-    {
-        "bitRightShift": int,
-        "bitMaskLength": int,
-    },
-    total=False,
-)
-
-class ObdSignalOutputTypeDef(_RequiredObdSignalOutputTypeDef, _OptionalObdSignalOutputTypeDef):
-    pass
 
 _RequiredObdSignalTypeDef = TypedDict(
     "_RequiredObdSignalTypeDef",
     {
         "pidResponseLength": int,
         "serviceMode": int,
         "pid": int,
@@ -1765,54 +1214,27 @@
     {
         "bitRightShift": int,
         "bitMaskLength": int,
     },
     total=False,
 )
 
+
 class ObdSignalTypeDef(_RequiredObdSignalTypeDef, _OptionalObdSignalTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
 
 TimestreamResourcesTypeDef = TypedDict(
     "TimestreamResourcesTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
     },
 )
 
-TimestreamResourcesOutputTypeDef = TypedDict(
-    "TimestreamResourcesOutputTypeDef",
-    {
-        "timestreamDatabaseName": str,
-        "timestreamTableName": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1829,37 +1251,20 @@
     {
         "description": str,
         "dataExtraDimensions": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "status": CampaignStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDecoderManifestResponseTypeDef = TypedDict(
-    "UpdateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
@@ -1867,27 +1272,20 @@
     "_OptionalUpdateFleetRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateFleetRequestRequestTypeDef(
     _RequiredUpdateFleetRequestRequestTypeDef, _OptionalUpdateFleetRequestRequestTypeDef
 ):
     pass
 
-UpdateFleetResponseTypeDef = TypedDict(
-    "UpdateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateModelManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -1898,37 +1296,21 @@
         "nodesToAdd": Sequence[str],
         "nodesToRemove": Sequence[str],
         "status": ManifestStatusType,
     },
     total=False,
 )
 
+
 class UpdateModelManifestRequestRequestTypeDef(
     _RequiredUpdateModelManifestRequestRequestTypeDef,
     _OptionalUpdateModelManifestRequestRequestTypeDef,
 ):
     pass
 
-UpdateModelManifestResponseTypeDef = TypedDict(
-    "UpdateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSignalCatalogResponseTypeDef = TypedDict(
-    "UpdateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
@@ -1939,34 +1321,282 @@
         "decoderManifestArn": str,
         "attributes": Mapping[str, str],
         "attributeUpdateMode": UpdateModeType,
     },
     total=False,
 )
 
+
 class UpdateVehicleRequestRequestTypeDef(
     _RequiredUpdateVehicleRequestRequestTypeDef, _OptionalUpdateVehicleRequestRequestTypeDef
 ):
     pass
 
-UpdateVehicleResponseTypeDef = TypedDict(
-    "UpdateVehicleResponseTypeDef",
+
+BatchCreateVehicleResponseTypeDef = TypedDict(
+    "BatchCreateVehicleResponseTypeDef",
+    {
+        "vehicles": List[CreateVehicleResponseItemTypeDef],
+        "errors": List[CreateVehicleErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDecoderManifestResponseTypeDef = TypedDict(
+    "CreateDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelManifestResponseTypeDef = TypedDict(
+    "CreateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSignalCatalogResponseTypeDef = TypedDict(
+    "CreateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVehicleResponseTypeDef = TypedDict(
+    "CreateVehicleResponseTypeDef",
     {
         "vehicleName": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "thingArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCreateVehicleResponseTypeDef = TypedDict(
-    "BatchCreateVehicleResponseTypeDef",
+DeleteCampaignResponseTypeDef = TypedDict(
+    "DeleteCampaignResponseTypeDef",
     {
-        "vehicles": List[CreateVehicleResponseItemTypeDef],
-        "errors": List[CreateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDecoderManifestResponseTypeDef = TypedDict(
+    "DeleteDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFleetResponseTypeDef = TypedDict(
+    "DeleteFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteModelManifestResponseTypeDef = TypedDict(
+    "DeleteModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSignalCatalogResponseTypeDef = TypedDict(
+    "DeleteSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVehicleResponseTypeDef = TypedDict(
+    "DeleteVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecoderManifestResponseTypeDef = TypedDict(
+    "GetDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "modelManifestArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFleetResponseTypeDef = TypedDict(
+    "GetFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelManifestResponseTypeDef = TypedDict(
+    "GetModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVehicleResponseTypeDef = TypedDict(
+    "GetVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "modelManifestArn": str,
+        "decoderManifestArn": str,
+        "attributes": Dict[str, str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportDecoderManifestResponseTypeDef = TypedDict(
+    "ImportDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSignalCatalogResponseTypeDef = TypedDict(
+    "ImportSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFleetsForVehicleResponseTypeDef = TypedDict(
+    "ListFleetsForVehicleResponseTypeDef",
+    {
+        "fleets": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVehiclesInFleetResponseTypeDef = TypedDict(
+    "ListVehiclesInFleetResponseTypeDef",
+    {
+        "vehicles": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "status": CampaignStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDecoderManifestResponseTypeDef = TypedDict(
+    "UpdateDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFleetResponseTypeDef = TypedDict(
+    "UpdateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelManifestResponseTypeDef = TypedDict(
+    "UpdateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSignalCatalogResponseTypeDef = TypedDict(
+    "UpdateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVehicleResponseTypeDef = TypedDict(
+    "UpdateVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateVehicleRequestRequestTypeDef = TypedDict(
     "BatchUpdateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[UpdateVehicleRequestItemTypeDef],
@@ -1974,59 +1604,50 @@
 )
 
 BatchUpdateVehicleResponseTypeDef = TypedDict(
     "BatchUpdateVehicleResponseTypeDef",
     {
         "vehicles": List[UpdateVehicleResponseItemTypeDef],
         "errors": List[UpdateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaries": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFileDefinitionTypeDef = TypedDict(
     "NetworkFileDefinitionTypeDef",
     {
         "canDbc": CanDbcDefinitionTypeDef,
     },
     total=False,
 )
 
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
-        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
     },
 )
 
-CollectionSchemeOutputTypeDef = TypedDict(
-    "CollectionSchemeOutputTypeDef",
-    {
-        "timeBasedCollectionScheme": TimeBasedCollectionSchemeOutputTypeDef,
-        "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeOutputTypeDef,
-    },
-    total=False,
-)
-
 CollectionSchemeTypeDef = TypedDict(
     "CollectionSchemeTypeDef",
     {
         "timeBasedCollectionScheme": TimeBasedCollectionSchemeTypeDef,
         "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeTypeDef,
     },
     total=False,
@@ -2044,19 +1665,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateModelManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelManifestRequestRequestTypeDef",
     {
         "name": str,
         "nodes": Sequence[str],
         "signalCatalogArn": str,
     },
@@ -2066,20 +1689,22 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelManifestRequestRequestTypeDef(
     _RequiredCreateModelManifestRequestRequestTypeDef,
     _OptionalCreateModelManifestRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVehicleRequestItemTypeDef = TypedDict(
     "_RequiredCreateVehicleRequestItemTypeDef",
     {
         "vehicleName": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
     },
@@ -2090,19 +1715,21 @@
         "attributes": Mapping[str, str],
         "associationBehavior": VehicleAssociationBehaviorType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVehicleRequestItemTypeDef(
     _RequiredCreateVehicleRequestItemTypeDef, _OptionalCreateVehicleRequestItemTypeDef
 ):
     pass
 
+
 _RequiredCreateVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
     },
@@ -2113,34 +1740,35 @@
         "attributes": Mapping[str, str],
         "associationBehavior": VehicleAssociationBehaviorType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVehicleRequestRequestTypeDef(
     _RequiredCreateVehicleRequestRequestTypeDef, _OptionalCreateVehicleRequestRequestTypeDef
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataDestinationConfigOutputTypeDef = TypedDict(
-    "DataDestinationConfigOutputTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "s3Config": S3ConfigOutputTypeDef,
-        "timestreamConfig": TimestreamConfigOutputTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
 DataDestinationConfigTypeDef = TypedDict(
     "DataDestinationConfigTypeDef",
     {
         "s3Config": S3ConfigTypeDef,
         "timestreamConfig": TimestreamConfigTypeDef,
@@ -2149,24 +1777,24 @@
 )
 
 ListDecoderManifestsResponseTypeDef = TypedDict(
     "ListDecoderManifestsResponseTypeDef",
     {
         "summaries": List[DecoderManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "fleetSummaries": List[FleetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredImportSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
@@ -2178,110 +1806,289 @@
         "description": str,
         "vss": FormattedVssTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportSignalCatalogRequestRequestTypeDef(
     _RequiredImportSignalCatalogRequestRequestTypeDef,
     _OptionalImportSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
+
 GetRegisterAccountStatusResponseTypeDef = TypedDict(
     "GetRegisterAccountStatusResponseTypeDef",
     {
         "customerAccountId": str,
         "accountStatus": RegistrationStatusType,
         "timestreamRegistrationResponse": TimestreamRegistrationResponseTypeDef,
         "iamRegistrationResponse": IamRegistrationResponseTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSignalCatalogResponseTypeDef = TypedDict(
     "GetSignalCatalogResponseTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "nodeCounts": NodeCountsTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
+    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+):
+    pass
+
+
+ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    {
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
+    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
+    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+):
+    pass
+
+
+ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
+    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+):
+    pass
+
+
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
+    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+):
+    pass
+
+
+ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    {
+        "signalCatalogArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
+    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+):
+    pass
+
+
+ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "fleetId": str,
+    },
+)
+_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
+    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+):
+    pass
+
+
+ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 GetVehicleStatusResponseTypeDef = TypedDict(
     "GetVehicleStatusResponseTypeDef",
     {
         "campaigns": List[VehicleStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelManifestsResponseTypeDef = TypedDict(
     "ListModelManifestsResponseTypeDef",
     {
         "summaries": List[ModelManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogsResponseTypeDef = TypedDict(
     "ListSignalCatalogsResponseTypeDef",
     {
         "summaries": List[SignalCatalogSummaryTypeDef],
         "nextToken": str,
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
 
 ListVehiclesResponseTypeDef = TypedDict(
     "ListVehiclesResponseTypeDef",
     {
         "vehicleSummaries": List[VehicleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredNetworkInterfaceOutputTypeDef = TypedDict(
-    "_RequiredNetworkInterfaceOutputTypeDef",
-    {
-        "interfaceId": str,
-        "type": NetworkInterfaceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalNetworkInterfaceOutputTypeDef = TypedDict(
-    "_OptionalNetworkInterfaceOutputTypeDef",
-    {
-        "canInterface": CanInterfaceOutputTypeDef,
-        "obdInterface": ObdInterfaceOutputTypeDef,
-    },
-    total=False,
-)
-
-class NetworkInterfaceOutputTypeDef(
-    _RequiredNetworkInterfaceOutputTypeDef, _OptionalNetworkInterfaceOutputTypeDef
-):
-    pass
 
 _RequiredNetworkInterfaceTypeDef = TypedDict(
     "_RequiredNetworkInterfaceTypeDef",
     {
         "interfaceId": str,
         "type": NetworkInterfaceTypeType,
     },
@@ -2291,21 +2098,23 @@
     {
         "canInterface": CanInterfaceTypeDef,
         "obdInterface": ObdInterfaceTypeDef,
     },
     total=False,
 )
 
+
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
+
 NodeOutputTypeDef = TypedDict(
     "NodeOutputTypeDef",
     {
-        "branch": BranchOutputTypeDef,
+        "branch": BranchTypeDef,
         "sensor": SensorOutputTypeDef,
         "actuator": ActuatorOutputTypeDef,
         "attribute": AttributeOutputTypeDef,
     },
     total=False,
 )
 
@@ -2316,36 +2125,14 @@
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
     },
     total=False,
 )
 
-_RequiredSignalDecoderOutputTypeDef = TypedDict(
-    "_RequiredSignalDecoderOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "type": SignalDecoderTypeType,
-        "interfaceId": str,
-    },
-)
-_OptionalSignalDecoderOutputTypeDef = TypedDict(
-    "_OptionalSignalDecoderOutputTypeDef",
-    {
-        "canSignal": CanSignalOutputTypeDef,
-        "obdSignal": ObdSignalOutputTypeDef,
-    },
-    total=False,
-)
-
-class SignalDecoderOutputTypeDef(
-    _RequiredSignalDecoderOutputTypeDef, _OptionalSignalDecoderOutputTypeDef
-):
-    pass
-
 _RequiredSignalDecoderTypeDef = TypedDict(
     "_RequiredSignalDecoderTypeDef",
     {
         "fullyQualifiedName": str,
         "type": SignalDecoderTypeType,
         "interfaceId": str,
     },
@@ -2355,35 +2142,37 @@
     {
         "canSignal": CanSignalTypeDef,
         "obdSignal": ObdSignalTypeDef,
     },
     total=False,
 )
 
+
 class SignalDecoderTypeDef(_RequiredSignalDecoderTypeDef, _OptionalSignalDecoderTypeDef):
     pass
 
+
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "timestreamResources": TimestreamResourcesTypeDef,
         "iamResources": IamResourcesTypeDef,
     },
     total=False,
 )
 
 RegisterAccountResponseTypeDef = TypedDict(
     "RegisterAccountResponseTypeDef",
     {
         "registerAccountStatus": RegistrationStatusType,
-        "timestreamResources": TimestreamResourcesOutputTypeDef,
-        "iamResources": IamResourcesOutputTypeDef,
+        "timestreamResources": TimestreamResourcesTypeDef,
+        "iamResources": IamResourcesTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportDecoderManifestRequestRequestTypeDef = TypedDict(
     "ImportDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
@@ -2394,40 +2183,14 @@
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
 )
 
-GetCampaignResponseTypeDef = TypedDict(
-    "GetCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "targetArn": str,
-        "status": CampaignStatusType,
-        "startTime": datetime,
-        "expiryTime": datetime,
-        "postTriggerCollectionDuration": int,
-        "diagnosticsMode": DiagnosticsModeType,
-        "spoolingMode": SpoolingModeType,
-        "compression": CompressionType,
-        "priority": int,
-        "signalsToCollect": List[SignalInformationOutputTypeDef],
-        "collectionScheme": CollectionSchemeOutputTypeDef,
-        "dataExtraDimensions": List[str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "dataDestinationConfigs": List[DataDestinationConfigOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "name": str,
         "signalCatalogArn": str,
         "targetArn": str,
         "collectionScheme": CollectionSchemeTypeDef,
@@ -2448,43 +2211,71 @@
         "dataExtraDimensions": Sequence[str],
         "tags": Sequence[TagTypeDef],
         "dataDestinationConfigs": Sequence[DataDestinationConfigTypeDef],
     },
     total=False,
 )
 
+
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
+
+GetCampaignResponseTypeDef = TypedDict(
+    "GetCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "targetArn": str,
+        "status": CampaignStatusType,
+        "startTime": datetime,
+        "expiryTime": datetime,
+        "postTriggerCollectionDuration": int,
+        "diagnosticsMode": DiagnosticsModeType,
+        "spoolingMode": SpoolingModeType,
+        "compression": CompressionType,
+        "priority": int,
+        "signalsToCollect": List[SignalInformationTypeDef],
+        "collectionScheme": CollectionSchemeTypeDef,
+        "dataExtraDimensions": List[str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "dataDestinationConfigs": List[DataDestinationConfigTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     {
-        "networkInterfaces": List[NetworkInterfaceOutputTypeDef],
+        "networkInterfaces": List[NetworkInterfaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelManifestNodesResponseTypeDef = TypedDict(
     "ListModelManifestNodesResponseTypeDef",
     {
         "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogNodesResponseTypeDef = TypedDict(
     "ListSignalCatalogNodesResponseTypeDef",
     {
         "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
@@ -2496,20 +2287,22 @@
         "description": str,
         "nodes": Sequence[NodeTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSignalCatalogRequestRequestTypeDef(
     _RequiredCreateSignalCatalogRequestRequestTypeDef,
     _OptionalCreateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
@@ -2519,28 +2312,21 @@
         "nodesToAdd": Sequence[NodeTypeDef],
         "nodesToUpdate": Sequence[NodeTypeDef],
         "nodesToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateSignalCatalogRequestRequestTypeDef(
     _RequiredUpdateSignalCatalogRequestRequestTypeDef,
     _OptionalUpdateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
-ListDecoderManifestSignalsResponseTypeDef = TypedDict(
-    "ListDecoderManifestSignalsResponseTypeDef",
-    {
-        "signalDecoders": List[SignalDecoderOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
@@ -2552,20 +2338,31 @@
         "signalDecoders": Sequence[SignalDecoderTypeDef],
         "networkInterfaces": Sequence[NetworkInterfaceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDecoderManifestRequestRequestTypeDef(
     _RequiredCreateDecoderManifestRequestRequestTypeDef,
     _OptionalCreateDecoderManifestRequestRequestTypeDef,
 ):
     pass
 
+
+ListDecoderManifestSignalsResponseTypeDef = TypedDict(
+    "ListDecoderManifestSignalsResponseTypeDef",
+    {
+        "signalDecoders": List[SignalDecoderTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
@@ -2579,12 +2376,13 @@
         "networkInterfacesToUpdate": Sequence[NetworkInterfaceTypeDef],
         "networkInterfacesToRemove": Sequence[str],
         "status": ManifestStatusType,
     },
     total=False,
 )
 
+
 class UpdateDecoderManifestRequestRequestTypeDef(
     _RequiredUpdateDecoderManifestRequestRequestTypeDef,
     _OptionalUpdateDecoderManifestRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.15/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iotfleetwise
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTFleetWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotfleetwise"></a>
 
 # mypy-boto3-iotfleetwise
 
 [![PyPI - mypy-boto3-iotfleetwise](https://img.shields.io/pypi/v/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,177 +367,159 @@
     ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
     AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
+    ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
-    BranchOutputTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
     CanDbcDefinitionTypeDef,
-    CanInterfaceOutputTypeDef,
     CanInterfaceTypeDef,
-    CanSignalOutputTypeDef,
     CanSignalTypeDef,
-    CloudWatchLogDeliveryOptionsOutputTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
-    ConditionBasedCollectionSchemeOutputTypeDef,
-    TimeBasedCollectionSchemeOutputTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDecoderManifestResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateModelManifestResponseTypeDef,
-    CreateSignalCatalogResponseTypeDef,
-    CreateVehicleResponseTypeDef,
-    S3ConfigOutputTypeDef,
-    TimestreamConfigOutputTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
-    DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
-    DeleteDecoderManifestResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
-    DeleteFleetResponseTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
-    DeleteModelManifestResponseTypeDef,
     DeleteSignalCatalogRequestRequestTypeDef,
-    DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
-    DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
-    SignalInformationOutputTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
-    GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
-    GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
-    GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
     TimestreamRegistrationResponseTypeDef,
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
-    GetVehicleResponseTypeDef,
-    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
-    IamResourcesOutputTypeDef,
     IamResourcesTypeDef,
-    ImportDecoderManifestResponseTypeDef,
-    ImportSignalCatalogResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
-    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
-    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
     ListDecoderManifestSignalsRequestRequestTypeDef,
-    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
     ListDecoderManifestsRequestRequestTypeDef,
-    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
     ListFleetsForVehicleRequestRequestTypeDef,
-    ListFleetsForVehicleResponseTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
     ListModelManifestNodesRequestRequestTypeDef,
-    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
     ListModelManifestsRequestRequestTypeDef,
     ModelManifestSummaryTypeDef,
-    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
-    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
-    ListVehiclesInFleetResponseTypeDef,
-    ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
-    ObdInterfaceOutputTypeDef,
     ObdInterfaceTypeDef,
     SensorOutputTypeDef,
     SensorTypeDef,
-    ObdSignalOutputTypeDef,
     ObdSignalTypeDef,
-    PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
-    TimestreamResourcesOutputTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    UpdateFleetRequestRequestTypeDef,
+    UpdateModelManifestRequestRequestTypeDef,
+    UpdateVehicleRequestRequestTypeDef,
+    BatchCreateVehicleResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDecoderManifestResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateModelManifestResponseTypeDef,
+    CreateSignalCatalogResponseTypeDef,
+    CreateVehicleResponseTypeDef,
+    DeleteCampaignResponseTypeDef,
+    DeleteDecoderManifestResponseTypeDef,
+    DeleteFleetResponseTypeDef,
+    DeleteModelManifestResponseTypeDef,
+    DeleteSignalCatalogResponseTypeDef,
+    DeleteVehicleResponseTypeDef,
+    GetDecoderManifestResponseTypeDef,
+    GetFleetResponseTypeDef,
+    GetModelManifestResponseTypeDef,
+    GetVehicleResponseTypeDef,
+    ImportDecoderManifestResponseTypeDef,
+    ImportSignalCatalogResponseTypeDef,
+    ListFleetsForVehicleResponseTypeDef,
+    ListVehiclesInFleetResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
-    UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
-    UpdateModelManifestRequestRequestTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
-    UpdateVehicleRequestRequestTypeDef,
     UpdateVehicleResponseTypeDef,
-    BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
     ListCampaignsResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    CollectionSchemeOutputTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    DataDestinationConfigOutputTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
+    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
+    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
+    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
+    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
+    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    ListVehiclesRequestListVehiclesPaginateTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVehiclesResponseTypeDef,
-    NetworkInterfaceOutputTypeDef,
     NetworkInterfaceTypeDef,
     NodeOutputTypeDef,
     NodeTypeDef,
-    SignalDecoderOutputTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
     ImportDecoderManifestRequestRequestTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
-    GetCampaignResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
+    GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
     CreateSignalCatalogRequestRequestTypeDef,
     UpdateSignalCatalogRequestRequestTypeDef,
-    ListDecoderManifestSignalsResponseTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
+    ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ActuatorOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt` & `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.12/setup.py` & `mypy-boto3-iotfleetwise-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleetwise",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetWise 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

