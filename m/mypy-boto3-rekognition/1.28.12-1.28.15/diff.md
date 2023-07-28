# Comparing `tmp/mypy-boto3-rekognition-1.28.12.tar.gz` & `tmp/mypy-boto3-rekognition-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
```

## Comparing `mypy-boto3-rekognition-1.28.12.tar` & `mypy-boto3-rekognition-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-07-27 11:44:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-07-27 11:44:29.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-27 11:44:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   101004 2023-07-27 11:44:33.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100883 2023-07-27 11:44:32.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.773728 mypy-boto3-rekognition-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-07-28 20:43:33.769728 mypy-boto3-rekognition-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.761727 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98431 2023-07-28 20:36:51.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98310 2023-07-28 20:36:49.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.769728 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.773728 mypy-boto3-rekognition-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/setup.py
```

### Comparing `mypy-boto3-rekognition-1.28.12/LICENSE` & `mypy-boto3-rekognition-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/PKG-INFO` & `mypy-boto3-rekognition-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.12
-Summary: Type annotations for boto3.Rekognition 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -431,19 +431,18 @@
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
     ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
-    BoundingBoxOutputTypeDef,
-    S3ObjectOutputTypeDef,
+    BoundingBoxTypeDef,
+    S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
-    BoundingBoxTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
@@ -474,16 +473,14 @@
     DescribeCollectionRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
-    StreamProcessorDataSharingPreferenceOutputTypeDef,
-    StreamProcessorNotificationChannelOutputTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
@@ -496,35 +493,32 @@
     EyeOpenTypeDef,
     EyeglassesTypeDef,
     FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
-    FaceSearchSettingsOutputTypeDef,
     FaceSearchSettingsTypeDef,
-    PointOutputTypeDef,
+    PointTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
     GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
     GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
     GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
-    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
-    KinesisVideoStreamOutputTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
@@ -535,16 +529,14 @@
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    OutputConfigOutputTypeDef,
-    PointTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
@@ -582,17 +574,18 @@
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
     StopProjectVersionResponseTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
-    GroundTruthManifestOutputTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
     SummaryTypeDef,
-    VideoOutputTypeDef,
+    VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
@@ -622,85 +615,83 @@
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestOutputTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
-    VideoTypeDef,
+    RegionOfInterestTypeDef,
     HumanLoopConfigTypeDef,
-    StreamProcessorInputOutputTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
     UserMatchTypeDef,
-    RegionOfInterestTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
-    AssetOutputTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
     EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
     StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    SearchUsersByImageRequestRequestTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    DetectModerationLabelsRequestRequestTypeDef,
-    StartStreamProcessorRequestRequestTypeDef,
-    SearchUsersResponseTypeDef,
     DetectTextFiltersTypeDef,
     StartTextDetectionFiltersTypeDef,
     UpdateStreamProcessorRequestRequestTypeDef,
+    DetectModerationLabelsRequestRequestTypeDef,
+    StartStreamProcessorRequestRequestTypeDef,
+    SearchUsersResponseTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     TestingDataOutputTypeDef,
+    TestingDataTypeDef,
     TrainingDataOutputTypeDef,
+    TrainingDataTypeDef,
     ValidationDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
@@ -708,28 +699,25 @@
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-rekognition-1.28.12/README.md` & `mypy-boto3-rekognition-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,19 +399,18 @@
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
     ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
-    BoundingBoxOutputTypeDef,
-    S3ObjectOutputTypeDef,
+    BoundingBoxTypeDef,
+    S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
-    BoundingBoxTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
@@ -442,16 +441,14 @@
     DescribeCollectionRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
-    StreamProcessorDataSharingPreferenceOutputTypeDef,
-    StreamProcessorNotificationChannelOutputTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
@@ -464,35 +461,32 @@
     EyeOpenTypeDef,
     EyeglassesTypeDef,
     FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
-    FaceSearchSettingsOutputTypeDef,
     FaceSearchSettingsTypeDef,
-    PointOutputTypeDef,
+    PointTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
     GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
     GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
     GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
-    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
-    KinesisVideoStreamOutputTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
@@ -503,16 +497,14 @@
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    OutputConfigOutputTypeDef,
-    PointTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
@@ -550,17 +542,18 @@
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
     StopProjectVersionResponseTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
-    GroundTruthManifestOutputTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
     SummaryTypeDef,
-    VideoOutputTypeDef,
+    VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
@@ -590,85 +583,83 @@
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestOutputTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
-    VideoTypeDef,
+    RegionOfInterestTypeDef,
     HumanLoopConfigTypeDef,
-    StreamProcessorInputOutputTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
     UserMatchTypeDef,
-    RegionOfInterestTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
-    AssetOutputTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
     EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
     StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    SearchUsersByImageRequestRequestTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    DetectModerationLabelsRequestRequestTypeDef,
-    StartStreamProcessorRequestRequestTypeDef,
-    SearchUsersResponseTypeDef,
     DetectTextFiltersTypeDef,
     StartTextDetectionFiltersTypeDef,
     UpdateStreamProcessorRequestRequestTypeDef,
+    DetectModerationLabelsRequestRequestTypeDef,
+    StartStreamProcessorRequestRequestTypeDef,
+    SearchUsersResponseTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     TestingDataOutputTypeDef,
+    TestingDataTypeDef,
     TrainingDataOutputTypeDef,
+    TrainingDataTypeDef,
     ValidationDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
@@ -676,28 +667,25 @@
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Rekognition 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,18 @@
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
-    "BoundingBoxOutputTypeDef",
-    "S3ObjectOutputTypeDef",
+    "BoundingBoxTypeDef",
+    "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
-    "BoundingBoxTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
@@ -114,16 +113,14 @@
     "DescribeCollectionRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
-    "StreamProcessorDataSharingPreferenceOutputTypeDef",
-    "StreamProcessorNotificationChannelOutputTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ProtectiveEquipmentSummarizationAttributesTypeDef",
     "ProtectiveEquipmentSummaryTypeDef",
@@ -136,35 +133,32 @@
     "EyeOpenTypeDef",
     "EyeglassesTypeDef",
     "FaceOccludedTypeDef",
     "GenderTypeDef",
     "MouthOpenTypeDef",
     "MustacheTypeDef",
     "SunglassesTypeDef",
-    "FaceSearchSettingsOutputTypeDef",
     "FaceSearchSettingsTypeDef",
-    "PointOutputTypeDef",
+    "PointTypeDef",
     "GetCelebrityInfoRequestRequestTypeDef",
     "GetCelebrityRecognitionRequestRequestTypeDef",
     "VideoMetadataTypeDef",
     "GetContentModerationRequestMetadataTypeDef",
     "GetContentModerationRequestRequestTypeDef",
     "GetFaceDetectionRequestRequestTypeDef",
     "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     "GetFaceSearchRequestRequestTypeDef",
     "GetLabelDetectionRequestMetadataTypeDef",
     "GetLabelDetectionRequestRequestTypeDef",
     "GetPersonTrackingRequestRequestTypeDef",
     "GetSegmentDetectionRequestRequestTypeDef",
     "SegmentTypeInfoTypeDef",
     "GetTextDetectionRequestRequestTypeDef",
-    "S3ObjectTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
-    "KinesisVideoStreamOutputTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
@@ -175,16 +169,14 @@
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
-    "OutputConfigOutputTypeDef",
-    "PointTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchedFaceTypeDef",
     "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
@@ -222,17 +214,18 @@
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
     "StopProjectVersionResponseTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
-    "GroundTruthManifestOutputTypeDef",
+    "GroundTruthManifestTypeDef",
+    "ImageTypeDef",
     "SummaryTypeDef",
-    "VideoOutputTypeDef",
+    "VideoTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
@@ -262,85 +255,83 @@
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
     "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
     "RegionOfInterestOutputTypeDef",
-    "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
-    "VideoTypeDef",
+    "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
-    "StreamProcessorInputOutputTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
     "UserMatchTypeDef",
-    "RegionOfInterestTypeDef",
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
-    "AssetOutputTypeDef",
+    "AssetTypeDef",
+    "DatasetSourceTypeDef",
+    "CompareFacesRequestRequestTypeDef",
+    "DetectCustomLabelsRequestRequestTypeDef",
+    "DetectFacesRequestRequestTypeDef",
+    "DetectProtectiveEquipmentRequestRequestTypeDef",
+    "IndexFacesRequestRequestTypeDef",
+    "RecognizeCelebritiesRequestRequestTypeDef",
+    "SearchFacesByImageRequestRequestTypeDef",
+    "SearchUsersByImageRequestRequestTypeDef",
     "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
     "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
     "DescribeProjectsResponseTypeDef",
     "DetectLabelsImagePropertiesTypeDef",
     "LabelTypeDef",
