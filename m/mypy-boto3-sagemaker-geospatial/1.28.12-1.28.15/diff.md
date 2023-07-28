# Comparing `tmp/mypy-boto3-sagemaker-geospatial-1.28.12.tar.gz` & `tmp/mypy-boto3-sagemaker-geospatial-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.28.12.tar", last modified: Thu Jul 27 11:49:35 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.28.15.tar", last modified: Fri Jul 28 20:43:39 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-geospatial-1.28.12.tar` & `mypy-boto3-sagemaker-geospatial-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.721264 mypy-boto3-sagemaker-geospatial-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-07-27 11:49:35.709264 mypy-boto3-sagemaker-geospatial-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.709264 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-27 11:45:58.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-07-27 11:45:58.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.709264 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:35.721264 mypy-boto3-sagemaker-geospatial-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:39.929812 mypy-boto3-sagemaker-geospatial-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-28 20:43:39.929812 mypy-boto3-sagemaker-geospatial-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:39.925812 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39531 2023-07-28 20:38:31.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-07-28 20:38:27.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:39.929812 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-28 20:43:39.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:43:39.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:39.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:39.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:39.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:43:39.000000 mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:39.929812 mypy-boto3-sagemaker-geospatial-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 20:38:26.000000 mypy-boto3-sagemaker-geospatial-1.28.15/setup.py
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/LICENSE` & `mypy-boto3-sagemaker-geospatial-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.28.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-geospatial
-Version: 1.28.12
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,26 +365,22 @@
     MultiPolygonGeometryInputOutputTypeDef,
     PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
     AssetValueTypeDef,
     CloudRemovalConfigInputOutputTypeDef,
     CloudRemovalConfigInputTypeDef,
-    OperationOutputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
-    EoCloudCoverInputOutputTypeDef,
     EoCloudCoverInputTypeDef,
     ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
-    ExportS3DataInputOutputTypeDef,
     ExportS3DataInputTypeDef,
-    VectorEnrichmentJobS3DataOutputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
     GeoMosaicConfigInputOutputTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
@@ -394,93 +390,76 @@
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
     TemporalStatisticsConfigInputOutputTypeDef,
     ZonalStatisticsConfigInputOutputTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
-    LandsatCloudCoverLandInputOutputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
     PaginatorConfigTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
-    MapMatchingConfigOutputTypeDef,
     MapMatchingConfigTypeDef,
-    UserDefinedOutputTypeDef,
     UserDefinedTypeDef,
-    PlatformInputOutputTypeDef,
     PlatformInputTypeDef,
-    ViewOffNadirInputOutputTypeDef,
-    ViewSunAzimuthInputOutputTypeDef,
-    ViewSunElevationInputOutputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
-    ReverseGeocodingConfigOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
     GetTileOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
-    OutputConfigInputOutputTypeDef,
     OutputConfigInputTypeDef,
-    ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
-    VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
     ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
     ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
-    OutputResolutionResamplingInputOutputTypeDef,
-    OutputResolutionStackInputOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
-    PropertyOutputTypeDef,
     PropertyTypeDef,
-    VectorEnrichmentJobConfigOutputTypeDef,
     VectorEnrichmentJobConfigTypeDef,
     AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
     BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
-    ExportEarthObservationJobOutputTypeDef,
     ExportEarthObservationJobInputRequestTypeDef,
-    ExportVectorEnrichmentJobOutputTypeDef,
-    VectorEnrichmentJobInputConfigOutputTypeDef,
+    ExportEarthObservationJobOutputTypeDef,
     ExportVectorEnrichmentJobInputRequestTypeDef,
+    ExportVectorEnrichmentJobOutputTypeDef,
     VectorEnrichmentJobInputConfigTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
     ResamplingConfigInputOutputTypeDef,
-    StackConfigInputOutputTypeDef,
     ResamplingConfigInputTypeDef,
+    StackConfigInputOutputTypeDef,
     StackConfigInputTypeDef,
-    PropertyFilterOutputTypeDef,
     PropertyFilterTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
-    StartVectorEnrichmentJobOutputTypeDef,
     StartVectorEnrichmentJobInputRequestTypeDef,
