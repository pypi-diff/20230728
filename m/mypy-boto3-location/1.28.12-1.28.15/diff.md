# Comparing `tmp/mypy-boto3-location-1.28.12.tar.gz` & `tmp/mypy-boto3-location-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
```

## Comparing `mypy-boto3-location-1.28.12.tar` & `mypy-boto3-location-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45468 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66915 2023-07-27 05:25:32.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66800 2023-07-27 05:25:32.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.021416 mypy-boto3-location-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-07-28 20:43:11.013415 mypy-boto3-location-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.013415 mypy-boto3-location-1.28.15/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45468 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65922 2023-07-28 20:30:27.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65809 2023-07-28 20:30:26.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.013415 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.021416 mypy-boto3-location-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:30:24.000000 mypy-boto3-location-1.28.15/setup.py
```

### Comparing `mypy-boto3-location-1.28.12/LICENSE` & `mypy-boto3-location-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/PKG-INFO` & `mypy-boto3-location-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.12
-Summary: Type annotations for boto3.LocationService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,143 +373,140 @@
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
-    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
-    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
-    CreateTrackerResponseTypeDef,
-    DataSourceConfigurationOutputTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
-    MapConfigurationOutputTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
-    DescribeTrackerResponseTypeDef,
-    PositionalAccuracyOutputTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
-    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
-    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
-    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
     MapConfigurationUpdateTypeDef,
-    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
-    PutGeofenceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
-    UpdateTrackerResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
+    CreateMapResponseTypeDef,
+    CreatePlaceIndexResponseTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
+    CreateTrackerResponseTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
+    DescribeKeyResponseTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
+    DescribeTrackerResponseTypeDef,
+    GetMapGlyphsResponseTypeDef,
+    GetMapSpritesResponseTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
+    GetMapTileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    PutGeofenceResponseTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
+    UpdateTrackerResponseTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
+    DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
-    UpdatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
-    DescribeMapResponseTypeDef,
+    UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
+    DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
-    DevicePositionUpdateTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -526,17 +523,17 @@
     CalculateRouteRequestRequestTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
-    ListDevicePositionsResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
+    ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
     ListGeofencesResponseTypeDef,
     BatchPutGeofenceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-location-1.28.12/README.md` & `mypy-boto3-location-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,143 +341,140 @@
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
-    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
-    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
-    CreateTrackerResponseTypeDef,
-    DataSourceConfigurationOutputTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
-    MapConfigurationOutputTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
-    DescribeTrackerResponseTypeDef,
-    PositionalAccuracyOutputTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
-    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
-    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
-    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
     MapConfigurationUpdateTypeDef,
-    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
-    PutGeofenceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
-    UpdateTrackerResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
+    CreateMapResponseTypeDef,
+    CreatePlaceIndexResponseTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
+    CreateTrackerResponseTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
+    DescribeKeyResponseTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
+    DescribeTrackerResponseTypeDef,
+    GetMapGlyphsResponseTypeDef,
+    GetMapSpritesResponseTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
+    GetMapTileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    PutGeofenceResponseTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
+    UpdateTrackerResponseTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
+    DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
-    UpdatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
-    DescribeMapResponseTypeDef,
+    UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
+    DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
-    DevicePositionUpdateTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -494,17 +491,17 @@
     CalculateRouteRequestRequestTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
-    ListDevicePositionsResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
+    ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
     ListGeofencesResponseTypeDef,
     BatchPutGeofenceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.28.15/mypy_boto3_location/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LocationService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/client.py` & `mypy-boto3-location-1.28.15/mypy_boto3_location/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.28.15/mypy_boto3_location/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.28.15/mypy_boto3_location/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.28.15/mypy_boto3_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,172 +66,160 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
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
 class GetDevicePositionHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: Union[datetime, str] = ...,
         StartTimeInclusive: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
         """
 
-
 class ListDevicePositionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
         """
 