+    "DetectLabelsRequestRequestTypeDef",
+    "StartLabelDetectionRequestRequestTypeDef",
     "CelebrityDetailTypeDef",
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
-    "AssetTypeDef",
-    "DatasetSourceTypeDef",
-    "CompareFacesRequestRequestTypeDef",
-    "DetectCustomLabelsRequestRequestTypeDef",
-    "DetectFacesRequestRequestTypeDef",
-    "DetectLabelsRequestRequestTypeDef",
-    "DetectProtectiveEquipmentRequestRequestTypeDef",
-    "IndexFacesRequestRequestTypeDef",
-    "RecognizeCelebritiesRequestRequestTypeDef",
-    "SearchFacesByImageRequestRequestTypeDef",
-    "SearchUsersByImageRequestRequestTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartLabelDetectionRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
-    "DetectModerationLabelsRequestRequestTypeDef",
-    "StartStreamProcessorRequestRequestTypeDef",
-    "SearchUsersResponseTypeDef",
     "DetectTextFiltersTypeDef",
     "StartTextDetectionFiltersTypeDef",
     "UpdateStreamProcessorRequestRequestTypeDef",
+    "DetectModerationLabelsRequestRequestTypeDef",
+    "StartStreamProcessorRequestRequestTypeDef",
+    "SearchUsersResponseTypeDef",
     "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
     "TestingDataOutputTypeDef",
+    "TestingDataTypeDef",
     "TrainingDataOutputTypeDef",
+    "TrainingDataTypeDef",
     "ValidationDataTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
     "DetectLabelsResponseTypeDef",
     "LabelDetectionTypeDef",
     "CelebrityRecognitionTypeDef",
@@ -348,28 +339,25 @@
     "PersonDetectionTypeDef",
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
-    "TestingDataTypeDef",
-    "TrainingDataTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DetectTextRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
+    "CreateProjectVersionRequestRequestTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
     "GetTextDetectionResponseTypeDef",
-    "CreateProjectVersionRequestRequestTypeDef",
     "ProjectVersionDescriptionTypeDef",
     "DescribeProjectVersionsResponseTypeDef",
 )
 
 AgeRangeTypeDef = TypedDict(
     "AgeRangeTypeDef",
     {
@@ -440,27 +428,27 @@
         "DurationMillis": int,
         "SampleRate": int,
         "NumberOfChannels": int,
     },
     total=False,
 )
 