+    StartVectorEnrichmentJobOutputTypeDef,
     JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
     PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
     RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/README.md` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sagemaker-geospatial
+Version: 1.28.15
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,26 +365,22 @@
     MultiPolygonGeometryInputOutputTypeDef,
     PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
     AssetValueTypeDef,
     CloudRemovalConfigInputOutputTypeDef,
     CloudRemovalConfigInputTypeDef,
-    OperationOutputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
-    EoCloudCoverInputOutputTypeDef,
     EoCloudCoverInputTypeDef,
     ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
-    ExportS3DataInputOutputTypeDef,
     ExportS3DataInputTypeDef,
-    VectorEnrichmentJobS3DataOutputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
     GeoMosaicConfigInputOutputTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
@@ -362,93 +390,76 @@
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
     TemporalStatisticsConfigInputOutputTypeDef,
     ZonalStatisticsConfigInputOutputTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
-    LandsatCloudCoverLandInputOutputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
     PaginatorConfigTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
-    MapMatchingConfigOutputTypeDef,
     MapMatchingConfigTypeDef,
-    UserDefinedOutputTypeDef,
     UserDefinedTypeDef,
-    PlatformInputOutputTypeDef,
     PlatformInputTypeDef,
-    ViewOffNadirInputOutputTypeDef,
-    ViewSunAzimuthInputOutputTypeDef,
-    ViewSunElevationInputOutputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
-    ReverseGeocodingConfigOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
     GetTileOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
-    OutputConfigInputOutputTypeDef,
     OutputConfigInputTypeDef,
-    ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
-    VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
     ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
     ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
-    OutputResolutionResamplingInputOutputTypeDef,
-    OutputResolutionStackInputOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
-    PropertyOutputTypeDef,
     PropertyTypeDef,
-    VectorEnrichmentJobConfigOutputTypeDef,
     VectorEnrichmentJobConfigTypeDef,
     AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
     BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
-    ExportEarthObservationJobOutputTypeDef,
     ExportEarthObservationJobInputRequestTypeDef,
-    ExportVectorEnrichmentJobOutputTypeDef,
-    VectorEnrichmentJobInputConfigOutputTypeDef,
+    ExportEarthObservationJobOutputTypeDef,
     ExportVectorEnrichmentJobInputRequestTypeDef,
+    ExportVectorEnrichmentJobOutputTypeDef,
     VectorEnrichmentJobInputConfigTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
     ResamplingConfigInputOutputTypeDef,
-    StackConfigInputOutputTypeDef,
     ResamplingConfigInputTypeDef,
+    StackConfigInputOutputTypeDef,
     StackConfigInputTypeDef,
-    PropertyFilterOutputTypeDef,
     PropertyFilterTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
-    StartVectorEnrichmentJobOutputTypeDef,
     StartVectorEnrichmentJobInputRequestTypeDef,
+    StartVectorEnrichmentJobOutputTypeDef,
     JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
     PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
     RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__main__.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,26 +54,22 @@
     "MultiPolygonGeometryInputOutputTypeDef",
     "PolygonGeometryInputOutputTypeDef",
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
     "CloudRemovalConfigInputOutputTypeDef",
     "CloudRemovalConfigInputTypeDef",
-    "OperationOutputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
-    "EoCloudCoverInputOutputTypeDef",
     "EoCloudCoverInputTypeDef",
     "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
-    "ExportS3DataInputOutputTypeDef",
     "ExportS3DataInputTypeDef",
-    "VectorEnrichmentJobS3DataOutputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
     "GeoMosaicConfigInputOutputTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
@@ -83,93 +79,76 @@
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
     "TemporalStatisticsConfigInputOutputTypeDef",
     "ZonalStatisticsConfigInputOutputTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
-    "LandsatCloudCoverLandInputOutputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
     "PaginatorConfigTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVectorEnrichmentJobInputRequestTypeDef",
     "ListVectorEnrichmentJobOutputConfigTypeDef",
-    "MapMatchingConfigOutputTypeDef",
     "MapMatchingConfigTypeDef",
-    "UserDefinedOutputTypeDef",
     "UserDefinedTypeDef",
-    "PlatformInputOutputTypeDef",
     "PlatformInputTypeDef",
-    "ViewOffNadirInputOutputTypeDef",
-    "ViewSunAzimuthInputOutputTypeDef",
-    "ViewSunElevationInputOutputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
     "TimeRangeFilterInputTypeDef",
     "TimeRangeFilterOutputTypeDef",
-    "ReverseGeocodingConfigOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
     "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
     "GetTileOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
-    "OutputConfigInputOutputTypeDef",
     "OutputConfigInputTypeDef",
-    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
-    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
     "GetRasterDataCollectionOutputTypeDef",
     "RasterDataCollectionMetadataTypeDef",
     "ItemSourceTypeDef",
     "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
     "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
     "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
-    "OutputResolutionResamplingInputOutputTypeDef",
-    "OutputResolutionStackInputOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
-    "PropertyOutputTypeDef",
     "PropertyTypeDef",
-    "VectorEnrichmentJobConfigOutputTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
     "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
     "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
-    "ExportEarthObservationJobOutputTypeDef",
     "ExportEarthObservationJobInputRequestTypeDef",
-    "ExportVectorEnrichmentJobOutputTypeDef",
-    "VectorEnrichmentJobInputConfigOutputTypeDef",
+    "ExportEarthObservationJobOutputTypeDef",
     "ExportVectorEnrichmentJobInputRequestTypeDef",
+    "ExportVectorEnrichmentJobOutputTypeDef",
     "VectorEnrichmentJobInputConfigTypeDef",
     "ListRasterDataCollectionsOutputTypeDef",
     "SearchRasterDataCollectionOutputTypeDef",
     "ResamplingConfigInputOutputTypeDef",
-    "StackConfigInputOutputTypeDef",
     "ResamplingConfigInputTypeDef",
+    "StackConfigInputOutputTypeDef",
     "StackConfigInputTypeDef",
-    "PropertyFilterOutputTypeDef",
     "PropertyFilterTypeDef",
     "GetVectorEnrichmentJobOutputTypeDef",
-    "StartVectorEnrichmentJobOutputTypeDef",
     "StartVectorEnrichmentJobInputRequestTypeDef",
+    "StartVectorEnrichmentJobOutputTypeDef",
     "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
     "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
     "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
@@ -233,34 +212,14 @@
         "AlgorithmName": Literal["INTERPOLATION"],
         "InterpolationValue": str,
         "TargetBands": Sequence[str],
     },
     total=False,
 )
 
-_RequiredOperationOutputTypeDef = TypedDict(
-    "_RequiredOperationOutputTypeDef",
-    {
-        "Equation": str,
-        "Name": str,
-    },
-)
-_OptionalOperationOutputTypeDef = TypedDict(
-    "_OptionalOperationOutputTypeDef",
-    {
-        "OutputType": OutputTypeType,
-    },
-    total=False,
-)
-
-
-class OperationOutputTypeDef(_RequiredOperationOutputTypeDef, _OptionalOperationOutputTypeDef):
-    pass
-
-
 _RequiredOperationTypeDef = TypedDict(
     "_RequiredOperationTypeDef",
     {
         "Equation": str,
         "Name": str,
     },
 )
@@ -296,22 +255,14 @@
     {
         "Message": str,
         "Type": EarthObservationJobErrorTypeType,
     },
     total=False,
 )
 
-EoCloudCoverInputOutputTypeDef = TypedDict(
-    "EoCloudCoverInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
 EoCloudCoverInputTypeDef = TypedDict(
     "EoCloudCoverInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -332,35 +283,14 @@
     {
         "Message": str,
         "Type": ExportErrorTypeType,
     },
     total=False,
 )
 
-_RequiredExportS3DataInputOutputTypeDef = TypedDict(
-    "_RequiredExportS3DataInputOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalExportS3DataInputOutputTypeDef = TypedDict(
-    "_OptionalExportS3DataInputOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class ExportS3DataInputOutputTypeDef(
-    _RequiredExportS3DataInputOutputTypeDef, _OptionalExportS3DataInputOutputTypeDef
-):
-    pass
-
-
 _RequiredExportS3DataInputTypeDef = TypedDict(
     "_RequiredExportS3DataInputTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalExportS3DataInputTypeDef = TypedDict(
@@ -374,35 +304,14 @@
 
 class ExportS3DataInputTypeDef(
     _RequiredExportS3DataInputTypeDef, _OptionalExportS3DataInputTypeDef
 ):
     pass
 
 
-_RequiredVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
-    "_RequiredVectorEnrichmentJobS3DataOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
-    "_OptionalVectorEnrichmentJobS3DataOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class VectorEnrichmentJobS3DataOutputTypeDef(
-    _RequiredVectorEnrichmentJobS3DataOutputTypeDef, _OptionalVectorEnrichmentJobS3DataOutputTypeDef
-):
-    pass
-
-
 _RequiredVectorEnrichmentJobS3DataTypeDef = TypedDict(
     "_RequiredVectorEnrichmentJobS3DataTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalVectorEnrichmentJobS3DataTypeDef = TypedDict(
@@ -646,22 +555,14 @@
 
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
 ):
     pass
 
 
-LandsatCloudCoverLandInputOutputTypeDef = TypedDict(
-    "LandsatCloudCoverLandInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
 LandsatCloudCoverLandInputTypeDef = TypedDict(
     "LandsatCloudCoverLandInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -766,71 +667,32 @@
 class ListVectorEnrichmentJobOutputConfigTypeDef(
     _RequiredListVectorEnrichmentJobOutputConfigTypeDef,
     _OptionalListVectorEnrichmentJobOutputConfigTypeDef,
 ):
     pass
 
 
-MapMatchingConfigOutputTypeDef = TypedDict(
-    "MapMatchingConfigOutputTypeDef",
-    {
-        "IdAttributeName": str,
-        "TimestampAttributeName": str,
-        "XAttributeName": str,
-        "YAttributeName": str,
-    },
-)
-
 MapMatchingConfigTypeDef = TypedDict(
     "MapMatchingConfigTypeDef",
     {
         "IdAttributeName": str,
         "TimestampAttributeName": str,
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
 
-UserDefinedOutputTypeDef = TypedDict(
-    "UserDefinedOutputTypeDef",
-    {
-        "Unit": Literal["METERS"],
-        "Value": float,
-    },
-)
-
 UserDefinedTypeDef = TypedDict(
     "UserDefinedTypeDef",
     {
         "Unit": Literal["METERS"],
         "Value": float,
     },
 )
 
-_RequiredPlatformInputOutputTypeDef = TypedDict(
-    "_RequiredPlatformInputOutputTypeDef",
-    {
-        "Value": str,
-    },
-)
-_OptionalPlatformInputOutputTypeDef = TypedDict(
-    "_OptionalPlatformInputOutputTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-    total=False,
-)
-
-
-class PlatformInputOutputTypeDef(
-    _RequiredPlatformInputOutputTypeDef, _OptionalPlatformInputOutputTypeDef
-):
-    pass
-
-
 _RequiredPlatformInputTypeDef = TypedDict(
     "_RequiredPlatformInputTypeDef",
     {
         "Value": str,
     },
 )
 _OptionalPlatformInputTypeDef = TypedDict(
@@ -842,38 +704,14 @@
 )
 
 
 class PlatformInputTypeDef(_RequiredPlatformInputTypeDef, _OptionalPlatformInputTypeDef):
     pass
 
 
-ViewOffNadirInputOutputTypeDef = TypedDict(
-    "ViewOffNadirInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
-ViewSunAzimuthInputOutputTypeDef = TypedDict(
-    "ViewSunAzimuthInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
-ViewSunElevationInputOutputTypeDef = TypedDict(
-    "ViewSunElevationInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
 ViewOffNadirInputTypeDef = TypedDict(
     "ViewOffNadirInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -906,22 +744,14 @@
     "TimeRangeFilterOutputTypeDef",
     {
         "EndTime": datetime,
         "StartTime": datetime,
     },
 )
 
-ReverseGeocodingConfigOutputTypeDef = TypedDict(
-    "ReverseGeocodingConfigOutputTypeDef",
-    {
-        "XAttributeName": str,
-        "YAttributeName": str,
-    },
-)
-
 ReverseGeocodingConfigTypeDef = TypedDict(
     "ReverseGeocodingConfigTypeDef",
     {
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
@@ -973,15 +803,15 @@
     },
     total=False,
 )
 
 CustomIndicesInputOutputTypeDef = TypedDict(
     "CustomIndicesInputOutputTypeDef",
     {
-        "Operations": List[OperationOutputTypeDef],
+        "Operations": List[OperationTypeDef],
     },
     total=False,
 )
 
 CustomIndicesInputTypeDef = TypedDict(
     "CustomIndicesInputTypeDef",
     {
@@ -1011,43 +841,21 @@
     {
         "ExportResults": ExportErrorDetailsOutputTypeDef,
         "ExportSourceImages": ExportErrorDetailsOutputTypeDef,
     },
     total=False,
 )
 
-OutputConfigInputOutputTypeDef = TypedDict(
-    "OutputConfigInputOutputTypeDef",
-    {
-        "S3Data": ExportS3DataInputOutputTypeDef,
-    },
-)
-
 OutputConfigInputTypeDef = TypedDict(
     "OutputConfigInputTypeDef",
     {
         "S3Data": ExportS3DataInputTypeDef,
     },
 )
 
-ExportVectorEnrichmentJobOutputConfigOutputTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
-    {
-        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
-    },
-)
-
-VectorEnrichmentJobDataSourceConfigInputOutputTypeDef = TypedDict(
-    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
-    {
-        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
-    },
-    total=False,
-)
-
 ExportVectorEnrichmentJobOutputConfigTypeDef = TypedDict(
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     {
         "S3Data": VectorEnrichmentJobS3DataTypeDef,
     },
 )
 
@@ -1166,30 +974,14 @@
     {
         "NextToken": str,
         "VectorEnrichmentJobSummaries": List[ListVectorEnrichmentJobOutputConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OutputResolutionResamplingInputOutputTypeDef = TypedDict(
-    "OutputResolutionResamplingInputOutputTypeDef",
-    {
-        "UserDefined": UserDefinedOutputTypeDef,
-    },
-)
-
-OutputResolutionStackInputOutputTypeDef = TypedDict(
-    "OutputResolutionStackInputOutputTypeDef",
-    {
-        "Predefined": PredefinedResolutionType,
-        "UserDefined": UserDefinedOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputResolutionResamplingInputTypeDef = TypedDict(
     "OutputResolutionResamplingInputTypeDef",
     {
         "UserDefined": UserDefinedTypeDef,
     },
 )
 
@@ -1198,49 +990,27 @@
     {
         "Predefined": PredefinedResolutionType,
         "UserDefined": UserDefinedTypeDef,
     },
     total=False,
 )
 
-PropertyOutputTypeDef = TypedDict(
-    "PropertyOutputTypeDef",
-    {
-        "EoCloudCover": EoCloudCoverInputOutputTypeDef,
-        "LandsatCloudCoverLand": LandsatCloudCoverLandInputOutputTypeDef,
-        "Platform": PlatformInputOutputTypeDef,
-        "ViewOffNadir": ViewOffNadirInputOutputTypeDef,
-        "ViewSunAzimuth": ViewSunAzimuthInputOutputTypeDef,
-        "ViewSunElevation": ViewSunElevationInputOutputTypeDef,
-    },
-    total=False,
-)
-
 PropertyTypeDef = TypedDict(
     "PropertyTypeDef",
     {
         "EoCloudCover": EoCloudCoverInputTypeDef,
         "LandsatCloudCoverLand": LandsatCloudCoverLandInputTypeDef,
         "Platform": PlatformInputTypeDef,
         "ViewOffNadir": ViewOffNadirInputTypeDef,
         "ViewSunAzimuth": ViewSunAzimuthInputTypeDef,
         "ViewSunElevation": ViewSunElevationInputTypeDef,
     },
     total=False,
 )
 
-VectorEnrichmentJobConfigOutputTypeDef = TypedDict(
-    "VectorEnrichmentJobConfigOutputTypeDef",
-    {
-        "MapMatchingConfig": MapMatchingConfigOutputTypeDef,
-        "ReverseGeocodingConfig": ReverseGeocodingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 VectorEnrichmentJobConfigTypeDef = TypedDict(
     "VectorEnrichmentJobConfigTypeDef",
     {
         "MapMatchingConfig": MapMatchingConfigTypeDef,
         "ReverseGeocodingConfig": ReverseGeocodingConfigTypeDef,
     },
     total=False,
@@ -1276,27 +1046,14 @@
     {
         "CustomIndices": CustomIndicesInputTypeDef,
         "PredefinedIndices": Sequence[str],
     },
     total=False,
 )
 
-ExportEarthObservationJobOutputTypeDef = TypedDict(
-    "ExportEarthObservationJobOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionRoleArn": str,
-        "ExportSourceImages": bool,
-        "ExportStatus": EarthObservationJobExportStatusType,
-        "OutputConfig": OutputConfigInputOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredExportEarthObservationJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": OutputConfigInputTypeDef,
     },
@@ -1314,34 +1071,27 @@
 class ExportEarthObservationJobInputRequestTypeDef(
     _RequiredExportEarthObservationJobInputRequestTypeDef,
     _OptionalExportEarthObservationJobInputRequestTypeDef,
 ):
     pass
 
 
-ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobOutputTypeDef",
+ExportEarthObservationJobOutputTypeDef = TypedDict(
+    "ExportEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
-        "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "OutputConfig": ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+        "ExportSourceImages": bool,
+        "ExportStatus": EarthObservationJobExportStatusType,
+        "OutputConfig": OutputConfigInputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VectorEnrichmentJobInputConfigOutputTypeDef = TypedDict(
-    "VectorEnrichmentJobInputConfigOutputTypeDef",
-    {
-        "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
-        "DocumentType": Literal["CSV"],
-    },
-)
-
 _RequiredExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
     },
@@ -1358,14 +1108,26 @@
 class ExportVectorEnrichmentJobInputRequestTypeDef(
     _RequiredExportVectorEnrichmentJobInputRequestTypeDef,
     _OptionalExportVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
 
+ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "ExportVectorEnrichmentJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionRoleArn": str,
+        "ExportStatus": VectorEnrichmentJobExportStatusType,
+        "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VectorEnrichmentJobInputConfigTypeDef = TypedDict(
     "VectorEnrichmentJobInputConfigTypeDef",
     {
         "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputTypeDef,
         "DocumentType": Literal["CSV"],
     },
 )
@@ -1388,15 +1150,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResamplingConfigInputOutputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputOutputTypeDef",
     {
-        "OutputResolution": OutputResolutionResamplingInputOutputTypeDef,
+        "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputOutputTypeDef = TypedDict(
     "_OptionalResamplingConfigInputOutputTypeDef",
     {
         "AlgorithmName": AlgorithmNameResamplingType,
         "TargetBands": List[str],
@@ -1407,23 +1169,14 @@
 
 class ResamplingConfigInputOutputTypeDef(
     _RequiredResamplingConfigInputOutputTypeDef, _OptionalResamplingConfigInputOutputTypeDef
 ):
     pass
 
 
-StackConfigInputOutputTypeDef = TypedDict(
-    "StackConfigInputOutputTypeDef",
-    {
-        "OutputResolution": OutputResolutionStackInputOutputTypeDef,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputTypeDef = TypedDict(
@@ -1438,28 +1191,30 @@
 
 class ResamplingConfigInputTypeDef(
     _RequiredResamplingConfigInputTypeDef, _OptionalResamplingConfigInputTypeDef
 ):
     pass
 
 
-StackConfigInputTypeDef = TypedDict(
-    "StackConfigInputTypeDef",
+StackConfigInputOutputTypeDef = TypedDict(
+    "StackConfigInputOutputTypeDef",
     {
         "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
-PropertyFilterOutputTypeDef = TypedDict(
-    "PropertyFilterOutputTypeDef",
+StackConfigInputTypeDef = TypedDict(
+    "StackConfigInputTypeDef",
     {
-        "Property": PropertyOutputTypeDef,
+        "OutputResolution": OutputResolutionStackInputTypeDef,
+        "TargetBands": Sequence[str],
     },
+    total=False,
 )
 
 PropertyFilterTypeDef = TypedDict(
     "PropertyFilterTypeDef",
     {
         "Property": PropertyTypeDef,
     },
@@ -1471,34 +1226,16 @@
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": VectorEnrichmentJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": VectorEnrichmentJobExportErrorDetailsTypeDef,
         "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
-        "KmsKeyId": str,
-        "Name": str,
-        "Status": VectorEnrichmentJobStatusType,
-        "Tags": Dict[str, str],
-        "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "StartVectorEnrichmentJobOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "DurationInSeconds": int,
-        "ExecutionRoleArn": str,
-        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
+        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1527,14 +1264,32 @@
 class StartVectorEnrichmentJobInputRequestTypeDef(
     _RequiredStartVectorEnrichmentJobInputRequestTypeDef,
     _OptionalStartVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
 
+StartVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "StartVectorEnrichmentJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "DurationInSeconds": int,
+        "ExecutionRoleArn": str,
+        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigTypeDef,
+        "KmsKeyId": str,
+        "Name": str,
+        "Status": VectorEnrichmentJobStatusType,
+        "Tags": Dict[str, str],
+        "Type": VectorEnrichmentJobTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 JobConfigInputOutputTypeDef = TypedDict(
     "JobConfigInputOutputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputOutputTypeDef,
         "CloudMaskingConfig": Dict[str, Any],
         "CloudRemovalConfig": CloudRemovalConfigInputOutputTypeDef,
         "GeoMosaicConfig": GeoMosaicConfigInputOutputTypeDef,
@@ -1563,15 +1318,15 @@
     total=False,
 )
 
 PropertyFiltersOutputTypeDef = TypedDict(
     "PropertyFiltersOutputTypeDef",
     {
         "LogicalOperator": Literal["AND"],
-        "Properties": List[PropertyFilterOutputTypeDef],
+        "Properties": List[PropertyFilterTypeDef],
     },
     total=False,
 )
 
 PropertyFiltersTypeDef = TypedDict(
     "PropertyFiltersTypeDef",
     {
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -53,26 +53,22 @@
     "MultiPolygonGeometryInputOutputTypeDef",
     "PolygonGeometryInputOutputTypeDef",
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
     "CloudRemovalConfigInputOutputTypeDef",
     "CloudRemovalConfigInputTypeDef",
-    "OperationOutputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
-    "EoCloudCoverInputOutputTypeDef",
     "EoCloudCoverInputTypeDef",
     "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
-    "ExportS3DataInputOutputTypeDef",
     "ExportS3DataInputTypeDef",
-    "VectorEnrichmentJobS3DataOutputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
     "GeoMosaicConfigInputOutputTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
@@ -82,93 +78,76 @@
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
     "TemporalStatisticsConfigInputOutputTypeDef",
     "ZonalStatisticsConfigInputOutputTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
-    "LandsatCloudCoverLandInputOutputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
     "PaginatorConfigTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVectorEnrichmentJobInputRequestTypeDef",
     "ListVectorEnrichmentJobOutputConfigTypeDef",
-    "MapMatchingConfigOutputTypeDef",
     "MapMatchingConfigTypeDef",
-    "UserDefinedOutputTypeDef",
     "UserDefinedTypeDef",
-    "PlatformInputOutputTypeDef",
     "PlatformInputTypeDef",
-    "ViewOffNadirInputOutputTypeDef",
-    "ViewSunAzimuthInputOutputTypeDef",
-    "ViewSunElevationInputOutputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
     "TimeRangeFilterInputTypeDef",
     "TimeRangeFilterOutputTypeDef",
-    "ReverseGeocodingConfigOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
     "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
     "GetTileOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
-    "OutputConfigInputOutputTypeDef",
     "OutputConfigInputTypeDef",
-    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
-    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
     "GetRasterDataCollectionOutputTypeDef",
     "RasterDataCollectionMetadataTypeDef",
     "ItemSourceTypeDef",
     "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
     "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
     "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
-    "OutputResolutionResamplingInputOutputTypeDef",
-    "OutputResolutionStackInputOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
-    "PropertyOutputTypeDef",
     "PropertyTypeDef",
-    "VectorEnrichmentJobConfigOutputTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
     "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
     "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
-    "ExportEarthObservationJobOutputTypeDef",
     "ExportEarthObservationJobInputRequestTypeDef",
-    "ExportVectorEnrichmentJobOutputTypeDef",
-    "VectorEnrichmentJobInputConfigOutputTypeDef",
+    "ExportEarthObservationJobOutputTypeDef",
     "ExportVectorEnrichmentJobInputRequestTypeDef",
+    "ExportVectorEnrichmentJobOutputTypeDef",
     "VectorEnrichmentJobInputConfigTypeDef",
     "ListRasterDataCollectionsOutputTypeDef",
     "SearchRasterDataCollectionOutputTypeDef",
     "ResamplingConfigInputOutputTypeDef",
-    "StackConfigInputOutputTypeDef",
     "ResamplingConfigInputTypeDef",
+    "StackConfigInputOutputTypeDef",
     "StackConfigInputTypeDef",
-    "PropertyFilterOutputTypeDef",
     "PropertyFilterTypeDef",
     "GetVectorEnrichmentJobOutputTypeDef",
-    "StartVectorEnrichmentJobOutputTypeDef",
     "StartVectorEnrichmentJobInputRequestTypeDef",
+    "StartVectorEnrichmentJobOutputTypeDef",
     "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
     "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
     "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
@@ -232,32 +211,14 @@
         "AlgorithmName": Literal["INTERPOLATION"],
         "InterpolationValue": str,
         "TargetBands": Sequence[str],
     },
     total=False,
 )
 
-_RequiredOperationOutputTypeDef = TypedDict(
-    "_RequiredOperationOutputTypeDef",
-    {
-        "Equation": str,
-        "Name": str,
-    },
-)
-_OptionalOperationOutputTypeDef = TypedDict(
-    "_OptionalOperationOutputTypeDef",
-    {
-        "OutputType": OutputTypeType,
-    },
-    total=False,
-)
-
-class OperationOutputTypeDef(_RequiredOperationOutputTypeDef, _OptionalOperationOutputTypeDef):
-    pass
-
 _RequiredOperationTypeDef = TypedDict(
     "_RequiredOperationTypeDef",
     {
         "Equation": str,
         "Name": str,
     },
 )
@@ -291,22 +252,14 @@
     {
         "Message": str,
         "Type": EarthObservationJobErrorTypeType,
     },
     total=False,
 )
 
-EoCloudCoverInputOutputTypeDef = TypedDict(
-    "EoCloudCoverInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
 EoCloudCoverInputTypeDef = TypedDict(
     "EoCloudCoverInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -327,33 +280,14 @@
     {
         "Message": str,
         "Type": ExportErrorTypeType,
     },
     total=False,
 )
 
-_RequiredExportS3DataInputOutputTypeDef = TypedDict(
-    "_RequiredExportS3DataInputOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalExportS3DataInputOutputTypeDef = TypedDict(
-    "_OptionalExportS3DataInputOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class ExportS3DataInputOutputTypeDef(
-    _RequiredExportS3DataInputOutputTypeDef, _OptionalExportS3DataInputOutputTypeDef
-):
-    pass
-
 _RequiredExportS3DataInputTypeDef = TypedDict(
     "_RequiredExportS3DataInputTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalExportS3DataInputTypeDef = TypedDict(
@@ -365,33 +299,14 @@
 )
 
 class ExportS3DataInputTypeDef(
     _RequiredExportS3DataInputTypeDef, _OptionalExportS3DataInputTypeDef
 ):
     pass
 
-_RequiredVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
-    "_RequiredVectorEnrichmentJobS3DataOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
-    "_OptionalVectorEnrichmentJobS3DataOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class VectorEnrichmentJobS3DataOutputTypeDef(
-    _RequiredVectorEnrichmentJobS3DataOutputTypeDef, _OptionalVectorEnrichmentJobS3DataOutputTypeDef
-):
-    pass
-
 _RequiredVectorEnrichmentJobS3DataTypeDef = TypedDict(
     "_RequiredVectorEnrichmentJobS3DataTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalVectorEnrichmentJobS3DataTypeDef = TypedDict(
@@ -621,22 +536,14 @@
 )
 
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
 ):
     pass
 
-LandsatCloudCoverLandInputOutputTypeDef = TypedDict(
-    "LandsatCloudCoverLandInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
 LandsatCloudCoverLandInputTypeDef = TypedDict(
     "LandsatCloudCoverLandInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -737,69 +644,32 @@
 
 class ListVectorEnrichmentJobOutputConfigTypeDef(
     _RequiredListVectorEnrichmentJobOutputConfigTypeDef,
     _OptionalListVectorEnrichmentJobOutputConfigTypeDef,
 ):
     pass
 
-MapMatchingConfigOutputTypeDef = TypedDict(
-    "MapMatchingConfigOutputTypeDef",
-    {
-        "IdAttributeName": str,
-        "TimestampAttributeName": str,
-        "XAttributeName": str,
-        "YAttributeName": str,
-    },
-)
-
 MapMatchingConfigTypeDef = TypedDict(
     "MapMatchingConfigTypeDef",
     {
         "IdAttributeName": str,
         "TimestampAttributeName": str,
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
 
-UserDefinedOutputTypeDef = TypedDict(
-    "UserDefinedOutputTypeDef",
-    {
-        "Unit": Literal["METERS"],
-        "Value": float,
-    },
-)
-
 UserDefinedTypeDef = TypedDict(
     "UserDefinedTypeDef",
     {
         "Unit": Literal["METERS"],
         "Value": float,
     },
 )
 
-_RequiredPlatformInputOutputTypeDef = TypedDict(
-    "_RequiredPlatformInputOutputTypeDef",
-    {
-        "Value": str,
-    },
-)
-_OptionalPlatformInputOutputTypeDef = TypedDict(
-    "_OptionalPlatformInputOutputTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-    total=False,
-)
-
-class PlatformInputOutputTypeDef(
-    _RequiredPlatformInputOutputTypeDef, _OptionalPlatformInputOutputTypeDef
-):
-    pass
-
 _RequiredPlatformInputTypeDef = TypedDict(
     "_RequiredPlatformInputTypeDef",
     {
         "Value": str,
     },
 )
 _OptionalPlatformInputTypeDef = TypedDict(
@@ -809,38 +679,14 @@
     },
     total=False,
 )
 
 class PlatformInputTypeDef(_RequiredPlatformInputTypeDef, _OptionalPlatformInputTypeDef):
     pass
 
-ViewOffNadirInputOutputTypeDef = TypedDict(
-    "ViewOffNadirInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
-ViewSunAzimuthInputOutputTypeDef = TypedDict(
-    "ViewSunAzimuthInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
-ViewSunElevationInputOutputTypeDef = TypedDict(
-    "ViewSunElevationInputOutputTypeDef",
-    {
-        "LowerBound": float,
-        "UpperBound": float,
-    },
-)
-
 ViewOffNadirInputTypeDef = TypedDict(
     "ViewOffNadirInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -873,22 +719,14 @@
     "TimeRangeFilterOutputTypeDef",
     {
         "EndTime": datetime,
         "StartTime": datetime,
     },
 )
 
-ReverseGeocodingConfigOutputTypeDef = TypedDict(
-    "ReverseGeocodingConfigOutputTypeDef",
-    {
-        "XAttributeName": str,
-        "YAttributeName": str,
-    },
-)
-
 ReverseGeocodingConfigTypeDef = TypedDict(
     "ReverseGeocodingConfigTypeDef",
     {
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
@@ -940,15 +778,15 @@
     },
     total=False,
 )
 
 CustomIndicesInputOutputTypeDef = TypedDict(
     "CustomIndicesInputOutputTypeDef",
     {
-        "Operations": List[OperationOutputTypeDef],
+        "Operations": List[OperationTypeDef],
     },
     total=False,
 )
 
 CustomIndicesInputTypeDef = TypedDict(
     "CustomIndicesInputTypeDef",
     {
@@ -978,43 +816,21 @@
     {
         "ExportResults": ExportErrorDetailsOutputTypeDef,
         "ExportSourceImages": ExportErrorDetailsOutputTypeDef,
     },
     total=False,
 )
 
-OutputConfigInputOutputTypeDef = TypedDict(
-    "OutputConfigInputOutputTypeDef",
-    {
-        "S3Data": ExportS3DataInputOutputTypeDef,
-    },
-)
-
 OutputConfigInputTypeDef = TypedDict(
     "OutputConfigInputTypeDef",
     {
         "S3Data": ExportS3DataInputTypeDef,
     },
 )
 
-ExportVectorEnrichmentJobOutputConfigOutputTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
-    {
-        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
-    },
-)
-
-VectorEnrichmentJobDataSourceConfigInputOutputTypeDef = TypedDict(
-    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
-    {
-        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
-    },
-    total=False,
-)
-
 ExportVectorEnrichmentJobOutputConfigTypeDef = TypedDict(
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     {
         "S3Data": VectorEnrichmentJobS3DataTypeDef,
     },
 )
 
@@ -1129,30 +945,14 @@
     {
         "NextToken": str,
         "VectorEnrichmentJobSummaries": List[ListVectorEnrichmentJobOutputConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OutputResolutionResamplingInputOutputTypeDef = TypedDict(
-    "OutputResolutionResamplingInputOutputTypeDef",
-    {
-        "UserDefined": UserDefinedOutputTypeDef,
-    },
-)
-
-OutputResolutionStackInputOutputTypeDef = TypedDict(
-    "OutputResolutionStackInputOutputTypeDef",
-    {
-        "Predefined": PredefinedResolutionType,
-        "UserDefined": UserDefinedOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputResolutionResamplingInputTypeDef = TypedDict(
     "OutputResolutionResamplingInputTypeDef",
     {
         "UserDefined": UserDefinedTypeDef,
     },
 )
 
@@ -1161,49 +961,27 @@
     {
         "Predefined": PredefinedResolutionType,
         "UserDefined": UserDefinedTypeDef,
     },
     total=False,
 )
 
-PropertyOutputTypeDef = TypedDict(
-    "PropertyOutputTypeDef",
-    {
-        "EoCloudCover": EoCloudCoverInputOutputTypeDef,
-        "LandsatCloudCoverLand": LandsatCloudCoverLandInputOutputTypeDef,
-        "Platform": PlatformInputOutputTypeDef,
-        "ViewOffNadir": ViewOffNadirInputOutputTypeDef,
-        "ViewSunAzimuth": ViewSunAzimuthInputOutputTypeDef,
-        "ViewSunElevation": ViewSunElevationInputOutputTypeDef,
-    },
-    total=False,
-)
-
 PropertyTypeDef = TypedDict(
     "PropertyTypeDef",
     {
         "EoCloudCover": EoCloudCoverInputTypeDef,
         "LandsatCloudCoverLand": LandsatCloudCoverLandInputTypeDef,
         "Platform": PlatformInputTypeDef,
         "ViewOffNadir": ViewOffNadirInputTypeDef,
         "ViewSunAzimuth": ViewSunAzimuthInputTypeDef,
         "ViewSunElevation": ViewSunElevationInputTypeDef,
     },
     total=False,
 )
 
-VectorEnrichmentJobConfigOutputTypeDef = TypedDict(
-    "VectorEnrichmentJobConfigOutputTypeDef",
-    {
-        "MapMatchingConfig": MapMatchingConfigOutputTypeDef,
-        "ReverseGeocodingConfig": ReverseGeocodingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 VectorEnrichmentJobConfigTypeDef = TypedDict(
     "VectorEnrichmentJobConfigTypeDef",
     {
         "MapMatchingConfig": MapMatchingConfigTypeDef,
         "ReverseGeocodingConfig": ReverseGeocodingConfigTypeDef,
     },
     total=False,
@@ -1239,27 +1017,14 @@
     {
         "CustomIndices": CustomIndicesInputTypeDef,
         "PredefinedIndices": Sequence[str],
     },
     total=False,
 )
 
-ExportEarthObservationJobOutputTypeDef = TypedDict(
-    "ExportEarthObservationJobOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionRoleArn": str,
-        "ExportSourceImages": bool,
-        "ExportStatus": EarthObservationJobExportStatusType,
-        "OutputConfig": OutputConfigInputOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredExportEarthObservationJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": OutputConfigInputTypeDef,
     },
@@ -1275,34 +1040,27 @@
 
 class ExportEarthObservationJobInputRequestTypeDef(
     _RequiredExportEarthObservationJobInputRequestTypeDef,
     _OptionalExportEarthObservationJobInputRequestTypeDef,
 ):
     pass
 
-ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobOutputTypeDef",
+ExportEarthObservationJobOutputTypeDef = TypedDict(
+    "ExportEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
-        "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "OutputConfig": ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+        "ExportSourceImages": bool,
+        "ExportStatus": EarthObservationJobExportStatusType,
+        "OutputConfig": OutputConfigInputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VectorEnrichmentJobInputConfigOutputTypeDef = TypedDict(
-    "VectorEnrichmentJobInputConfigOutputTypeDef",
-    {
-        "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
-        "DocumentType": Literal["CSV"],
-    },
-)
-
 _RequiredExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
     },
@@ -1317,14 +1075,26 @@
 
 class ExportVectorEnrichmentJobInputRequestTypeDef(
     _RequiredExportVectorEnrichmentJobInputRequestTypeDef,
     _OptionalExportVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
+ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "ExportVectorEnrichmentJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionRoleArn": str,
+        "ExportStatus": VectorEnrichmentJobExportStatusType,
+        "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VectorEnrichmentJobInputConfigTypeDef = TypedDict(
     "VectorEnrichmentJobInputConfigTypeDef",
     {
         "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputTypeDef,
         "DocumentType": Literal["CSV"],
     },
 )
@@ -1347,15 +1117,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResamplingConfigInputOutputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputOutputTypeDef",
     {
-        "OutputResolution": OutputResolutionResamplingInputOutputTypeDef,
+        "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputOutputTypeDef = TypedDict(
     "_OptionalResamplingConfigInputOutputTypeDef",
     {
         "AlgorithmName": AlgorithmNameResamplingType,
         "TargetBands": List[str],
@@ -1364,23 +1134,14 @@
 )
 
 class ResamplingConfigInputOutputTypeDef(
     _RequiredResamplingConfigInputOutputTypeDef, _OptionalResamplingConfigInputOutputTypeDef
 ):
     pass
 
-StackConfigInputOutputTypeDef = TypedDict(
-    "StackConfigInputOutputTypeDef",
-    {
-        "OutputResolution": OutputResolutionStackInputOutputTypeDef,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputTypeDef = TypedDict(
@@ -1393,28 +1154,30 @@
 )
 
 class ResamplingConfigInputTypeDef(
     _RequiredResamplingConfigInputTypeDef, _OptionalResamplingConfigInputTypeDef
 ):
     pass
 
-StackConfigInputTypeDef = TypedDict(
-    "StackConfigInputTypeDef",
+StackConfigInputOutputTypeDef = TypedDict(
+    "StackConfigInputOutputTypeDef",
     {
         "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
-PropertyFilterOutputTypeDef = TypedDict(
-    "PropertyFilterOutputTypeDef",
+StackConfigInputTypeDef = TypedDict(
+    "StackConfigInputTypeDef",
     {
-        "Property": PropertyOutputTypeDef,
+        "OutputResolution": OutputResolutionStackInputTypeDef,
+        "TargetBands": Sequence[str],
     },
+    total=False,
 )
 
 PropertyFilterTypeDef = TypedDict(
     "PropertyFilterTypeDef",
     {
         "Property": PropertyTypeDef,
     },
@@ -1426,34 +1189,16 @@
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": VectorEnrichmentJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": VectorEnrichmentJobExportErrorDetailsTypeDef,
         "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
-        "KmsKeyId": str,
-        "Name": str,
-        "Status": VectorEnrichmentJobStatusType,
-        "Tags": Dict[str, str],
-        "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "StartVectorEnrichmentJobOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "DurationInSeconds": int,
-        "ExecutionRoleArn": str,
-        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
+        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1480,14 +1225,32 @@
 
 class StartVectorEnrichmentJobInputRequestTypeDef(
     _RequiredStartVectorEnrichmentJobInputRequestTypeDef,
     _OptionalStartVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
+StartVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "StartVectorEnrichmentJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "DurationInSeconds": int,
+        "ExecutionRoleArn": str,
+        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigTypeDef,
+        "KmsKeyId": str,
+        "Name": str,
+        "Status": VectorEnrichmentJobStatusType,
+        "Tags": Dict[str, str],
+        "Type": VectorEnrichmentJobTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 JobConfigInputOutputTypeDef = TypedDict(
     "JobConfigInputOutputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputOutputTypeDef,
         "CloudMaskingConfig": Dict[str, Any],
         "CloudRemovalConfig": CloudRemovalConfigInputOutputTypeDef,
         "GeoMosaicConfig": GeoMosaicConfigInputOutputTypeDef,
@@ -1516,15 +1279,15 @@
     total=False,
 )
 
 PropertyFiltersOutputTypeDef = TypedDict(
     "PropertyFiltersOutputTypeDef",
     {
         "LogicalOperator": Literal["AND"],
-        "Properties": List[PropertyFilterOutputTypeDef],
+        "Properties": List[PropertyFilterTypeDef],
     },
     total=False,
 )
 
 PropertyFiltersTypeDef = TypedDict(
     "PropertyFiltersTypeDef",
     {
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.28.15/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sagemaker-geospatial
-Version: 1.28.12
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,26 +333,22 @@
     MultiPolygonGeometryInputOutputTypeDef,
     PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
     AssetValueTypeDef,
     CloudRemovalConfigInputOutputTypeDef,
     CloudRemovalConfigInputTypeDef,
-    OperationOutputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
-    EoCloudCoverInputOutputTypeDef,
     EoCloudCoverInputTypeDef,
     ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
-    ExportS3DataInputOutputTypeDef,
     ExportS3DataInputTypeDef,
-    VectorEnrichmentJobS3DataOutputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
     GeoMosaicConfigInputOutputTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
@@ -394,93 +358,76 @@
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
     TemporalStatisticsConfigInputOutputTypeDef,
     ZonalStatisticsConfigInputOutputTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
-    LandsatCloudCoverLandInputOutputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
     PaginatorConfigTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
-    MapMatchingConfigOutputTypeDef,
     MapMatchingConfigTypeDef,
-    UserDefinedOutputTypeDef,
     UserDefinedTypeDef,
-    PlatformInputOutputTypeDef,
     PlatformInputTypeDef,
-    ViewOffNadirInputOutputTypeDef,
-    ViewSunAzimuthInputOutputTypeDef,
-    ViewSunElevationInputOutputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
-    ReverseGeocodingConfigOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
     GetTileOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
-    OutputConfigInputOutputTypeDef,
     OutputConfigInputTypeDef,
-    ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
-    VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
     ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
     ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
-    OutputResolutionResamplingInputOutputTypeDef,
-    OutputResolutionStackInputOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
-    PropertyOutputTypeDef,
     PropertyTypeDef,
-    VectorEnrichmentJobConfigOutputTypeDef,
     VectorEnrichmentJobConfigTypeDef,
     AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
     BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
-    ExportEarthObservationJobOutputTypeDef,
     ExportEarthObservationJobInputRequestTypeDef,
-    ExportVectorEnrichmentJobOutputTypeDef,
-    VectorEnrichmentJobInputConfigOutputTypeDef,
+    ExportEarthObservationJobOutputTypeDef,
     ExportVectorEnrichmentJobInputRequestTypeDef,
+    ExportVectorEnrichmentJobOutputTypeDef,
     VectorEnrichmentJobInputConfigTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
     ResamplingConfigInputOutputTypeDef,
-    StackConfigInputOutputTypeDef,
     ResamplingConfigInputTypeDef,
+    StackConfigInputOutputTypeDef,
     StackConfigInputTypeDef,
-    PropertyFilterOutputTypeDef,
     PropertyFilterTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
-    StartVectorEnrichmentJobOutputTypeDef,
     StartVectorEnrichmentJobInputRequestTypeDef,
+    StartVectorEnrichmentJobOutputTypeDef,
     JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
     PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
     RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-geospatial-1.28.15/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.12/setup.py` & `mypy-boto3-sagemaker-geospatial-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-geospatial",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