-
 class ListGeofenceCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeofenceCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
         """
 
-
 class ListGeofencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
     """
 
     def paginate(
-        self, *, CollectionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeofencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
         """
 
-
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
         """
 
-
 class ListMapsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMapsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
         """
 
-
 class ListPlaceIndexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlaceIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
         """
 
-
 class ListRouteCalculatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRouteCalculatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
         """
 
-
 class ListTrackerConsumersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrackerConsumersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
         """
 
-
 class ListTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
         """
```

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,160 +66,172 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
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
 class GetDevicePositionHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: Union[datetime, str] = ...,
         StartTimeInclusive: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
         """
 
+
 class ListDevicePositionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
         """
 
+
 class ListGeofenceCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeofenceCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
         """
 
+
 class ListGeofencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
     """
 
     def paginate(
-        self, *, CollectionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeofencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
         """
 
+
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
         """
 
+
 class ListMapsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMapsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
         """
 
+
 class ListPlaceIndexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlaceIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
         """
 
+
 class ListRouteCalculatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRouteCalculatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
         """
 
+
 class ListTrackerConsumersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrackerConsumersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
         """
 
+
 class ListTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
         """
```

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,143 +39,140 @@
 __all__ = (
     "ApiKeyFilterTypeDef",
     "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
     "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
-    "CreateGeofenceCollectionResponseTypeDef",
-    "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
-    "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
-    "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
-    "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
-    "CreateTrackerResponseTypeDef",
-    "DataSourceConfigurationOutputTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
-    "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
-    "MapConfigurationOutputTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
-    "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
-    "DescribeTrackerResponseTypeDef",
-    "PositionalAccuracyOutputTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
-    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
-    "GetMapGlyphsResponseTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
-    "GetMapSpritesResponseTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
-    "GetMapStyleDescriptorResponseTypeDef",
     "GetMapTileRequestRequestTypeDef",
-    "GetMapTileResponseTypeDef",
     "GetPlaceRequestRequestTypeDef",
     "LegGeometryTypeDef",
     "StepTypeDef",
-    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
     "ListDevicePositionsRequestRequestTypeDef",
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
     "ListGeofenceCollectionsRequestRequestTypeDef",
     "ListGeofenceCollectionsResponseEntryTypeDef",
-    "ListGeofencesRequestListGeofencesPaginateTypeDef",
     "ListGeofencesRequestRequestTypeDef",
-    "ListMapsRequestListMapsPaginateTypeDef",
     "ListMapsRequestRequestTypeDef",
     "ListMapsResponseEntryTypeDef",
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
     "ListPlaceIndexesRequestRequestTypeDef",
     "ListPlaceIndexesResponseEntryTypeDef",
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
     "ListRouteCalculatorsRequestRequestTypeDef",
     "ListRouteCalculatorsResponseEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
     "ListTrackerConsumersRequestRequestTypeDef",
-    "ListTrackerConsumersResponseTypeDef",
-    "ListTrackersRequestListTrackersPaginateTypeDef",
     "ListTrackersRequestRequestTypeDef",
     "ListTrackersResponseEntryTypeDef",
     "MapConfigurationUpdateTypeDef",
-    "PaginatorConfigTypeDef",
     "PlaceGeometryTypeDef",
     "TimeZoneTypeDef",
-    "PutGeofenceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteMatrixEntryErrorTypeDef",
     "SearchForSuggestionsResultTypeDef",
     "SearchPlaceIndexForPositionRequestRequestTypeDef",
     "SearchPlaceIndexForPositionSummaryTypeDef",
     "SearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     "SearchPlaceIndexForSuggestionsSummaryTypeDef",
     "SearchPlaceIndexForTextRequestRequestTypeDef",
     "SearchPlaceIndexForTextSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
-    "UpdateGeofenceCollectionResponseTypeDef",
-    "UpdateKeyResponseTypeDef",
-    "UpdateMapResponseTypeDef",
-    "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
-    "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
-    "UpdateTrackerResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
+    "CreateGeofenceCollectionResponseTypeDef",
+    "CreateKeyResponseTypeDef",
+    "CreateMapResponseTypeDef",
+    "CreatePlaceIndexResponseTypeDef",
+    "CreateRouteCalculatorResponseTypeDef",
+    "CreateTrackerResponseTypeDef",
+    "DescribeGeofenceCollectionResponseTypeDef",
+    "DescribeKeyResponseTypeDef",
+    "DescribeRouteCalculatorResponseTypeDef",
+    "DescribeTrackerResponseTypeDef",
+    "GetMapGlyphsResponseTypeDef",
+    "GetMapSpritesResponseTypeDef",
+    "GetMapStyleDescriptorResponseTypeDef",
+    "GetMapTileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTrackerConsumersResponseTypeDef",
+    "PutGeofenceResponseTypeDef",
+    "UpdateGeofenceCollectionResponseTypeDef",
+    "UpdateKeyResponseTypeDef",
+    "UpdateMapResponseTypeDef",
+    "UpdatePlaceIndexResponseTypeDef",
+    "UpdateRouteCalculatorResponseTypeDef",
+    "UpdateTrackerResponseTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
     "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
+    "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
-    "UpdatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
-    "DescribeMapResponseTypeDef",
+    "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
+    "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
-    "DevicePositionUpdateTypeDef",
+    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    "ListGeofencesRequestListGeofencesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListMapsRequestListMapsPaginateTypeDef",
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    "ListTrackersRequestListTrackersPaginateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
     "UpdateMapRequestRequestTypeDef",
@@ -192,17 +189,17 @@
     "CalculateRouteRequestRequestTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
     "BatchPutGeofenceRequestEntryTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
-    "ListDevicePositionsResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
+    "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
     "ListGeofencesResponseTypeDef",
     "BatchPutGeofenceRequestRequestTypeDef",
@@ -283,14 +280,25 @@
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
         "TrackerName": str,
     },
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
 BatchDeleteGeofenceRequestRequestTypeDef = TypedDict(
     "BatchDeleteGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceIds": Sequence[str],
     },
 )
@@ -400,35 +408,14 @@
 class CreateGeofenceCollectionRequestRequestTypeDef(
     _RequiredCreateGeofenceCollectionRequestRequestTypeDef,
     _OptionalCreateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateGeofenceCollectionResponseTypeDef = TypedDict(
-    "CreateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateKeyResponseTypeDef = TypedDict(
-    "CreateKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapConfigurationTypeDef = TypedDict(
     "_RequiredMapConfigurationTypeDef",
     {
         "Style": str,
     },
 )
 _OptionalMapConfigurationTypeDef = TypedDict(
@@ -440,42 +427,22 @@
 )
 
 
 class MapConfigurationTypeDef(_RequiredMapConfigurationTypeDef, _OptionalMapConfigurationTypeDef):
     pass
 
 
-CreateMapResponseTypeDef = TypedDict(
-    "CreateMapResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "MapArn": str,
-        "MapName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "IntendedUse": IntendedUseType,
     },
     total=False,
 )
 
-CreatePlaceIndexResponseTypeDef = TypedDict(
-    "CreatePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "IndexArn": str,
-        "IndexName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
         "DataSource": str,
     },
 )
@@ -493,24 +460,14 @@
 class CreateRouteCalculatorRequestRequestTypeDef(
     _RequiredCreateRouteCalculatorRequestRequestTypeDef,
     _OptionalCreateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
 
-CreateRouteCalculatorResponseTypeDef = TypedDict(
-    "CreateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
@@ -530,32 +487,14 @@
 
 class CreateTrackerRequestRequestTypeDef(
     _RequiredCreateTrackerRequestRequestTypeDef, _OptionalCreateTrackerRequestRequestTypeDef
 ):
     pass
 
 
-CreateTrackerResponseTypeDef = TypedDict(
-    "CreateTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "TrackerArn": str,
-        "TrackerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataSourceConfigurationOutputTypeDef = TypedDict(
-    "DataSourceConfigurationOutputTypeDef",
-    {
-        "IntendedUse": IntendedUseType,
-    },
-    total=False,
-)
-
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -597,126 +536,49 @@
 DescribeGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
-DescribeGeofenceCollectionResponseTypeDef = TypedDict(
-    "DescribeGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeKeyRequestRequestTypeDef = TypedDict(
     "DescribeKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 
 DescribeMapRequestRequestTypeDef = TypedDict(
     "DescribeMapRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 
-_RequiredMapConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMapConfigurationOutputTypeDef",
-    {
-        "Style": str,
-    },
-)
-_OptionalMapConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMapConfigurationOutputTypeDef",
-    {
-        "PoliticalView": str,
-    },
-    total=False,
-)
-
-
-class MapConfigurationOutputTypeDef(
-    _RequiredMapConfigurationOutputTypeDef, _OptionalMapConfigurationOutputTypeDef
-):
-    pass
-
-
 DescribePlaceIndexRequestRequestTypeDef = TypedDict(
     "DescribePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 
 DescribeRouteCalculatorRequestRequestTypeDef = TypedDict(
     "DescribeRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 
-DescribeRouteCalculatorResponseTypeDef = TypedDict(
-    "DescribeRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTrackerRequestRequestTypeDef = TypedDict(
     "DescribeTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 
-DescribeTrackerResponseTypeDef = TypedDict(
-    "DescribeTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "EventBridgeEnabled": bool,
-        "KmsKeyId": str,
-        "PositionFiltering": PositionFilteringType,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PositionalAccuracyOutputTypeDef = TypedDict(
-    "PositionalAccuracyOutputTypeDef",
-    {
-        "Horizontal": float,
-    },
-)
-
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -724,39 +586,24 @@
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     {
         "ConsumerArn": str,
         "TrackerName": str,
     },
 )
 
-_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
-    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -814,24 +661,14 @@
 
 class GetMapGlyphsRequestRequestTypeDef(
     _RequiredGetMapGlyphsRequestRequestTypeDef, _OptionalGetMapGlyphsRequestRequestTypeDef
 ):
     pass
 
 
-GetMapGlyphsResponseTypeDef = TypedDict(
-    "GetMapGlyphsResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapSpritesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapSpritesRequestRequestTypeDef",
     {
         "FileName": str,
         "MapName": str,
     },
 )
@@ -846,24 +683,14 @@
 
 class GetMapSpritesRequestRequestTypeDef(
     _RequiredGetMapSpritesRequestRequestTypeDef, _OptionalGetMapSpritesRequestRequestTypeDef
 ):
     pass
 
 
-GetMapSpritesResponseTypeDef = TypedDict(
-    "GetMapSpritesResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapStyleDescriptorRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 _OptionalGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
@@ -878,24 +705,14 @@
 class GetMapStyleDescriptorRequestRequestTypeDef(
     _RequiredGetMapStyleDescriptorRequestRequestTypeDef,
     _OptionalGetMapStyleDescriptorRequestRequestTypeDef,
 ):
     pass
 
 
-GetMapStyleDescriptorResponseTypeDef = TypedDict(
-    "GetMapStyleDescriptorResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapTileRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapTileRequestRequestTypeDef",
     {
         "MapName": str,
         "X": str,
         "Y": str,
         "Z": str,
@@ -912,24 +729,14 @@
 
 class GetMapTileRequestRequestTypeDef(
     _RequiredGetMapTileRequestRequestTypeDef, _OptionalGetMapTileRequestRequestTypeDef
 ):
     pass
 
 
-GetMapTileResponseTypeDef = TypedDict(
-    "GetMapTileResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPlaceRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlaceRequestRequestTypeDef",
     {
         "IndexName": str,
         "PlaceId": str,
     },
 )
@@ -975,36 +782,14 @@
 )
 
 
 class StepTypeDef(_RequiredStepTypeDef, _OptionalStepTypeDef):
     pass
 
 
-_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
-    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDevicePositionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePositionsRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListDevicePositionsRequestRequestTypeDef = TypedDict(
@@ -1020,22 +805,14 @@
 class ListDevicePositionsRequestRequestTypeDef(
     _RequiredListDevicePositionsRequestRequestTypeDef,
     _OptionalListDevicePositionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeofenceCollectionsRequestRequestTypeDef = TypedDict(
     "ListGeofenceCollectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1063,36 +840,14 @@
 class ListGeofenceCollectionsResponseEntryTypeDef(
     _RequiredListGeofenceCollectionsResponseEntryTypeDef,
     _OptionalListGeofenceCollectionsResponseEntryTypeDef,
 ):
     pass
 
 
-_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "CollectionName": str,
-    },
-)
-_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGeofencesRequestListGeofencesPaginateTypeDef(
-    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
-    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGeofencesRequestRequestTypeDef = TypedDict(
     "_RequiredListGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 _OptionalListGeofencesRequestRequestTypeDef = TypedDict(
@@ -1107,22 +862,14 @@
 
 class ListGeofencesRequestRequestTypeDef(
     _RequiredListGeofencesRequestRequestTypeDef, _OptionalListGeofencesRequestRequestTypeDef
 ):
     pass
 
 
-ListMapsRequestListMapsPaginateTypeDef = TypedDict(
-    "ListMapsRequestListMapsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMapsRequestRequestTypeDef = TypedDict(
     "ListMapsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1149,22 +896,14 @@
 
 class ListMapsResponseEntryTypeDef(
     _RequiredListMapsResponseEntryTypeDef, _OptionalListMapsResponseEntryTypeDef
 ):
     pass
 
 
-ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaceIndexesRequestRequestTypeDef = TypedDict(
     "ListPlaceIndexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1191,22 +930,14 @@
 
 class ListPlaceIndexesResponseEntryTypeDef(
     _RequiredListPlaceIndexesResponseEntryTypeDef, _OptionalListPlaceIndexesResponseEntryTypeDef
 ):
     pass
 
 
-ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRouteCalculatorsRequestRequestTypeDef = TypedDict(
     "ListRouteCalculatorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1241,44 +972,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
-    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTrackerConsumersRequestRequestTypeDef = TypedDict(
     "_RequiredListTrackerConsumersRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListTrackerConsumersRequestRequestTypeDef = TypedDict(
@@ -1294,31 +995,14 @@
 class ListTrackerConsumersRequestRequestTypeDef(
     _RequiredListTrackerConsumersRequestRequestTypeDef,
     _OptionalListTrackerConsumersRequestRequestTypeDef,
 ):
     pass
 
 
-ListTrackerConsumersResponseTypeDef = TypedDict(
-    "ListTrackerConsumersResponseTypeDef",
-    {
-        "ConsumerArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
-    "ListTrackersRequestListTrackersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrackersRequestRequestTypeDef = TypedDict(
     "ListTrackersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1353,24 +1037,14 @@
     "MapConfigurationUpdateTypeDef",
     {
         "PoliticalView": str,
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
 PlaceGeometryTypeDef = TypedDict(
     "PlaceGeometryTypeDef",
     {
         "Point": List[float],
     },
     total=False,
 )
@@ -1390,35 +1064,14 @@
 )
 
 
 class TimeZoneTypeDef(_RequiredTimeZoneTypeDef, _OptionalTimeZoneTypeDef):
     pass
 
 
-PutGeofenceResponseTypeDef = TypedDict(
-    "PutGeofenceResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "GeofenceId": str,
-        "UpdateTime": datetime,
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
 _RequiredRouteMatrixEntryErrorTypeDef = TypedDict(
     "_RequiredRouteMatrixEntryErrorTypeDef",
     {
         "Code": RouteMatrixErrorCodeType,
     },
 )
 _OptionalRouteMatrixEntryErrorTypeDef = TypedDict(
@@ -1658,54 +1311,14 @@
 class UpdateGeofenceCollectionRequestRequestTypeDef(
     _RequiredUpdateGeofenceCollectionRequestRequestTypeDef,
     _OptionalUpdateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateGeofenceCollectionResponseTypeDef = TypedDict(
-    "UpdateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateKeyResponseTypeDef = TypedDict(
-    "UpdateKeyResponseTypeDef",
-    {
-        "KeyArn": str,
-        "KeyName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMapResponseTypeDef = TypedDict(
-    "UpdateMapResponseTypeDef",
-    {
-        "MapArn": str,
-        "MapName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePlaceIndexResponseTypeDef = TypedDict(
-    "UpdatePlaceIndexResponseTypeDef",
-    {
-        "IndexArn": str,
-        "IndexName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 _OptionalUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
@@ -1721,24 +1334,14 @@
 class UpdateRouteCalculatorRequestRequestTypeDef(
     _RequiredUpdateRouteCalculatorRequestRequestTypeDef,
     _OptionalUpdateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateRouteCalculatorResponseTypeDef = TypedDict(
-    "UpdateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
@@ -1756,59 +1359,24 @@
 
 class UpdateTrackerRequestRequestTypeDef(
     _RequiredUpdateTrackerRequestRequestTypeDef, _OptionalUpdateTrackerRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTrackerResponseTypeDef = TypedDict(
-    "UpdateTrackerResponseTypeDef",
-    {
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "Filter": ApiKeyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeKeyResponseTypeDef = TypedDict(
-    "DescribeKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "ExpireTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
         "Restrictions": ApiKeyRestrictionsOutputTypeDef,
@@ -1926,14 +1494,267 @@
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
         "SampleTime": datetime,
     },
 )
 
+CreateGeofenceCollectionResponseTypeDef = TypedDict(
+    "CreateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKeyResponseTypeDef = TypedDict(
+    "CreateKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMapResponseTypeDef = TypedDict(
+    "CreateMapResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "MapArn": str,
+        "MapName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePlaceIndexResponseTypeDef = TypedDict(
+    "CreatePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRouteCalculatorResponseTypeDef = TypedDict(
+    "CreateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrackerResponseTypeDef = TypedDict(
+    "CreateTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGeofenceCollectionResponseTypeDef = TypedDict(
+    "DescribeGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeKeyResponseTypeDef = TypedDict(
+    "DescribeKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "ExpireTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRouteCalculatorResponseTypeDef = TypedDict(
+    "DescribeRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTrackerResponseTypeDef = TypedDict(
+    "DescribeTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "EventBridgeEnabled": bool,
+        "KmsKeyId": str,
+        "PositionFiltering": PositionFilteringType,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapGlyphsResponseTypeDef = TypedDict(
+    "GetMapGlyphsResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapSpritesResponseTypeDef = TypedDict(
+    "GetMapSpritesResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapStyleDescriptorResponseTypeDef = TypedDict(
+    "GetMapStyleDescriptorResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapTileResponseTypeDef = TypedDict(
+    "GetMapTileResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTrackerConsumersResponseTypeDef = TypedDict(
+    "ListTrackerConsumersResponseTypeDef",
+    {
+        "ConsumerArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutGeofenceResponseTypeDef = TypedDict(
+    "PutGeofenceResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "GeofenceId": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGeofenceCollectionResponseTypeDef = TypedDict(
+    "UpdateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKeyResponseTypeDef = TypedDict(
+    "UpdateKeyResponseTypeDef",
+    {
+        "KeyArn": str,
+        "KeyName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMapResponseTypeDef = TypedDict(
+    "UpdateMapResponseTypeDef",
+    {
+        "MapArn": str,
+        "MapName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePlaceIndexResponseTypeDef = TypedDict(
+    "UpdatePlaceIndexResponseTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRouteCalculatorResponseTypeDef = TypedDict(
+    "UpdateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrackerResponseTypeDef = TypedDict(
+    "UpdateTrackerResponseTypeDef",
+    {
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
@@ -1979,14 +1800,30 @@
 
 class CreateMapRequestRequestTypeDef(
     _RequiredCreateMapRequestRequestTypeDef, _OptionalCreateMapRequestRequestTypeDef
 ):
     pass
 
 
+DescribeMapResponseTypeDef = TypedDict(
+    "DescribeMapResponseTypeDef",
+    {
+        "Configuration": MapConfigurationTypeDef,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "MapArn": str,
+        "MapName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
         "IndexName": str,
     },
 )
@@ -2004,14 +1841,30 @@
 
 class CreatePlaceIndexRequestRequestTypeDef(
     _RequiredCreatePlaceIndexRequestRequestTypeDef, _OptionalCreatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
 
+DescribePlaceIndexResponseTypeDef = TypedDict(
+    "DescribePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "DataSource": str,
+        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
+        "Description": str,
+        "IndexArn": str,
+        "IndexName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
@@ -2027,131 +1880,239 @@
 
 class UpdatePlaceIndexRequestRequestTypeDef(
     _RequiredUpdatePlaceIndexRequestRequestTypeDef, _OptionalUpdatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
 
-DescribePlaceIndexResponseTypeDef = TypedDict(
-    "DescribePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "DataSource": str,
-        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
-        "Description": str,
-        "IndexArn": str,
-        "IndexName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMapResponseTypeDef = TypedDict(
-    "DescribeMapResponseTypeDef",
-    {
-        "Configuration": MapConfigurationOutputTypeDef,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "MapArn": str,
-        "MapName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDevicePositionTypeDef = TypedDict(
     "_RequiredDevicePositionTypeDef",
     {
         "Position": List[float],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
     },
 )
 _OptionalDevicePositionTypeDef = TypedDict(
     "_OptionalDevicePositionTypeDef",
     {
-        "Accuracy": PositionalAccuracyOutputTypeDef,
+        "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 
 class DevicePositionTypeDef(_RequiredDevicePositionTypeDef, _OptionalDevicePositionTypeDef):
     pass
 
 
+_RequiredDevicePositionUpdateTypeDef = TypedDict(
+    "_RequiredDevicePositionUpdateTypeDef",
+    {
+        "DeviceId": str,
+        "Position": Sequence[float],
+        "SampleTime": Union[datetime, str],
+    },
+)
+_OptionalDevicePositionUpdateTypeDef = TypedDict(
+    "_OptionalDevicePositionUpdateTypeDef",
+    {
+        "Accuracy": PositionalAccuracyTypeDef,
+        "PositionProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class DevicePositionUpdateTypeDef(
+    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
+):
+    pass
+
+
 GetDevicePositionResponseTypeDef = TypedDict(
     "GetDevicePositionResponseTypeDef",
     {
-        "Accuracy": PositionalAccuracyOutputTypeDef,
+        "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_RequiredListDevicePositionsResponseEntryTypeDef",
     {
         "DeviceId": str,
         "Position": List[float],
         "SampleTime": datetime,
     },
 )
 _OptionalListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_OptionalListDevicePositionsResponseEntryTypeDef",
     {
-        "Accuracy": PositionalAccuracyOutputTypeDef,
+        "Accuracy": PositionalAccuracyTypeDef,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
 
-_RequiredDevicePositionUpdateTypeDef = TypedDict(
-    "_RequiredDevicePositionUpdateTypeDef",
+_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
         "DeviceId": str,
-        "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
+        "TrackerName": str,
     },
 )
-_OptionalDevicePositionUpdateTypeDef = TypedDict(
-    "_OptionalDevicePositionUpdateTypeDef",
+_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
-        "PositionProperties": Mapping[str, str],
+        "EndTimeExclusive": Union[datetime, str],
+        "StartTimeInclusive": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DevicePositionUpdateTypeDef(
-    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
+class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
+    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
+    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+):
+    pass
+
+
+ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "CollectionName": str,
+    },
+)
+_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGeofencesRequestListGeofencesPaginateTypeDef(
+    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
+    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
 ):
     pass
 
 
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "Filter": ApiKeyFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMapsRequestListMapsPaginateTypeDef = TypedDict(
+    "ListMapsRequestListMapsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
+    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+):
+    pass
+
+
+ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
+    "ListTrackersRequestListTrackersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -2172,51 +2133,51 @@
 
 
 ListGeofenceCollectionsResponseTypeDef = TypedDict(
     "ListGeofenceCollectionsResponseTypeDef",
     {
         "Entries": List[ListGeofenceCollectionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMapsResponseTypeDef = TypedDict(
     "ListMapsResponseTypeDef",
     {
         "Entries": List[ListMapsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlaceIndexesResponseTypeDef = TypedDict(
     "ListPlaceIndexesResponseTypeDef",
     {
         "Entries": List[ListPlaceIndexesResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRouteCalculatorsResponseTypeDef = TypedDict(
     "ListRouteCalculatorsResponseTypeDef",
     {
         "Entries": List[ListRouteCalculatorsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrackersResponseTypeDef = TypedDict(
     "ListTrackersResponseTypeDef",
     {
         "Entries": List[ListTrackersResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMapRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMapRequestRequestTypeDef",
     {
         "MapName": str,
@@ -2283,65 +2244,65 @@
 )
 
 SearchPlaceIndexForSuggestionsResponseTypeDef = TypedDict(
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     {
         "Results": List[SearchForSuggestionsResultTypeDef],
         "Summary": SearchPlaceIndexForSuggestionsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Entries": List[ListKeysResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDevicePositionHistoryResponseTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     {
         "Errors": List[BatchDeleteDevicePositionHistoryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteGeofenceResponseTypeDef = TypedDict(
     "BatchDeleteGeofenceResponseTypeDef",
     {
         "Errors": List[BatchDeleteGeofenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesResponseTypeDef = TypedDict(
     "BatchEvaluateGeofencesResponseTypeDef",
     {
         "Errors": List[BatchEvaluateGeofencesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutGeofenceResponseTypeDef = TypedDict(
     "BatchPutGeofenceResponseTypeDef",
     {
         "Errors": List[BatchPutGeofenceErrorTypeDef],
         "Successes": List[BatchPutGeofenceSuccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateDevicePositionResponseTypeDef = TypedDict(
     "BatchUpdateDevicePositionResponseTypeDef",
     {
         "Errors": List[BatchUpdateDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_RequiredCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CalculatorName": str,
@@ -2407,15 +2368,15 @@
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
         "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
@@ -2486,33 +2447,24 @@
 
 
 BatchGetDevicePositionResponseTypeDef = TypedDict(
     "BatchGetDevicePositionResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "Errors": List[BatchGetDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDevicePositionHistoryResponseTypeDef = TypedDict(
     "GetDevicePositionHistoryResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevicePositionsResponseTypeDef = TypedDict(
-    "ListDevicePositionsResponseTypeDef",
-    {
-        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2524,28 +2476,37 @@
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     {
         "TrackerName": str,
         "Updates": Sequence[DevicePositionUpdateTypeDef],
     },
 )
 
+ListDevicePositionsResponseTypeDef = TypedDict(
+    "ListDevicePositionsResponseTypeDef",
+    {
+        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPlaceResponseTypeDef = TypedDict(
     "GetPlaceResponseTypeDef",
     {
         "Place": PlaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchForPositionResultTypeDef = TypedDict(
     "_RequiredSearchForPositionResultTypeDef",
     {
         "Distance": float,
@@ -2593,24 +2554,24 @@
 CalculateRouteMatrixResponseTypeDef = TypedDict(
     "CalculateRouteMatrixResponseTypeDef",
     {
         "RouteMatrix": List[List[RouteMatrixEntryTypeDef]],
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutGeofenceRequestRequestTypeDef = TypedDict(
     "BatchPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2619,19 +2580,19 @@
 )
 
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchPlaceIndexForTextResponseTypeDef = TypedDict(
     "SearchPlaceIndexForTextResponseTypeDef",
     {
         "Results": List[SearchForTextResultTypeDef],
         "Summary": SearchPlaceIndexForTextSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,143 +38,140 @@
 __all__ = (
     "ApiKeyFilterTypeDef",
     "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
     "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
-    "CreateGeofenceCollectionResponseTypeDef",
-    "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
-    "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
-    "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
-    "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
-    "CreateTrackerResponseTypeDef",
-    "DataSourceConfigurationOutputTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
-    "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
-    "MapConfigurationOutputTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
-    "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
-    "DescribeTrackerResponseTypeDef",
-    "PositionalAccuracyOutputTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
-    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
-    "GetMapGlyphsResponseTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
-    "GetMapSpritesResponseTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
-    "GetMapStyleDescriptorResponseTypeDef",
     "GetMapTileRequestRequestTypeDef",
-    "GetMapTileResponseTypeDef",
     "GetPlaceRequestRequestTypeDef",
     "LegGeometryTypeDef",
     "StepTypeDef",
-    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
     "ListDevicePositionsRequestRequestTypeDef",
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
     "ListGeofenceCollectionsRequestRequestTypeDef",
     "ListGeofenceCollectionsResponseEntryTypeDef",
-    "ListGeofencesRequestListGeofencesPaginateTypeDef",
     "ListGeofencesRequestRequestTypeDef",
-    "ListMapsRequestListMapsPaginateTypeDef",
     "ListMapsRequestRequestTypeDef",
     "ListMapsResponseEntryTypeDef",
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
     "ListPlaceIndexesRequestRequestTypeDef",
     "ListPlaceIndexesResponseEntryTypeDef",
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
     "ListRouteCalculatorsRequestRequestTypeDef",
     "ListRouteCalculatorsResponseEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
     "ListTrackerConsumersRequestRequestTypeDef",
-    "ListTrackerConsumersResponseTypeDef",
-    "ListTrackersRequestListTrackersPaginateTypeDef",
     "ListTrackersRequestRequestTypeDef",
     "ListTrackersResponseEntryTypeDef",
     "MapConfigurationUpdateTypeDef",
-    "PaginatorConfigTypeDef",
     "PlaceGeometryTypeDef",
     "TimeZoneTypeDef",
-    "PutGeofenceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteMatrixEntryErrorTypeDef",
     "SearchForSuggestionsResultTypeDef",
     "SearchPlaceIndexForPositionRequestRequestTypeDef",
     "SearchPlaceIndexForPositionSummaryTypeDef",
     "SearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     "SearchPlaceIndexForSuggestionsSummaryTypeDef",
     "SearchPlaceIndexForTextRequestRequestTypeDef",
     "SearchPlaceIndexForTextSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
-    "UpdateGeofenceCollectionResponseTypeDef",
-    "UpdateKeyResponseTypeDef",
-    "UpdateMapResponseTypeDef",
-    "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
-    "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
-    "UpdateTrackerResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
+    "CreateGeofenceCollectionResponseTypeDef",
+    "CreateKeyResponseTypeDef",
+    "CreateMapResponseTypeDef",
+    "CreatePlaceIndexResponseTypeDef",
+    "CreateRouteCalculatorResponseTypeDef",
+    "CreateTrackerResponseTypeDef",
+    "DescribeGeofenceCollectionResponseTypeDef",
+    "DescribeKeyResponseTypeDef",
+    "DescribeRouteCalculatorResponseTypeDef",
+    "DescribeTrackerResponseTypeDef",
+    "GetMapGlyphsResponseTypeDef",
+    "GetMapSpritesResponseTypeDef",
+    "GetMapStyleDescriptorResponseTypeDef",
+    "GetMapTileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTrackerConsumersResponseTypeDef",
+    "PutGeofenceResponseTypeDef",
+    "UpdateGeofenceCollectionResponseTypeDef",
+    "UpdateKeyResponseTypeDef",
+    "UpdateMapResponseTypeDef",
+    "UpdatePlaceIndexResponseTypeDef",
+    "UpdateRouteCalculatorResponseTypeDef",
+    "UpdateTrackerResponseTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
     "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
+    "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
-    "UpdatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
-    "DescribeMapResponseTypeDef",
+    "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
+    "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
-    "DevicePositionUpdateTypeDef",
+    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    "ListGeofencesRequestListGeofencesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListMapsRequestListMapsPaginateTypeDef",
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    "ListTrackersRequestListTrackersPaginateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
     "UpdateMapRequestRequestTypeDef",
@@ -191,17 +188,17 @@
     "CalculateRouteRequestRequestTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
     "BatchPutGeofenceRequestEntryTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
-    "ListDevicePositionsResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
+    "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
     "ListGeofencesResponseTypeDef",
     "BatchPutGeofenceRequestRequestTypeDef",
@@ -278,14 +275,25 @@
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
         "TrackerName": str,
     },
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
 BatchDeleteGeofenceRequestRequestTypeDef = TypedDict(
     "BatchDeleteGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceIds": Sequence[str],
     },
 )
@@ -393,35 +401,14 @@
 
 class CreateGeofenceCollectionRequestRequestTypeDef(
     _RequiredCreateGeofenceCollectionRequestRequestTypeDef,
     _OptionalCreateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
-CreateGeofenceCollectionResponseTypeDef = TypedDict(
-    "CreateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateKeyResponseTypeDef = TypedDict(
-    "CreateKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapConfigurationTypeDef = TypedDict(
     "_RequiredMapConfigurationTypeDef",
     {
         "Style": str,
     },
 )
 _OptionalMapConfigurationTypeDef = TypedDict(
@@ -431,42 +418,22 @@
     },
     total=False,
 )
 
 class MapConfigurationTypeDef(_RequiredMapConfigurationTypeDef, _OptionalMapConfigurationTypeDef):
     pass
 
-CreateMapResponseTypeDef = TypedDict(
-    "CreateMapResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "MapArn": str,
-        "MapName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "IntendedUse": IntendedUseType,
     },
     total=False,
 )
 
-CreatePlaceIndexResponseTypeDef = TypedDict(
-    "CreatePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "IndexArn": str,
-        "IndexName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
         "DataSource": str,
     },
 )
@@ -482,24 +449,14 @@
 
 class CreateRouteCalculatorRequestRequestTypeDef(
     _RequiredCreateRouteCalculatorRequestRequestTypeDef,
     _OptionalCreateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
-CreateRouteCalculatorResponseTypeDef = TypedDict(
-    "CreateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
@@ -517,32 +474,14 @@
 )
 
 class CreateTrackerRequestRequestTypeDef(
     _RequiredCreateTrackerRequestRequestTypeDef, _OptionalCreateTrackerRequestRequestTypeDef
 ):
     pass
 
-CreateTrackerResponseTypeDef = TypedDict(
-    "CreateTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "TrackerArn": str,
-        "TrackerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataSourceConfigurationOutputTypeDef = TypedDict(
-    "DataSourceConfigurationOutputTypeDef",
-    {
-        "IntendedUse": IntendedUseType,
-    },
-    total=False,
-)
-
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -584,124 +523,49 @@
 DescribeGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
-DescribeGeofenceCollectionResponseTypeDef = TypedDict(
-    "DescribeGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeKeyRequestRequestTypeDef = TypedDict(
     "DescribeKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 
 DescribeMapRequestRequestTypeDef = TypedDict(
     "DescribeMapRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 
-_RequiredMapConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMapConfigurationOutputTypeDef",
-    {
-        "Style": str,
-    },
-)
-_OptionalMapConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMapConfigurationOutputTypeDef",
-    {
-        "PoliticalView": str,
-    },
-    total=False,
-)
-
-class MapConfigurationOutputTypeDef(
-    _RequiredMapConfigurationOutputTypeDef, _OptionalMapConfigurationOutputTypeDef
-):
-    pass
-
 DescribePlaceIndexRequestRequestTypeDef = TypedDict(
     "DescribePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 
 DescribeRouteCalculatorRequestRequestTypeDef = TypedDict(
     "DescribeRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 
-DescribeRouteCalculatorResponseTypeDef = TypedDict(
-    "DescribeRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTrackerRequestRequestTypeDef = TypedDict(
     "DescribeTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 
-DescribeTrackerResponseTypeDef = TypedDict(
-    "DescribeTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "EventBridgeEnabled": bool,
-        "KmsKeyId": str,
-        "PositionFiltering": PositionFilteringType,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PositionalAccuracyOutputTypeDef = TypedDict(
-    "PositionalAccuracyOutputTypeDef",
-    {
-        "Horizontal": float,
-    },
-)
-
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -709,37 +573,24 @@
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     {
         "ConsumerArn": str,
         "TrackerName": str,
     },
 )
 
-_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
-    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -793,24 +644,14 @@
 )
 
 class GetMapGlyphsRequestRequestTypeDef(
     _RequiredGetMapGlyphsRequestRequestTypeDef, _OptionalGetMapGlyphsRequestRequestTypeDef
 ):
     pass
 
-GetMapGlyphsResponseTypeDef = TypedDict(
-    "GetMapGlyphsResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapSpritesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapSpritesRequestRequestTypeDef",
     {
         "FileName": str,
         "MapName": str,
     },
 )
@@ -823,24 +664,14 @@
 )
 
 class GetMapSpritesRequestRequestTypeDef(
     _RequiredGetMapSpritesRequestRequestTypeDef, _OptionalGetMapSpritesRequestRequestTypeDef
 ):
     pass
 
-GetMapSpritesResponseTypeDef = TypedDict(
-    "GetMapSpritesResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapStyleDescriptorRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 _OptionalGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
@@ -853,24 +684,14 @@
 
 class GetMapStyleDescriptorRequestRequestTypeDef(
     _RequiredGetMapStyleDescriptorRequestRequestTypeDef,
     _OptionalGetMapStyleDescriptorRequestRequestTypeDef,
 ):
     pass
 
-GetMapStyleDescriptorResponseTypeDef = TypedDict(
-    "GetMapStyleDescriptorResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapTileRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapTileRequestRequestTypeDef",
     {
         "MapName": str,
         "X": str,
         "Y": str,
         "Z": str,
@@ -885,24 +706,14 @@
 )
 
 class GetMapTileRequestRequestTypeDef(
     _RequiredGetMapTileRequestRequestTypeDef, _OptionalGetMapTileRequestRequestTypeDef
 ):
     pass
 
-GetMapTileResponseTypeDef = TypedDict(
-    "GetMapTileResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPlaceRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlaceRequestRequestTypeDef",
     {
         "IndexName": str,
         "PlaceId": str,
     },
 )
@@ -944,34 +755,14 @@
     },
     total=False,
 )
 
 class StepTypeDef(_RequiredStepTypeDef, _OptionalStepTypeDef):
     pass
 
-_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
-    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDevicePositionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePositionsRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListDevicePositionsRequestRequestTypeDef = TypedDict(
@@ -985,22 +776,14 @@
 
 class ListDevicePositionsRequestRequestTypeDef(
     _RequiredListDevicePositionsRequestRequestTypeDef,
     _OptionalListDevicePositionsRequestRequestTypeDef,
 ):
     pass
 
-ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeofenceCollectionsRequestRequestTypeDef = TypedDict(
     "ListGeofenceCollectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1026,34 +809,14 @@
 
 class ListGeofenceCollectionsResponseEntryTypeDef(
     _RequiredListGeofenceCollectionsResponseEntryTypeDef,
     _OptionalListGeofenceCollectionsResponseEntryTypeDef,
 ):
     pass
 
-_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "CollectionName": str,
-    },
-)
-_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGeofencesRequestListGeofencesPaginateTypeDef(
-    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
-    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
-):
-    pass
-
 _RequiredListGeofencesRequestRequestTypeDef = TypedDict(
     "_RequiredListGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 _OptionalListGeofencesRequestRequestTypeDef = TypedDict(
@@ -1066,22 +829,14 @@
 )
 
 class ListGeofencesRequestRequestTypeDef(
     _RequiredListGeofencesRequestRequestTypeDef, _OptionalListGeofencesRequestRequestTypeDef
 ):
     pass
 
-ListMapsRequestListMapsPaginateTypeDef = TypedDict(
-    "ListMapsRequestListMapsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMapsRequestRequestTypeDef = TypedDict(
     "ListMapsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1106,22 +861,14 @@
 )
 
 class ListMapsResponseEntryTypeDef(
     _RequiredListMapsResponseEntryTypeDef, _OptionalListMapsResponseEntryTypeDef
 ):
     pass
 
-ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaceIndexesRequestRequestTypeDef = TypedDict(
     "ListPlaceIndexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1146,22 +893,14 @@
 )
 
 class ListPlaceIndexesResponseEntryTypeDef(
     _RequiredListPlaceIndexesResponseEntryTypeDef, _OptionalListPlaceIndexesResponseEntryTypeDef
 ):
     pass
 
-ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRouteCalculatorsRequestRequestTypeDef = TypedDict(
     "ListRouteCalculatorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1194,42 +933,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
-    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-):
-    pass
-
 _RequiredListTrackerConsumersRequestRequestTypeDef = TypedDict(
     "_RequiredListTrackerConsumersRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListTrackerConsumersRequestRequestTypeDef = TypedDict(
@@ -1243,31 +954,14 @@
 
 class ListTrackerConsumersRequestRequestTypeDef(
     _RequiredListTrackerConsumersRequestRequestTypeDef,
     _OptionalListTrackerConsumersRequestRequestTypeDef,
 ):
     pass
 
-ListTrackerConsumersResponseTypeDef = TypedDict(
-    "ListTrackerConsumersResponseTypeDef",
-    {
-        "ConsumerArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
-    "ListTrackersRequestListTrackersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrackersRequestRequestTypeDef = TypedDict(
     "ListTrackersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1300,24 +994,14 @@
     "MapConfigurationUpdateTypeDef",
     {
         "PoliticalView": str,
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
 PlaceGeometryTypeDef = TypedDict(
     "PlaceGeometryTypeDef",
     {
         "Point": List[float],
     },
     total=False,
 )
@@ -1335,35 +1019,14 @@
     },
     total=False,
 )
 
 class TimeZoneTypeDef(_RequiredTimeZoneTypeDef, _OptionalTimeZoneTypeDef):
     pass
 
-PutGeofenceResponseTypeDef = TypedDict(
-    "PutGeofenceResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "GeofenceId": str,
-        "UpdateTime": datetime,
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
 _RequiredRouteMatrixEntryErrorTypeDef = TypedDict(
     "_RequiredRouteMatrixEntryErrorTypeDef",
     {
         "Code": RouteMatrixErrorCodeType,
     },
 )
 _OptionalRouteMatrixEntryErrorTypeDef = TypedDict(
@@ -1585,54 +1248,14 @@
 
 class UpdateGeofenceCollectionRequestRequestTypeDef(
     _RequiredUpdateGeofenceCollectionRequestRequestTypeDef,
     _OptionalUpdateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
-UpdateGeofenceCollectionResponseTypeDef = TypedDict(
-    "UpdateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateKeyResponseTypeDef = TypedDict(
-    "UpdateKeyResponseTypeDef",
-    {
-        "KeyArn": str,
-        "KeyName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMapResponseTypeDef = TypedDict(
-    "UpdateMapResponseTypeDef",
-    {
-        "MapArn": str,
-        "MapName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePlaceIndexResponseTypeDef = TypedDict(
-    "UpdatePlaceIndexResponseTypeDef",
-    {
-        "IndexArn": str,
-        "IndexName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 _OptionalUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
@@ -1646,24 +1269,14 @@
 
 class UpdateRouteCalculatorRequestRequestTypeDef(
     _RequiredUpdateRouteCalculatorRequestRequestTypeDef,
     _OptionalUpdateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
-UpdateRouteCalculatorResponseTypeDef = TypedDict(
-    "UpdateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
@@ -1679,59 +1292,24 @@
 )
 
 class UpdateTrackerRequestRequestTypeDef(
     _RequiredUpdateTrackerRequestRequestTypeDef, _OptionalUpdateTrackerRequestRequestTypeDef
 ):
     pass
 
-UpdateTrackerResponseTypeDef = TypedDict(
-    "UpdateTrackerResponseTypeDef",
-    {
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "Filter": ApiKeyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeKeyResponseTypeDef = TypedDict(
-    "DescribeKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "ExpireTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
         "Restrictions": ApiKeyRestrictionsOutputTypeDef,
@@ -1843,14 +1421,267 @@
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
         "SampleTime": datetime,
     },
 )
 
+CreateGeofenceCollectionResponseTypeDef = TypedDict(
+    "CreateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKeyResponseTypeDef = TypedDict(
+    "CreateKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMapResponseTypeDef = TypedDict(
+    "CreateMapResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "MapArn": str,
+        "MapName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePlaceIndexResponseTypeDef = TypedDict(
+    "CreatePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRouteCalculatorResponseTypeDef = TypedDict(
+    "CreateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrackerResponseTypeDef = TypedDict(
+    "CreateTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGeofenceCollectionResponseTypeDef = TypedDict(
+    "DescribeGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeKeyResponseTypeDef = TypedDict(
+    "DescribeKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "ExpireTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRouteCalculatorResponseTypeDef = TypedDict(
+    "DescribeRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTrackerResponseTypeDef = TypedDict(
+    "DescribeTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "EventBridgeEnabled": bool,
+        "KmsKeyId": str,
+        "PositionFiltering": PositionFilteringType,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapGlyphsResponseTypeDef = TypedDict(
+    "GetMapGlyphsResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapSpritesResponseTypeDef = TypedDict(
+    "GetMapSpritesResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapStyleDescriptorResponseTypeDef = TypedDict(
+    "GetMapStyleDescriptorResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapTileResponseTypeDef = TypedDict(
+    "GetMapTileResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTrackerConsumersResponseTypeDef = TypedDict(
+    "ListTrackerConsumersResponseTypeDef",
+    {
+        "ConsumerArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutGeofenceResponseTypeDef = TypedDict(
+    "PutGeofenceResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "GeofenceId": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGeofenceCollectionResponseTypeDef = TypedDict(
+    "UpdateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKeyResponseTypeDef = TypedDict(
+    "UpdateKeyResponseTypeDef",
+    {
+        "KeyArn": str,
+        "KeyName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMapResponseTypeDef = TypedDict(
+    "UpdateMapResponseTypeDef",
+    {
+        "MapArn": str,
+        "MapName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePlaceIndexResponseTypeDef = TypedDict(
+    "UpdatePlaceIndexResponseTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRouteCalculatorResponseTypeDef = TypedDict(
+    "UpdateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrackerResponseTypeDef = TypedDict(
+    "UpdateTrackerResponseTypeDef",
+    {
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
@@ -1894,14 +1725,30 @@
 )
 
 class CreateMapRequestRequestTypeDef(
     _RequiredCreateMapRequestRequestTypeDef, _OptionalCreateMapRequestRequestTypeDef
 ):
     pass
 
+DescribeMapResponseTypeDef = TypedDict(
+    "DescribeMapResponseTypeDef",
+    {
+        "Configuration": MapConfigurationTypeDef,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "MapArn": str,
+        "MapName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
         "IndexName": str,
     },
 )
@@ -1917,14 +1764,30 @@
 )
 
 class CreatePlaceIndexRequestRequestTypeDef(
     _RequiredCreatePlaceIndexRequestRequestTypeDef, _OptionalCreatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
+DescribePlaceIndexResponseTypeDef = TypedDict(
+    "DescribePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "DataSource": str,
+        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
+        "Description": str,
+        "IndexArn": str,
+        "IndexName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
@@ -1938,125 +1801,225 @@
 )
 
 class UpdatePlaceIndexRequestRequestTypeDef(
     _RequiredUpdatePlaceIndexRequestRequestTypeDef, _OptionalUpdatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
-DescribePlaceIndexResponseTypeDef = TypedDict(
-    "DescribePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "DataSource": str,
-        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
-        "Description": str,
-        "IndexArn": str,
-        "IndexName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMapResponseTypeDef = TypedDict(
-    "DescribeMapResponseTypeDef",
-    {
-        "Configuration": MapConfigurationOutputTypeDef,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "MapArn": str,
-        "MapName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDevicePositionTypeDef = TypedDict(
     "_RequiredDevicePositionTypeDef",
     {
         "Position": List[float],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
     },
 )
 _OptionalDevicePositionTypeDef = TypedDict(
     "_OptionalDevicePositionTypeDef",
     {
-        "Accuracy": PositionalAccuracyOutputTypeDef,
+        "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 class DevicePositionTypeDef(_RequiredDevicePositionTypeDef, _OptionalDevicePositionTypeDef):
     pass
 
+_RequiredDevicePositionUpdateTypeDef = TypedDict(
+    "_RequiredDevicePositionUpdateTypeDef",
+    {
+        "DeviceId": str,
+        "Position": Sequence[float],
+        "SampleTime": Union[datetime, str],
+    },
+)
+_OptionalDevicePositionUpdateTypeDef = TypedDict(
+    "_OptionalDevicePositionUpdateTypeDef",
+    {
+        "Accuracy": PositionalAccuracyTypeDef,
+        "PositionProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class DevicePositionUpdateTypeDef(
+    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
+):
+    pass
+
 GetDevicePositionResponseTypeDef = TypedDict(
     "GetDevicePositionResponseTypeDef",
     {
-        "Accuracy": PositionalAccuracyOutputTypeDef,
+        "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_RequiredListDevicePositionsResponseEntryTypeDef",
     {
         "DeviceId": str,
         "Position": List[float],
         "SampleTime": datetime,
     },
 )
 _OptionalListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_OptionalListDevicePositionsResponseEntryTypeDef",
     {
-        "Accuracy": PositionalAccuracyOutputTypeDef,
+        "Accuracy": PositionalAccuracyTypeDef,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
-_RequiredDevicePositionUpdateTypeDef = TypedDict(
-    "_RequiredDevicePositionUpdateTypeDef",
+_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
         "DeviceId": str,
-        "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
+        "TrackerName": str,
     },
 )
-_OptionalDevicePositionUpdateTypeDef = TypedDict(
-    "_OptionalDevicePositionUpdateTypeDef",
+_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
-        "PositionProperties": Mapping[str, str],
+        "EndTimeExclusive": Union[datetime, str],
+        "StartTimeInclusive": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DevicePositionUpdateTypeDef(
-    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
+class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
+    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
 ):
     pass
 
+_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
+    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+):
+    pass
+
+ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "CollectionName": str,
+    },
+)
+_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGeofencesRequestListGeofencesPaginateTypeDef(
+    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
+    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
+):
+    pass
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "Filter": ApiKeyFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMapsRequestListMapsPaginateTypeDef = TypedDict(
+    "ListMapsRequestListMapsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
+    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+):
+    pass
+
+ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
+    "ListTrackersRequestListTrackersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -2075,51 +2038,51 @@
     pass
 
 ListGeofenceCollectionsResponseTypeDef = TypedDict(
     "ListGeofenceCollectionsResponseTypeDef",
     {
         "Entries": List[ListGeofenceCollectionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMapsResponseTypeDef = TypedDict(
     "ListMapsResponseTypeDef",
     {
         "Entries": List[ListMapsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlaceIndexesResponseTypeDef = TypedDict(
     "ListPlaceIndexesResponseTypeDef",
     {
         "Entries": List[ListPlaceIndexesResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRouteCalculatorsResponseTypeDef = TypedDict(
     "ListRouteCalculatorsResponseTypeDef",
     {
         "Entries": List[ListRouteCalculatorsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrackersResponseTypeDef = TypedDict(
     "ListTrackersResponseTypeDef",
     {
         "Entries": List[ListTrackersResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMapRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMapRequestRequestTypeDef",
     {
         "MapName": str,
@@ -2182,65 +2145,65 @@
 )
 
 SearchPlaceIndexForSuggestionsResponseTypeDef = TypedDict(
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     {
         "Results": List[SearchForSuggestionsResultTypeDef],
         "Summary": SearchPlaceIndexForSuggestionsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Entries": List[ListKeysResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDevicePositionHistoryResponseTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     {
         "Errors": List[BatchDeleteDevicePositionHistoryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteGeofenceResponseTypeDef = TypedDict(
     "BatchDeleteGeofenceResponseTypeDef",
     {
         "Errors": List[BatchDeleteGeofenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesResponseTypeDef = TypedDict(
     "BatchEvaluateGeofencesResponseTypeDef",
     {
         "Errors": List[BatchEvaluateGeofencesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutGeofenceResponseTypeDef = TypedDict(
     "BatchPutGeofenceResponseTypeDef",
     {
         "Errors": List[BatchPutGeofenceErrorTypeDef],
         "Successes": List[BatchPutGeofenceSuccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateDevicePositionResponseTypeDef = TypedDict(
     "BatchUpdateDevicePositionResponseTypeDef",
     {
         "Errors": List[BatchUpdateDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_RequiredCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CalculatorName": str,
@@ -2302,15 +2265,15 @@
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
         "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
@@ -2375,33 +2338,24 @@
     pass
 
 BatchGetDevicePositionResponseTypeDef = TypedDict(
     "BatchGetDevicePositionResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "Errors": List[BatchGetDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDevicePositionHistoryResponseTypeDef = TypedDict(
     "GetDevicePositionHistoryResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevicePositionsResponseTypeDef = TypedDict(
-    "ListDevicePositionsResponseTypeDef",
-    {
-        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2413,28 +2367,37 @@
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     {
         "TrackerName": str,
         "Updates": Sequence[DevicePositionUpdateTypeDef],
     },
 )
 
+ListDevicePositionsResponseTypeDef = TypedDict(
+    "ListDevicePositionsResponseTypeDef",
+    {
+        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPlaceResponseTypeDef = TypedDict(
     "GetPlaceResponseTypeDef",
     {
         "Place": PlaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchForPositionResultTypeDef = TypedDict(
     "_RequiredSearchForPositionResultTypeDef",
     {
         "Distance": float,
@@ -2478,24 +2441,24 @@
 CalculateRouteMatrixResponseTypeDef = TypedDict(
     "CalculateRouteMatrixResponseTypeDef",
     {
         "RouteMatrix": List[List[RouteMatrixEntryTypeDef]],
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutGeofenceRequestRequestTypeDef = TypedDict(
     "BatchPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2504,19 +2467,19 @@
 )
 
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchPlaceIndexForTextResponseTypeDef = TypedDict(
     "SearchPlaceIndexForTextResponseTypeDef",
     {
         "Results": List[SearchForTextResultTypeDef],
         "Summary": SearchPlaceIndexForTextSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.12
-Summary: Type annotations for boto3.LocationService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,143 +373,140 @@
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
-    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
-    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
-    CreateTrackerResponseTypeDef,
-    DataSourceConfigurationOutputTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
-    MapConfigurationOutputTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
-    DescribeTrackerResponseTypeDef,
-    PositionalAccuracyOutputTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
-    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
-    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
-    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
     MapConfigurationUpdateTypeDef,
-    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
-    PutGeofenceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
-    UpdateTrackerResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
+    CreateMapResponseTypeDef,
+    CreatePlaceIndexResponseTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
+    CreateTrackerResponseTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
+    DescribeKeyResponseTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
+    DescribeTrackerResponseTypeDef,
+    GetMapGlyphsResponseTypeDef,
+    GetMapSpritesResponseTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
+    GetMapTileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    PutGeofenceResponseTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
+    UpdateTrackerResponseTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
+    DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
-    UpdatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
-    DescribeMapResponseTypeDef,
+    UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
+    DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
-    DevicePositionUpdateTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -526,17 +523,17 @@
     CalculateRouteRequestRequestTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
-    ListDevicePositionsResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
+    ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
     ListGeofencesResponseTypeDef,
     BatchPutGeofenceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.12/setup.py` & `mypy-boto3-location-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LocationService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LocationService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