-BoundingBoxOutputTypeDef = TypedDict(
-    "BoundingBoxOutputTypeDef",
+BoundingBoxTypeDef = TypedDict(
+    "BoundingBoxTypeDef",
     {
         "Width": float,
         "Height": float,
         "Left": float,
         "Top": float,
     },
     total=False,
 )
 
-S3ObjectOutputTypeDef = TypedDict(
-    "S3ObjectOutputTypeDef",
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
     {
         "Bucket": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
@@ -479,25 +467,14 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
-BoundingBoxTypeDef = TypedDict(
-    "BoundingBoxTypeDef",
-    {
-        "Width": float,
-        "Height": float,
-        "Left": float,
-        "Top": float,
-    },
-    total=False,
-)
-
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -921,28 +898,14 @@
 DescribeStreamProcessorRequestRequestTypeDef = TypedDict(
     "DescribeStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-StreamProcessorDataSharingPreferenceOutputTypeDef = TypedDict(
-    "StreamProcessorDataSharingPreferenceOutputTypeDef",
-    {
-        "OptIn": bool,
-    },
-)
-
-StreamProcessorNotificationChannelOutputTypeDef = TypedDict(
-    "StreamProcessorNotificationChannelOutputTypeDef",
-    {
-        "SNSTopicArn": str,
-    },
-)
-
 DetectLabelsImageQualityTypeDef = TypedDict(
     "DetectLabelsImageQualityTypeDef",
     {
         "Brightness": float,
         "Sharpness": float,
         "Contrast": float,
     },
@@ -1137,34 +1100,25 @@
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
 )
 
-FaceSearchSettingsOutputTypeDef = TypedDict(
-    "FaceSearchSettingsOutputTypeDef",
-    {
-        "CollectionId": str,
-        "FaceMatchThreshold": float,
-    },
-    total=False,
-)
-
 FaceSearchSettingsTypeDef = TypedDict(
     "FaceSearchSettingsTypeDef",
     {
         "CollectionId": str,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
-PointOutputTypeDef = TypedDict(
-    "PointOutputTypeDef",
+PointTypeDef = TypedDict(
+    "PointTypeDef",
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
@@ -1405,24 +1359,14 @@
 
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
-    {
-        "Bucket": str,
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1431,22 +1375,14 @@
     "KinesisDataStreamTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-KinesisVideoStreamOutputTypeDef = TypedDict(
-    "KinesisVideoStreamOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 KinesisVideoStreamStartSelectorTypeDef = TypedDict(
     "KinesisVideoStreamStartSelectorTypeDef",
     {
         "ProducerTimestamp": int,
         "FragmentNumber": str,
     },
     total=False,
@@ -1671,32 +1607,14 @@
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
 )
 
-OutputConfigOutputTypeDef = TypedDict(
-    "OutputConfigOutputTypeDef",
-    {
-        "S3Bucket": str,
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-PointTypeDef = TypedDict(
-    "PointTypeDef",
-    {
-        "X": float,
-        "Y": float,
-    },
-    total=False,
-)
-
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyDocument": str,
     },
@@ -2101,64 +2019,73 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedSourceImageFaceTypeDef = TypedDict(
     "ComparedSourceImageFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
     },
     total=False,
 )
 
 FaceTypeDef = TypedDict(
     "FaceTypeDef",
     {
         "FaceId": str,
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "ImageId": str,
         "ExternalImageId": str,
         "Confidence": float,
         "IndexFacesModelVersion": str,
         "UserId": str,
     },
     total=False,
 )
 
 AuditImageTypeDef = TypedDict(
     "AuditImageTypeDef",
     {
         "Bytes": bytes,
-        "S3Object": S3ObjectOutputTypeDef,
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
     },
     total=False,
 )
 
-GroundTruthManifestOutputTypeDef = TypedDict(
-    "GroundTruthManifestOutputTypeDef",
+GroundTruthManifestTypeDef = TypedDict(
+    "GroundTruthManifestTypeDef",
+    {
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
-        "S3Object": S3ObjectOutputTypeDef,
+        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
-        "S3Object": S3ObjectOutputTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-VideoOutputTypeDef = TypedDict(
-    "VideoOutputTypeDef",
+VideoTypeDef = TypedDict(
+    "VideoTypeDef",
     {
-        "S3Object": S3ObjectOutputTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 StartTechnicalCueDetectionFilterTypeDef = TypedDict(
     "StartTechnicalCueDetectionFilterTypeDef",
     {
@@ -2177,15 +2104,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Landmarks": List[LandmarkTypeDef],
         "Pose": PoseTypeDef,
         "Quality": ImageQualityTypeDef,
         "Emotions": List[EmotionTypeDef],
         "Smile": SmileTypeDef,
     },
@@ -2238,15 +2165,15 @@
 ):
     pass
 
 
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
     },
     total=False,
 )
 
@@ -2540,15 +2467,15 @@
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
 )
 
 DetectLabelsSettingsTypeDef = TypedDict(
@@ -2594,15 +2521,15 @@
         "Datasets": Sequence[DistributeDatasetTypeDef],
     },
 )
 
 FaceDetailTypeDef = TypedDict(
     "FaceDetailTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "AgeRange": AgeRangeTypeDef,
         "Smile": SmileTypeDef,
         "Eyeglasses": EyeglassesTypeDef,
         "Sunglasses": SunglassesTypeDef,
         "Gender": GenderTypeDef,
         "Beard": BeardTypeDef,
         "Mustache": MustacheTypeDef,
@@ -2618,15 +2545,15 @@
     },
     total=False,
 )
 
 StreamProcessorSettingsOutputTypeDef = TypedDict(
     "StreamProcessorSettingsOutputTypeDef",
     {
-        "FaceSearch": FaceSearchSettingsOutputTypeDef,
+        "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
     },
     total=False,
 )
 
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
@@ -2636,50 +2563,34 @@
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Polygon": List[PointOutputTypeDef],
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
 RegionOfInterestOutputTypeDef = TypedDict(
     "RegionOfInterestOutputTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Polygon": List[PointOutputTypeDef],
-    },
-    total=False,
-)
-
-GroundTruthManifestTypeDef = TypedDict(
-    "GroundTruthManifestTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-VideoTypeDef = TypedDict(
-    "VideoTypeDef",
+RegionOfInterestTypeDef = TypedDict(
+    "RegionOfInterestTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": Sequence[PointTypeDef],
     },
     total=False,
 )
 
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
@@ -2696,22 +2607,14 @@
 )
 
 
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
 
-StreamProcessorInputOutputTypeDef = TypedDict(
-    "StreamProcessorInputOutputTypeDef",
-    {
-        "KinesisVideoStream": KinesisVideoStreamOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2756,23 +2659,14 @@
     {
         "Similarity": float,
         "User": MatchedUserTypeDef,
     },
     total=False,
 )
 
-RegionOfInterestTypeDef = TypedDict(
-    "RegionOfInterestTypeDef",
-    {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": Sequence[PointTypeDef],
-    },
-    total=False,
-)
-
 StreamProcessorOutputTypeDef = TypedDict(
     "StreamProcessorOutputTypeDef",
     {
         "KinesisDataStream": KinesisDataStreamTypeDef,
         "S3Destination": S3DestinationTypeDef,
     },
     total=False,
@@ -2824,249 +2718,14 @@
         "Confidence": float,
         "ReferenceImage": AuditImageTypeDef,
         "AuditImages": List[AuditImageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssetOutputTypeDef = TypedDict(
-    "AssetOutputTypeDef",
-    {
-        "GroundTruthManifest": GroundTruthManifestOutputTypeDef,
-    },
-    total=False,
-)
-
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
-CelebrityTypeDef = TypedDict(
-    "CelebrityTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Face": ComparedFaceTypeDef,
-        "MatchConfidence": float,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-CompareFacesMatchTypeDef = TypedDict(
-    "CompareFacesMatchTypeDef",
-    {
-        "Similarity": float,
-        "Face": ComparedFaceTypeDef,
-    },
-    total=False,
-)
-
-GetContentModerationResponseTypeDef = TypedDict(
-    "GetContentModerationResponseTypeDef",
-    {
-        "JobStatus": VideoJobStatusType,
-        "StatusMessage": str,
-        "VideoMetadata": VideoMetadataTypeDef,
-        "ModerationLabels": List[ContentModerationDetectionTypeDef],
-        "NextToken": str,
-        "ModerationModelVersion": str,
-        "JobId": str,
-        "Video": VideoOutputTypeDef,
-        "JobTag": str,
-        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProtectiveEquipmentBodyPartTypeDef = TypedDict(
-    "ProtectiveEquipmentBodyPartTypeDef",
-    {
-        "Name": BodyPartType,
-        "Confidence": float,
-        "EquipmentDetections": List[EquipmentDetectionTypeDef],
-    },
-    total=False,
-)
-
-CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
-    "CreateFaceLivenessSessionRequestRequestTypeDef",
-    {
-        "KmsKeyId": str,
-        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatasetLabelsResponseTypeDef = TypedDict(
-    "ListDatasetLabelsResponseTypeDef",
-    {
-        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeProjectsResponseTypeDef = TypedDict(
-    "DescribeProjectsResponseTypeDef",
-    {
-        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectLabelsImagePropertiesTypeDef = TypedDict(
-    "DetectLabelsImagePropertiesTypeDef",
-    {
-        "Quality": DetectLabelsImageQualityTypeDef,
-        "DominantColors": List[DominantColorTypeDef],
-        "Foreground": DetectLabelsImageForegroundTypeDef,
-        "Background": DetectLabelsImageBackgroundTypeDef,
-    },
-    total=False,
-)
-
-LabelTypeDef = TypedDict(
-    "LabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Instances": List[InstanceTypeDef],
-        "Parents": List[ParentTypeDef],
-        "Aliases": List[LabelAliasTypeDef],
-        "Categories": List[LabelCategoryTypeDef],
-    },
-    total=False,
-)
-
-CelebrityDetailTypeDef = TypedDict(
-    "CelebrityDetailTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Confidence": float,
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Face": FaceDetailTypeDef,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-DetectFacesResponseTypeDef = TypedDict(
-    "DetectFacesResponseTypeDef",
-    {
-        "FaceDetails": List[FaceDetailTypeDef],
-        "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-FaceDetectionTypeDef = TypedDict(
-    "FaceDetectionTypeDef",
-    {
-        "Timestamp": int,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-FaceRecordTypeDef = TypedDict(
-    "FaceRecordTypeDef",
-    {
-        "Face": FaceTypeDef,
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-PersonDetailTypeDef = TypedDict(
-    "PersonDetailTypeDef",
-    {
-        "Index": int,
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-SearchedFaceDetailsTypeDef = TypedDict(
-    "SearchedFaceDetailsTypeDef",
-    {
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-UnindexedFaceTypeDef = TypedDict(
-    "UnindexedFaceTypeDef",
-    {
-        "Reasons": List[ReasonType],
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-UnsearchedFaceTypeDef = TypedDict(
-    "UnsearchedFaceTypeDef",
-    {
-        "FaceDetails": FaceDetailTypeDef,
-        "Reasons": List[UnsearchedFaceReasonType],
-    },
-    total=False,
-)
-
-CustomLabelTypeDef = TypedDict(
-    "CustomLabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-TextDetectionTypeDef = TypedDict(
-    "TextDetectionTypeDef",
-    {
-        "DetectedText": str,
-        "Type": TextTypesType,
-        "Id": int,
-        "ParentId": int,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
     },
     total=False,
 )
@@ -3144,38 +2803,14 @@
 
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectLabelsRequestRequestTypeDef",
-    {
-        "MaxLabels": int,
-        "MinConfidence": float,
-        "Features": Sequence[DetectLabelsFeatureNameType],
-        "Settings": DetectLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class DetectLabelsRequestRequestTypeDef(
-    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
@@ -3272,14 +2907,23 @@
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
 
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
@@ -3371,122 +3015,307 @@
 
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartLabelDetectionRequestRequestTypeDef",
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
-_OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartLabelDetectionRequestRequestTypeDef",
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
-        "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
-        "Features": Sequence[Literal["GENERAL_LABELS"]],
-        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
 
-class StartLabelDetectionRequestRequestTypeDef(
-    _RequiredStartLabelDetectionRequestRequestTypeDef,
-    _OptionalStartLabelDetectionRequestRequestTypeDef,
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+CelebrityTypeDef = TypedDict(
+    "CelebrityTypeDef",
     {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Face": ComparedFaceTypeDef,
+        "MatchConfidence": float,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+CompareFacesMatchTypeDef = TypedDict(
+    "CompareFacesMatchTypeDef",
+    {
+        "Similarity": float,
+        "Face": ComparedFaceTypeDef,
+    },
+    total=False,
+)
+
+GetContentModerationResponseTypeDef = TypedDict(
+    "GetContentModerationResponseTypeDef",
+    {
+        "JobStatus": VideoJobStatusType,
+        "StatusMessage": str,
+        "VideoMetadata": VideoMetadataTypeDef,
+        "ModerationLabels": List[ContentModerationDetectionTypeDef],
+        "NextToken": str,
+        "ModerationModelVersion": str,
+        "JobId": str,
         "Video": VideoTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+
+ProtectiveEquipmentBodyPartTypeDef = TypedDict(
+    "ProtectiveEquipmentBodyPartTypeDef",
     {
+        "Name": BodyPartType,
+        "Confidence": float,
+        "EquipmentDetections": List[EquipmentDetectionTypeDef],
+    },
+    total=False,
+)
+
+CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
+    {
+        "KmsKeyId": str,
+        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
         "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
     },
     total=False,
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetDescription": DatasetDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
+ListDatasetLabelsResponseTypeDef = TypedDict(
+    "ListDatasetLabelsResponseTypeDef",
+    {
+        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+DescribeProjectsResponseTypeDef = TypedDict(
+    "DescribeProjectsResponseTypeDef",
+    {
+        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
+DetectLabelsImagePropertiesTypeDef = TypedDict(
+    "DetectLabelsImagePropertiesTypeDef",
+    {
+        "Quality": DetectLabelsImageQualityTypeDef,
+        "DominantColors": List[DominantColorTypeDef],
+        "Foreground": DetectLabelsImageForegroundTypeDef,
+        "Background": DetectLabelsImageBackgroundTypeDef,
+    },
+    total=False,
+)
+
+LabelTypeDef = TypedDict(
+    "LabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Instances": List[InstanceTypeDef],
+        "Parents": List[ParentTypeDef],
+        "Aliases": List[LabelAliasTypeDef],
+        "Categories": List[LabelCategoryTypeDef],
+    },
+    total=False,
+)
+
+_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
-_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
+_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectLabelsRequestRequestTypeDef",
     {
+        "MaxLabels": int,
         "MinConfidence": float,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
+        "Features": Sequence[DetectLabelsFeatureNameType],
+        "Settings": DetectLabelsSettingsTypeDef,
     },
     total=False,
 )
 
 
-class DetectModerationLabelsRequestRequestTypeDef(
-    _RequiredDetectModerationLabelsRequestRequestTypeDef,
-    _OptionalDetectModerationLabelsRequestRequestTypeDef,
+class DetectLabelsRequestRequestTypeDef(
+    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredStartStreamProcessorRequestRequestTypeDef",
+_RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
-        "Name": str,
+        "Video": VideoTypeDef,
     },
 )
-_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalStartStreamProcessorRequestRequestTypeDef",
+_OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
-        "StartSelector": StreamProcessingStartSelectorTypeDef,
-        "StopSelector": StreamProcessingStopSelectorTypeDef,
+        "ClientRequestToken": str,
+        "MinConfidence": float,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+        "Features": Sequence[Literal["GENERAL_LABELS"]],
+        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
 
-class StartStreamProcessorRequestRequestTypeDef(
-    _RequiredStartStreamProcessorRequestRequestTypeDef,
-    _OptionalStartStreamProcessorRequestRequestTypeDef,
+class StartLabelDetectionRequestRequestTypeDef(
+    _RequiredStartLabelDetectionRequestRequestTypeDef,
+    _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
 
-SearchUsersResponseTypeDef = TypedDict(
-    "SearchUsersResponseTypeDef",
+CelebrityDetailTypeDef = TypedDict(
+    "CelebrityDetailTypeDef",
     {
-        "UserMatches": List[UserMatchTypeDef],
-        "FaceModelVersion": str,
-        "SearchedFace": SearchedFaceTypeDef,
-        "SearchedUser": SearchedUserTypeDef,
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Confidence": float,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+DetectFacesResponseTypeDef = TypedDict(
+    "DetectFacesResponseTypeDef",
+    {
+        "FaceDetails": List[FaceDetailTypeDef],
+        "OrientationCorrection": OrientationCorrectionType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FaceDetectionTypeDef = TypedDict(
+    "FaceDetectionTypeDef",
+    {
+        "Timestamp": int,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+FaceRecordTypeDef = TypedDict(
+    "FaceRecordTypeDef",
+    {
+        "Face": FaceTypeDef,
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+PersonDetailTypeDef = TypedDict(
+    "PersonDetailTypeDef",
+    {
+        "Index": int,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+SearchedFaceDetailsTypeDef = TypedDict(
+    "SearchedFaceDetailsTypeDef",
+    {
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnindexedFaceTypeDef = TypedDict(
+    "UnindexedFaceTypeDef",
+    {
+        "Reasons": List[ReasonType],
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnsearchedFaceTypeDef = TypedDict(
+    "UnsearchedFaceTypeDef",
+    {
+        "FaceDetails": FaceDetailTypeDef,
+        "Reasons": List[UnsearchedFaceReasonType],
+    },
+    total=False,
+)
+
+CustomLabelTypeDef = TypedDict(
+    "CustomLabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+TextDetectionTypeDef = TypedDict(
+    "TextDetectionTypeDef",
+    {
+        "DetectedText": str,
+        "Type": TextTypesType,
+        "Id": int,
+        "ParentId": int,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
 DetectTextFiltersTypeDef = TypedDict(
     "DetectTextFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
@@ -3522,14 +3351,71 @@
 class UpdateStreamProcessorRequestRequestTypeDef(
     _RequiredUpdateStreamProcessorRequestRequestTypeDef,
     _OptionalUpdateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
+    {
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
+    {
+        "MinConfidence": float,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DetectModerationLabelsRequestRequestTypeDef(
+    _RequiredDetectModerationLabelsRequestRequestTypeDef,
+    _OptionalDetectModerationLabelsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredStartStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalStartStreamProcessorRequestRequestTypeDef",
+    {
+        "StartSelector": StreamProcessingStartSelectorTypeDef,
+        "StopSelector": StreamProcessingStopSelectorTypeDef,
+    },
+    total=False,
+)
+
+
+class StartStreamProcessorRequestRequestTypeDef(
+    _RequiredStartStreamProcessorRequestRequestTypeDef,
+    _OptionalStartStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
+    {
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceTypeDef,
+        "SearchedUser": SearchedUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamProcessorRequestRequestTypeDef",
     {
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "Name": str,
         "Settings": StreamProcessorSettingsTypeDef,
@@ -3561,22 +3447,22 @@
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
-        "Input": StreamProcessorInputOutputTypeDef,
+        "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
         "Settings": StreamProcessorSettingsOutputTypeDef,
-        "NotificationChannel": StreamProcessorNotificationChannelOutputTypeDef,
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
         "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceOutputTypeDef,
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
@@ -3584,24 +3470,24 @@
         "StatusMessage": str,
         "VideoMetadata": List[VideoMetadataTypeDef],
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesByImageResponseTypeDef = TypedDict(
     "SearchFacesByImageResponseTypeDef",
     {
-        "SearchedFaceBoundingBox": BoundingBoxOutputTypeDef,
+        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
         "SearchedFaceConfidence": float,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3614,36 +3500,75 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestingDataOutputTypeDef = TypedDict(
     "TestingDataOutputTypeDef",
     {
-        "Assets": List[AssetOutputTypeDef],
+        "Assets": List[AssetTypeDef],
+        "AutoCreate": bool,
+    },
+    total=False,
+)
+
+TestingDataTypeDef = TypedDict(
+    "TestingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
 TrainingDataOutputTypeDef = TypedDict(
     "TrainingDataOutputTypeDef",
     {
-        "Assets": List[AssetOutputTypeDef],
+        "Assets": List[AssetTypeDef],
+    },
+    total=False,
+)
+
+TrainingDataTypeDef = TypedDict(
+    "TrainingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
 
 ValidationDataTypeDef = TypedDict(
     "ValidationDataTypeDef",
     {
-        "Assets": List[AssetOutputTypeDef],
+        "Assets": List[AssetTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "ProjectArn": str,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetSource": DatasetSourceTypeDef,
     },
     total=False,
 )
 
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -3688,15 +3613,15 @@
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Id": int,
     },
     total=False,
 )
 
 DetectLabelsResponseTypeDef = TypedDict(
@@ -3736,15 +3661,15 @@
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
@@ -3809,53 +3734,14 @@
     {
         "Timestamp": int,
         "TextDetection": TextDetectionTypeDef,
     },
     total=False,
 )
 
-TestingDataTypeDef = TypedDict(
-    "TestingDataTypeDef",
-    {
-        "Assets": Sequence[AssetTypeDef],
-        "AutoCreate": bool,
-    },
-    total=False,
-)
-
-TrainingDataTypeDef = TypedDict(
-    "TrainingDataTypeDef",
-    {
-        "Assets": Sequence[AssetTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "ProjectArn": str,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetSource": DatasetSourceTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredDetectTextRequestRequestTypeDef = TypedDict(
     "_RequiredDetectTextRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectTextRequestRequestTypeDef = TypedDict(
@@ -3894,14 +3780,41 @@
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectVersionRequestRequestTypeDef",
+    {
+        "ProjectArn": str,
+        "VersionName": str,
+        "OutputConfig": OutputConfigTypeDef,
+    },
+)
+_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectVersionRequestRequestTypeDef",
+    {
+        "TrainingData": TrainingDataTypeDef,
+        "TestingData": TestingDataTypeDef,
+        "Tags": Mapping[str, str],
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class CreateProjectVersionRequestRequestTypeDef(
+    _RequiredCreateProjectVersionRequestRequestTypeDef,
+    _OptionalCreateProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
         "Input": TestingDataOutputTypeDef,
         "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
@@ -3934,15 +3847,15 @@
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
@@ -3950,45 +3863,45 @@
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
@@ -3996,62 +3909,35 @@
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectArn": str,
-        "VersionName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectVersionRequestRequestTypeDef",
-    {
-        "TrainingData": TrainingDataTypeDef,
-        "TestingData": TestingDataTypeDef,
-        "Tags": Mapping[str, str],
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class CreateProjectVersionRequestRequestTypeDef(
-    _RequiredCreateProjectVersionRequestRequestTypeDef,
-    _OptionalCreateProjectVersionRequestRequestTypeDef,
-):
-    pass
-
-
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
         "CreationTimestamp": datetime,
         "MinInferenceUnits": int,
         "Status": ProjectVersionStatusType,
         "StatusMessage": str,
         "BillableTrainingTimeInSeconds": int,
         "TrainingEndTimestamp": datetime,
-        "OutputConfig": OutputConfigOutputTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
         "TrainingDataResult": TrainingDataResultTypeDef,
         "TestingDataResult": TestingDataResultTypeDef,
         "EvaluationResult": EvaluationResultTypeDef,
-        "ManifestSummary": GroundTruthManifestOutputTypeDef,
+        "ManifestSummary": GroundTruthManifestTypeDef,
         "KmsKeyId": str,
         "MaxInferenceUnits": int,
         "SourceProjectVersionArn": str,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,18 @@
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
-    "BoundingBoxOutputTypeDef",
-    "S3ObjectOutputTypeDef",
+    "BoundingBoxTypeDef",
+    "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
-    "BoundingBoxTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
@@ -113,16 +112,14 @@
     "DescribeCollectionRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
-    "StreamProcessorDataSharingPreferenceOutputTypeDef",
-    "StreamProcessorNotificationChannelOutputTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ProtectiveEquipmentSummarizationAttributesTypeDef",
     "ProtectiveEquipmentSummaryTypeDef",
@@ -135,35 +132,32 @@
     "EyeOpenTypeDef",
     "EyeglassesTypeDef",
     "FaceOccludedTypeDef",
     "GenderTypeDef",
     "MouthOpenTypeDef",
     "MustacheTypeDef",
     "SunglassesTypeDef",
-    "FaceSearchSettingsOutputTypeDef",
     "FaceSearchSettingsTypeDef",
-    "PointOutputTypeDef",
+    "PointTypeDef",
     "GetCelebrityInfoRequestRequestTypeDef",
     "GetCelebrityRecognitionRequestRequestTypeDef",
     "VideoMetadataTypeDef",
     "GetContentModerationRequestMetadataTypeDef",
     "GetContentModerationRequestRequestTypeDef",
     "GetFaceDetectionRequestRequestTypeDef",
     "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     "GetFaceSearchRequestRequestTypeDef",
     "GetLabelDetectionRequestMetadataTypeDef",
     "GetLabelDetectionRequestRequestTypeDef",
     "GetPersonTrackingRequestRequestTypeDef",
     "GetSegmentDetectionRequestRequestTypeDef",
     "SegmentTypeInfoTypeDef",
     "GetTextDetectionRequestRequestTypeDef",
-    "S3ObjectTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
-    "KinesisVideoStreamOutputTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
@@ -174,16 +168,14 @@
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
-    "OutputConfigOutputTypeDef",
-    "PointTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchedFaceTypeDef",
     "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
@@ -221,17 +213,18 @@
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
     "StopProjectVersionResponseTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
-    "GroundTruthManifestOutputTypeDef",
+    "GroundTruthManifestTypeDef",
+    "ImageTypeDef",
     "SummaryTypeDef",
-    "VideoOutputTypeDef",
+    "VideoTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
@@ -261,85 +254,83 @@
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
     "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
     "RegionOfInterestOutputTypeDef",
-    "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
-    "VideoTypeDef",
+    "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
-    "StreamProcessorInputOutputTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
     "UserMatchTypeDef",
-    "RegionOfInterestTypeDef",
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
-    "AssetOutputTypeDef",
+    "AssetTypeDef",
+    "DatasetSourceTypeDef",
+    "CompareFacesRequestRequestTypeDef",
+    "DetectCustomLabelsRequestRequestTypeDef",
+    "DetectFacesRequestRequestTypeDef",
+    "DetectProtectiveEquipmentRequestRequestTypeDef",
+    "IndexFacesRequestRequestTypeDef",
+    "RecognizeCelebritiesRequestRequestTypeDef",
+    "SearchFacesByImageRequestRequestTypeDef",
+    "SearchUsersByImageRequestRequestTypeDef",
     "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
     "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
     "DescribeProjectsResponseTypeDef",
     "DetectLabelsImagePropertiesTypeDef",
     "LabelTypeDef",
+    "DetectLabelsRequestRequestTypeDef",
+    "StartLabelDetectionRequestRequestTypeDef",
     "CelebrityDetailTypeDef",
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
-    "AssetTypeDef",
-    "DatasetSourceTypeDef",
-    "CompareFacesRequestRequestTypeDef",
-    "DetectCustomLabelsRequestRequestTypeDef",
-    "DetectFacesRequestRequestTypeDef",
-    "DetectLabelsRequestRequestTypeDef",
-    "DetectProtectiveEquipmentRequestRequestTypeDef",
-    "IndexFacesRequestRequestTypeDef",
-    "RecognizeCelebritiesRequestRequestTypeDef",
-    "SearchFacesByImageRequestRequestTypeDef",
-    "SearchUsersByImageRequestRequestTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartLabelDetectionRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
-    "DetectModerationLabelsRequestRequestTypeDef",
-    "StartStreamProcessorRequestRequestTypeDef",
-    "SearchUsersResponseTypeDef",
     "DetectTextFiltersTypeDef",
     "StartTextDetectionFiltersTypeDef",
     "UpdateStreamProcessorRequestRequestTypeDef",
+    "DetectModerationLabelsRequestRequestTypeDef",
+    "StartStreamProcessorRequestRequestTypeDef",
+    "SearchUsersResponseTypeDef",
     "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
     "TestingDataOutputTypeDef",
+    "TestingDataTypeDef",
     "TrainingDataOutputTypeDef",
+    "TrainingDataTypeDef",
     "ValidationDataTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
     "DetectLabelsResponseTypeDef",
     "LabelDetectionTypeDef",
     "CelebrityRecognitionTypeDef",
@@ -347,28 +338,25 @@
     "PersonDetectionTypeDef",
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
-    "TestingDataTypeDef",
-    "TrainingDataTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DetectTextRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
+    "CreateProjectVersionRequestRequestTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
     "GetTextDetectionResponseTypeDef",
-    "CreateProjectVersionRequestRequestTypeDef",
     "ProjectVersionDescriptionTypeDef",
     "DescribeProjectVersionsResponseTypeDef",
 )
 
 AgeRangeTypeDef = TypedDict(
     "AgeRangeTypeDef",
     {
@@ -437,27 +425,27 @@
         "DurationMillis": int,
         "SampleRate": int,
         "NumberOfChannels": int,
     },
     total=False,
 )
 
-BoundingBoxOutputTypeDef = TypedDict(
-    "BoundingBoxOutputTypeDef",
+BoundingBoxTypeDef = TypedDict(
+    "BoundingBoxTypeDef",
     {
         "Width": float,
         "Height": float,
         "Left": float,
         "Top": float,
     },
     total=False,
 )
 
-S3ObjectOutputTypeDef = TypedDict(
-    "S3ObjectOutputTypeDef",
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
     {
         "Bucket": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
@@ -476,25 +464,14 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
-BoundingBoxTypeDef = TypedDict(
-    "BoundingBoxTypeDef",
-    {
-        "Width": float,
-        "Height": float,
-        "Left": float,
-        "Top": float,
-    },
-    total=False,
-)
-
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -902,28 +879,14 @@
 DescribeStreamProcessorRequestRequestTypeDef = TypedDict(
     "DescribeStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-StreamProcessorDataSharingPreferenceOutputTypeDef = TypedDict(
-    "StreamProcessorDataSharingPreferenceOutputTypeDef",
-    {
-        "OptIn": bool,
-    },
-)
-
-StreamProcessorNotificationChannelOutputTypeDef = TypedDict(
-    "StreamProcessorNotificationChannelOutputTypeDef",
-    {
-        "SNSTopicArn": str,
-    },
-)
-
 DetectLabelsImageQualityTypeDef = TypedDict(
     "DetectLabelsImageQualityTypeDef",
     {
         "Brightness": float,
         "Sharpness": float,
         "Contrast": float,
     },
@@ -1116,34 +1079,25 @@
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
 )
 
-FaceSearchSettingsOutputTypeDef = TypedDict(
-    "FaceSearchSettingsOutputTypeDef",
-    {
-        "CollectionId": str,
-        "FaceMatchThreshold": float,
-    },
-    total=False,
-)
-
 FaceSearchSettingsTypeDef = TypedDict(
     "FaceSearchSettingsTypeDef",
     {
         "CollectionId": str,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
-PointOutputTypeDef = TypedDict(
-    "PointOutputTypeDef",
+PointTypeDef = TypedDict(
+    "PointTypeDef",
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
@@ -1368,24 +1322,14 @@
 )
 
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
-    {
-        "Bucket": str,
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1394,22 +1338,14 @@
     "KinesisDataStreamTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-KinesisVideoStreamOutputTypeDef = TypedDict(
-    "KinesisVideoStreamOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 KinesisVideoStreamStartSelectorTypeDef = TypedDict(
     "KinesisVideoStreamStartSelectorTypeDef",
     {
         "ProducerTimestamp": int,
         "FragmentNumber": str,
     },
     total=False,
@@ -1624,32 +1560,14 @@
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
 )
 
-OutputConfigOutputTypeDef = TypedDict(
-    "OutputConfigOutputTypeDef",
-    {
-        "S3Bucket": str,
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-PointTypeDef = TypedDict(
-    "PointTypeDef",
-    {
-        "X": float,
-        "Y": float,
-    },
-    total=False,
-)
-
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyDocument": str,
     },
@@ -2046,64 +1964,73 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedSourceImageFaceTypeDef = TypedDict(
     "ComparedSourceImageFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
     },
     total=False,
 )
 
 FaceTypeDef = TypedDict(
     "FaceTypeDef",
     {
         "FaceId": str,
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "ImageId": str,
         "ExternalImageId": str,
         "Confidence": float,
         "IndexFacesModelVersion": str,
         "UserId": str,
     },
     total=False,
 )
 
 AuditImageTypeDef = TypedDict(
     "AuditImageTypeDef",
     {
         "Bytes": bytes,
-        "S3Object": S3ObjectOutputTypeDef,
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+    },
+    total=False,
+)
+
+GroundTruthManifestTypeDef = TypedDict(
+    "GroundTruthManifestTypeDef",
+    {
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-GroundTruthManifestOutputTypeDef = TypedDict(
-    "GroundTruthManifestOutputTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
-        "S3Object": S3ObjectOutputTypeDef,
+        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
-        "S3Object": S3ObjectOutputTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
-VideoOutputTypeDef = TypedDict(
-    "VideoOutputTypeDef",
+VideoTypeDef = TypedDict(
+    "VideoTypeDef",
     {
-        "S3Object": S3ObjectOutputTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 StartTechnicalCueDetectionFilterTypeDef = TypedDict(
     "StartTechnicalCueDetectionFilterTypeDef",
     {
@@ -2122,15 +2049,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Landmarks": List[LandmarkTypeDef],
         "Pose": PoseTypeDef,
         "Quality": ImageQualityTypeDef,
         "Emotions": List[EmotionTypeDef],
         "Smile": SmileTypeDef,
     },
@@ -2181,15 +2108,15 @@
     _OptionalCopyProjectVersionRequestRequestTypeDef,
 ):
     pass
 
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
     },
     total=False,
 )
 
@@ -2467,15 +2394,15 @@
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
 )
 
 DetectLabelsSettingsTypeDef = TypedDict(
@@ -2521,15 +2448,15 @@
         "Datasets": Sequence[DistributeDatasetTypeDef],
     },
 )
 
 FaceDetailTypeDef = TypedDict(
     "FaceDetailTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "AgeRange": AgeRangeTypeDef,
         "Smile": SmileTypeDef,
         "Eyeglasses": EyeglassesTypeDef,
         "Sunglasses": SunglassesTypeDef,
         "Gender": GenderTypeDef,
         "Beard": BeardTypeDef,
         "Mustache": MustacheTypeDef,
@@ -2545,15 +2472,15 @@
     },
     total=False,
 )
 
 StreamProcessorSettingsOutputTypeDef = TypedDict(
     "StreamProcessorSettingsOutputTypeDef",
     {
-        "FaceSearch": FaceSearchSettingsOutputTypeDef,
+        "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
     },
     total=False,
 )
 
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
@@ -2563,50 +2490,34 @@
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Polygon": List[PointOutputTypeDef],
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
 RegionOfInterestOutputTypeDef = TypedDict(
     "RegionOfInterestOutputTypeDef",
     {
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Polygon": List[PointOutputTypeDef],
-    },
-    total=False,
-)
-
-GroundTruthManifestTypeDef = TypedDict(
-    "GroundTruthManifestTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-VideoTypeDef = TypedDict(
-    "VideoTypeDef",
+RegionOfInterestTypeDef = TypedDict(
+    "RegionOfInterestTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": Sequence[PointTypeDef],
     },
     total=False,
 )
 
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
@@ -2621,22 +2532,14 @@
     },
     total=False,
 )
 
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
-StreamProcessorInputOutputTypeDef = TypedDict(
-    "StreamProcessorInputOutputTypeDef",
-    {
-        "KinesisVideoStream": KinesisVideoStreamOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2681,23 +2584,14 @@
     {
         "Similarity": float,
         "User": MatchedUserTypeDef,
     },
     total=False,
 )
 
-RegionOfInterestTypeDef = TypedDict(
-    "RegionOfInterestTypeDef",
-    {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": Sequence[PointTypeDef],
-    },
-    total=False,
-)
-
 StreamProcessorOutputTypeDef = TypedDict(
     "StreamProcessorOutputTypeDef",
     {
         "KinesisDataStream": KinesisDataStreamTypeDef,
         "S3Destination": S3DestinationTypeDef,
     },
     total=False,
@@ -2749,249 +2643,14 @@
         "Confidence": float,
         "ReferenceImage": AuditImageTypeDef,
         "AuditImages": List[AuditImageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssetOutputTypeDef = TypedDict(
-    "AssetOutputTypeDef",
-    {
-        "GroundTruthManifest": GroundTruthManifestOutputTypeDef,
-    },
-    total=False,
-)
-
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
-CelebrityTypeDef = TypedDict(
-    "CelebrityTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Face": ComparedFaceTypeDef,
-        "MatchConfidence": float,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-CompareFacesMatchTypeDef = TypedDict(
-    "CompareFacesMatchTypeDef",
-    {
-        "Similarity": float,
-        "Face": ComparedFaceTypeDef,
-    },
-    total=False,
-)
-
-GetContentModerationResponseTypeDef = TypedDict(
-    "GetContentModerationResponseTypeDef",
-    {
-        "JobStatus": VideoJobStatusType,
-        "StatusMessage": str,
-        "VideoMetadata": VideoMetadataTypeDef,
-        "ModerationLabels": List[ContentModerationDetectionTypeDef],
-        "NextToken": str,
-        "ModerationModelVersion": str,
-        "JobId": str,
-        "Video": VideoOutputTypeDef,
-        "JobTag": str,
-        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProtectiveEquipmentBodyPartTypeDef = TypedDict(
-    "ProtectiveEquipmentBodyPartTypeDef",
-    {
-        "Name": BodyPartType,
-        "Confidence": float,
-        "EquipmentDetections": List[EquipmentDetectionTypeDef],
-    },
-    total=False,
-)
-
-CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
-    "CreateFaceLivenessSessionRequestRequestTypeDef",
-    {
-        "KmsKeyId": str,
-        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatasetLabelsResponseTypeDef = TypedDict(
-    "ListDatasetLabelsResponseTypeDef",
-    {
-        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeProjectsResponseTypeDef = TypedDict(
-    "DescribeProjectsResponseTypeDef",
-    {
-        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectLabelsImagePropertiesTypeDef = TypedDict(
-    "DetectLabelsImagePropertiesTypeDef",
-    {
-        "Quality": DetectLabelsImageQualityTypeDef,
-        "DominantColors": List[DominantColorTypeDef],
-        "Foreground": DetectLabelsImageForegroundTypeDef,
-        "Background": DetectLabelsImageBackgroundTypeDef,
-    },
-    total=False,
-)
-
-LabelTypeDef = TypedDict(
-    "LabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Instances": List[InstanceTypeDef],
-        "Parents": List[ParentTypeDef],
-        "Aliases": List[LabelAliasTypeDef],
-        "Categories": List[LabelCategoryTypeDef],
-    },
-    total=False,
-)
-
-CelebrityDetailTypeDef = TypedDict(
-    "CelebrityDetailTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Confidence": float,
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Face": FaceDetailTypeDef,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-DetectFacesResponseTypeDef = TypedDict(
-    "DetectFacesResponseTypeDef",
-    {
-        "FaceDetails": List[FaceDetailTypeDef],
-        "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-FaceDetectionTypeDef = TypedDict(
-    "FaceDetectionTypeDef",
-    {
-        "Timestamp": int,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-FaceRecordTypeDef = TypedDict(
-    "FaceRecordTypeDef",
-    {
-        "Face": FaceTypeDef,
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-PersonDetailTypeDef = TypedDict(
-    "PersonDetailTypeDef",
-    {
-        "Index": int,
-        "BoundingBox": BoundingBoxOutputTypeDef,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-SearchedFaceDetailsTypeDef = TypedDict(
-    "SearchedFaceDetailsTypeDef",
-    {
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-UnindexedFaceTypeDef = TypedDict(
-    "UnindexedFaceTypeDef",
-    {
-        "Reasons": List[ReasonType],
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-UnsearchedFaceTypeDef = TypedDict(
-    "UnsearchedFaceTypeDef",
-    {
-        "FaceDetails": FaceDetailTypeDef,
-        "Reasons": List[UnsearchedFaceReasonType],
-    },
-    total=False,
-)
-
-CustomLabelTypeDef = TypedDict(
-    "CustomLabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-TextDetectionTypeDef = TypedDict(
-    "TextDetectionTypeDef",
-    {
-        "DetectedText": str,
-        "Type": TextTypesType,
-        "Id": int,
-        "ParentId": int,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
     },
     total=False,
 )
@@ -3063,36 +2722,14 @@
 )
 
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
-_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectLabelsRequestRequestTypeDef",
-    {
-        "MaxLabels": int,
-        "MinConfidence": float,
-        "Features": Sequence[DetectLabelsFeatureNameType],
-        "Settings": DetectLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
-class DetectLabelsRequestRequestTypeDef(
-    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
-):
-    pass
-
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
@@ -3181,14 +2818,23 @@
 
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
@@ -3272,114 +2918,301 @@
 )
 
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartLabelDetectionRequestRequestTypeDef",
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
-_OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartLabelDetectionRequestRequestTypeDef",
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
-        "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
-        "Features": Sequence[Literal["GENERAL_LABELS"]],
-        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
-class StartLabelDetectionRequestRequestTypeDef(
-    _RequiredStartLabelDetectionRequestRequestTypeDef,
-    _OptionalStartLabelDetectionRequestRequestTypeDef,
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+CelebrityTypeDef = TypedDict(
+    "CelebrityTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Face": ComparedFaceTypeDef,
+        "MatchConfidence": float,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+CompareFacesMatchTypeDef = TypedDict(
+    "CompareFacesMatchTypeDef",
     {
+        "Similarity": float,
+        "Face": ComparedFaceTypeDef,
+    },
+    total=False,
+)
+
+GetContentModerationResponseTypeDef = TypedDict(
+    "GetContentModerationResponseTypeDef",
+    {
+        "JobStatus": VideoJobStatusType,
+        "StatusMessage": str,
+        "VideoMetadata": VideoMetadataTypeDef,
+        "ModerationLabels": List[ContentModerationDetectionTypeDef],
+        "NextToken": str,
+        "ModerationModelVersion": str,
+        "JobId": str,
         "Video": VideoTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+
+ProtectiveEquipmentBodyPartTypeDef = TypedDict(
+    "ProtectiveEquipmentBodyPartTypeDef",
     {
+        "Name": BodyPartType,
+        "Confidence": float,
+        "EquipmentDetections": List[EquipmentDetectionTypeDef],
+    },
+    total=False,
+)
+
+CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
+    {
+        "KmsKeyId": str,
+        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
         "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
     },
     total=False,
 )
 
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetDescription": DatasetDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
+ListDatasetLabelsResponseTypeDef = TypedDict(
+    "ListDatasetLabelsResponseTypeDef",
+    {
+        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProjectsResponseTypeDef = TypedDict(
+    "DescribeProjectsResponseTypeDef",
+    {
+        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectLabelsImagePropertiesTypeDef = TypedDict(
+    "DetectLabelsImagePropertiesTypeDef",
+    {
+        "Quality": DetectLabelsImageQualityTypeDef,
+        "DominantColors": List[DominantColorTypeDef],
+        "Foreground": DetectLabelsImageForegroundTypeDef,
+        "Background": DetectLabelsImageBackgroundTypeDef,
+    },
+    total=False,
+)
+
+LabelTypeDef = TypedDict(
+    "LabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Instances": List[InstanceTypeDef],
+        "Parents": List[ParentTypeDef],
+        "Aliases": List[LabelAliasTypeDef],
+        "Categories": List[LabelCategoryTypeDef],
+    },
+    total=False,
+)
+
+_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
-_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
+_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectLabelsRequestRequestTypeDef",
     {
+        "MaxLabels": int,
         "MinConfidence": float,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
+        "Features": Sequence[DetectLabelsFeatureNameType],
+        "Settings": DetectLabelsSettingsTypeDef,
     },
     total=False,
 )
 
-class DetectModerationLabelsRequestRequestTypeDef(
-    _RequiredDetectModerationLabelsRequestRequestTypeDef,
-    _OptionalDetectModerationLabelsRequestRequestTypeDef,
+class DetectLabelsRequestRequestTypeDef(
+    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredStartStreamProcessorRequestRequestTypeDef",
+_RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
-        "Name": str,
+        "Video": VideoTypeDef,
     },
 )
-_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalStartStreamProcessorRequestRequestTypeDef",
+_OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
-        "StartSelector": StreamProcessingStartSelectorTypeDef,
-        "StopSelector": StreamProcessingStopSelectorTypeDef,
+        "ClientRequestToken": str,
+        "MinConfidence": float,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+        "Features": Sequence[Literal["GENERAL_LABELS"]],
+        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
-class StartStreamProcessorRequestRequestTypeDef(
-    _RequiredStartStreamProcessorRequestRequestTypeDef,
-    _OptionalStartStreamProcessorRequestRequestTypeDef,
+class StartLabelDetectionRequestRequestTypeDef(
+    _RequiredStartLabelDetectionRequestRequestTypeDef,
+    _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
-SearchUsersResponseTypeDef = TypedDict(
-    "SearchUsersResponseTypeDef",
+CelebrityDetailTypeDef = TypedDict(
+    "CelebrityDetailTypeDef",
     {
-        "UserMatches": List[UserMatchTypeDef],
-        "FaceModelVersion": str,
-        "SearchedFace": SearchedFaceTypeDef,
-        "SearchedUser": SearchedUserTypeDef,
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Confidence": float,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+DetectFacesResponseTypeDef = TypedDict(
+    "DetectFacesResponseTypeDef",
+    {
+        "FaceDetails": List[FaceDetailTypeDef],
+        "OrientationCorrection": OrientationCorrectionType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FaceDetectionTypeDef = TypedDict(
+    "FaceDetectionTypeDef",
+    {
+        "Timestamp": int,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+FaceRecordTypeDef = TypedDict(
+    "FaceRecordTypeDef",
+    {
+        "Face": FaceTypeDef,
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+PersonDetailTypeDef = TypedDict(
+    "PersonDetailTypeDef",
+    {
+        "Index": int,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+SearchedFaceDetailsTypeDef = TypedDict(
+    "SearchedFaceDetailsTypeDef",
+    {
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnindexedFaceTypeDef = TypedDict(
+    "UnindexedFaceTypeDef",
+    {
+        "Reasons": List[ReasonType],
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnsearchedFaceTypeDef = TypedDict(
+    "UnsearchedFaceTypeDef",
+    {
+        "FaceDetails": FaceDetailTypeDef,
+        "Reasons": List[UnsearchedFaceReasonType],
+    },
+    total=False,
+)
+
+CustomLabelTypeDef = TypedDict(
+    "CustomLabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+TextDetectionTypeDef = TypedDict(
+    "TextDetectionTypeDef",
+    {
+        "DetectedText": str,
+        "Type": TextTypesType,
+        "Id": int,
+        "ParentId": int,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
 DetectTextFiltersTypeDef = TypedDict(
     "DetectTextFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
@@ -3413,14 +3246,67 @@
 
 class UpdateStreamProcessorRequestRequestTypeDef(
     _RequiredUpdateStreamProcessorRequestRequestTypeDef,
     _OptionalUpdateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
+    {
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
+    {
+        "MinConfidence": float,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
+    },
+    total=False,
+)
+
+class DetectModerationLabelsRequestRequestTypeDef(
+    _RequiredDetectModerationLabelsRequestRequestTypeDef,
+    _OptionalDetectModerationLabelsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredStartStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalStartStreamProcessorRequestRequestTypeDef",
+    {
+        "StartSelector": StreamProcessingStartSelectorTypeDef,
+        "StopSelector": StreamProcessingStopSelectorTypeDef,
+    },
+    total=False,
+)
+
+class StartStreamProcessorRequestRequestTypeDef(
+    _RequiredStartStreamProcessorRequestRequestTypeDef,
+    _OptionalStartStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
+    {
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceTypeDef,
+        "SearchedUser": SearchedUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamProcessorRequestRequestTypeDef",
     {
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "Name": str,
         "Settings": StreamProcessorSettingsTypeDef,
@@ -3450,22 +3336,22 @@
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
-        "Input": StreamProcessorInputOutputTypeDef,
+        "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
         "Settings": StreamProcessorSettingsOutputTypeDef,
-        "NotificationChannel": StreamProcessorNotificationChannelOutputTypeDef,
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
         "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceOutputTypeDef,
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
@@ -3473,24 +3359,24 @@
         "StatusMessage": str,
         "VideoMetadata": List[VideoMetadataTypeDef],
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesByImageResponseTypeDef = TypedDict(
     "SearchFacesByImageResponseTypeDef",
     {
-        "SearchedFaceBoundingBox": BoundingBoxOutputTypeDef,
+        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
         "SearchedFaceConfidence": float,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3503,36 +3389,73 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestingDataOutputTypeDef = TypedDict(
     "TestingDataOutputTypeDef",
     {
-        "Assets": List[AssetOutputTypeDef],
+        "Assets": List[AssetTypeDef],
+        "AutoCreate": bool,
+    },
+    total=False,
+)
+
+TestingDataTypeDef = TypedDict(
+    "TestingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
 TrainingDataOutputTypeDef = TypedDict(
     "TrainingDataOutputTypeDef",
     {
-        "Assets": List[AssetOutputTypeDef],
+        "Assets": List[AssetTypeDef],
+    },
+    total=False,
+)
+
+TrainingDataTypeDef = TypedDict(
+    "TrainingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
 
 ValidationDataTypeDef = TypedDict(
     "ValidationDataTypeDef",
     {
-        "Assets": List[AssetOutputTypeDef],
+        "Assets": List[AssetTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "ProjectArn": str,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetSource": DatasetSourceTypeDef,
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -3575,15 +3498,15 @@
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
-        "BoundingBox": BoundingBoxOutputTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Id": int,
     },
     total=False,
 )
 
 DetectLabelsResponseTypeDef = TypedDict(
@@ -3623,15 +3546,15 @@
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
@@ -3696,51 +3619,14 @@
     {
         "Timestamp": int,
         "TextDetection": TextDetectionTypeDef,
     },
     total=False,
 )
 
-TestingDataTypeDef = TypedDict(
-    "TestingDataTypeDef",
-    {
-        "Assets": Sequence[AssetTypeDef],
-        "AutoCreate": bool,
-    },
-    total=False,
-)
-
-TrainingDataTypeDef = TypedDict(
-    "TrainingDataTypeDef",
-    {
-        "Assets": Sequence[AssetTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "ProjectArn": str,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetSource": DatasetSourceTypeDef,
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
 _RequiredDetectTextRequestRequestTypeDef = TypedDict(
     "_RequiredDetectTextRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectTextRequestRequestTypeDef = TypedDict(
@@ -3775,14 +3661,39 @@
 
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectVersionRequestRequestTypeDef",
+    {
+        "ProjectArn": str,
+        "VersionName": str,
+        "OutputConfig": OutputConfigTypeDef,
+    },
+)
+_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectVersionRequestRequestTypeDef",
+    {
+        "TrainingData": TrainingDataTypeDef,
+        "TestingData": TestingDataTypeDef,
+        "Tags": Mapping[str, str],
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class CreateProjectVersionRequestRequestTypeDef(
+    _RequiredCreateProjectVersionRequestRequestTypeDef,
+    _OptionalCreateProjectVersionRequestRequestTypeDef,
+):
+    pass
+
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
         "Input": TestingDataOutputTypeDef,
         "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
@@ -3815,15 +3726,15 @@
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
@@ -3831,45 +3742,45 @@
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
@@ -3877,60 +3788,35 @@
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
         "JobId": str,
-        "Video": VideoOutputTypeDef,
+        "Video": VideoTypeDef,
         "JobTag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectArn": str,
-        "VersionName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectVersionRequestRequestTypeDef",
-    {
-        "TrainingData": TrainingDataTypeDef,
-        "TestingData": TestingDataTypeDef,
-        "Tags": Mapping[str, str],
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class CreateProjectVersionRequestRequestTypeDef(
-    _RequiredCreateProjectVersionRequestRequestTypeDef,
-    _OptionalCreateProjectVersionRequestRequestTypeDef,
-):
-    pass
-
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
         "CreationTimestamp": datetime,
         "MinInferenceUnits": int,
         "Status": ProjectVersionStatusType,
         "StatusMessage": str,
         "BillableTrainingTimeInSeconds": int,
         "TrainingEndTimestamp": datetime,
-        "OutputConfig": OutputConfigOutputTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
         "TrainingDataResult": TrainingDataResultTypeDef,
         "TestingDataResult": TestingDataResultTypeDef,
         "EvaluationResult": EvaluationResultTypeDef,
-        "ManifestSummary": GroundTruthManifestOutputTypeDef,
+        "ManifestSummary": GroundTruthManifestTypeDef,
         "KmsKeyId": str,
         "MaxInferenceUnits": int,
         "SourceProjectVersionArn": str,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.12
-Summary: Type annotations for boto3.Rekognition 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -431,19 +431,18 @@
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
     ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
-    BoundingBoxOutputTypeDef,
-    S3ObjectOutputTypeDef,
+    BoundingBoxTypeDef,
+    S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
-    BoundingBoxTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
@@ -474,16 +473,14 @@
     DescribeCollectionRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
-    StreamProcessorDataSharingPreferenceOutputTypeDef,
-    StreamProcessorNotificationChannelOutputTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
@@ -496,35 +493,32 @@
     EyeOpenTypeDef,
     EyeglassesTypeDef,
     FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
-    FaceSearchSettingsOutputTypeDef,
     FaceSearchSettingsTypeDef,
-    PointOutputTypeDef,
+    PointTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
     GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
     GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
     GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
-    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
-    KinesisVideoStreamOutputTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
@@ -535,16 +529,14 @@
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    OutputConfigOutputTypeDef,
-    PointTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
@@ -582,17 +574,18 @@
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
     StopProjectVersionResponseTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
-    GroundTruthManifestOutputTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
     SummaryTypeDef,
-    VideoOutputTypeDef,
+    VideoTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
@@ -622,85 +615,83 @@
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestOutputTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
-    VideoTypeDef,
+    RegionOfInterestTypeDef,
     HumanLoopConfigTypeDef,
-    StreamProcessorInputOutputTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
     UserMatchTypeDef,
-    RegionOfInterestTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
-    AssetOutputTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
     EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
     StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    SearchUsersByImageRequestRequestTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
-    DetectModerationLabelsRequestRequestTypeDef,
-    StartStreamProcessorRequestRequestTypeDef,
-    SearchUsersResponseTypeDef,
     DetectTextFiltersTypeDef,
     StartTextDetectionFiltersTypeDef,
     UpdateStreamProcessorRequestRequestTypeDef,
+    DetectModerationLabelsRequestRequestTypeDef,
+    StartStreamProcessorRequestRequestTypeDef,
+    SearchUsersResponseTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     TestingDataOutputTypeDef,
+    TestingDataTypeDef,
     TrainingDataOutputTypeDef,
+    TrainingDataTypeDef,
     ValidationDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
@@ -708,28 +699,25 @@
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.12/setup.py` & `mypy-boto3-rekognition-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Rekognition 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

