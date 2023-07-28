# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.12.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.876567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21021 2023-07-27 05:34:22.872567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.872567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63499 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63426 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.872567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21021 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.876567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.388738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-28 20:20:36.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48676 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48619 2023-07-28 20:20:36.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,173 +337,133 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
-    ActiveSpeakerOnlyConfigurationOutputTypeDef,
     ActiveSpeakerOnlyConfigurationTypeDef,
-    PostCallAnalyticsSettingsOutputTypeDef,
     PostCallAnalyticsSettingsTypeDef,
-    AmazonTranscribeProcessorConfigurationOutputTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
-    AudioConcatenationConfigurationOutputTypeDef,
-    CompositedVideoConcatenationConfigurationOutputTypeDef,
-    ContentConcatenationConfigurationOutputTypeDef,
-    DataChannelConcatenationConfigurationOutputTypeDef,
-    MeetingEventsConcatenationConfigurationOutputTypeDef,
-    TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
-    VideoConcatenationConfigurationOutputTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
     ContentConcatenationConfigurationTypeDef,
     DataChannelConcatenationConfigurationTypeDef,
     MeetingEventsConcatenationConfigurationTypeDef,
     TranscriptionMessagesConcatenationConfigurationTypeDef,
     VideoConcatenationConfigurationTypeDef,
-    AudioArtifactsConfigurationOutputTypeDef,
-    ContentArtifactsConfigurationOutputTypeDef,
-    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
-    ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
-    S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
-    HorizontalLayoutConfigurationOutputTypeDef,
-    PresenterOnlyConfigurationOutputTypeDef,
-    VerticalLayoutConfigurationOutputTypeDef,
-    VideoAttributeOutputTypeDef,
     HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
     VerticalLayoutConfigurationTypeDef,
     VideoAttributeTypeDef,
-    IssueDetectionConfigurationOutputTypeDef,
     IssueDetectionConfigurationTypeDef,
     KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
-    KinesisDataStreamSinkConfigurationOutputTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
-    RecordingStreamConfigurationOutputTypeDef,
     RecordingStreamConfigurationTypeDef,
-    LambdaFunctionSinkConfigurationOutputTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationSummaryTypeDef,
     ListMediaPipelinesRequestRequestTypeDef,
     MediaPipelineSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    LiveConnectorRTMPConfigurationOutputTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
-    S3RecordingSinkConfigurationOutputTypeDef,
-    SnsTopicSinkConfigurationOutputTypeDef,
-    SqsQueueSinkConfigurationOutputTypeDef,
-    VoiceAnalyticsProcessorConfigurationOutputTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
-    S3RecordingSinkRuntimeConfigurationOutputTypeDef,
-    SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
-    ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
-    ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
-    GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LiveConnectorSinkConfigurationOutputTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
-    ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
     StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    CompositedVideoArtifactsConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
     RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
-    MediaCapturePipelineSourceConfigurationOutputTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-    ArtifactsConfigurationOutputTypeDef,
-    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
-    ConcatenationSourceOutputTypeDef,
     ConcatenationSourceTypeDef,
     MediaInsightsPipelineTypeDef,
     CreateMediaInsightsPipelineRequestRequestTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
-    LiveConnectorSourceConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
-    MediaConcatenationPipelineTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
+    MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     MediaCapturePipelineTypeDef,
-    MediaLiveConnectorPipelineTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
+    MediaLiveConnectorPipelineTypeDef,
     CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveSpeakerOnlyConfigurationOutputTypeDef:
+def get_structure() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-chime-sdk-media-pipelines
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,173 +337,133 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
-    ActiveSpeakerOnlyConfigurationOutputTypeDef,
     ActiveSpeakerOnlyConfigurationTypeDef,
-    PostCallAnalyticsSettingsOutputTypeDef,
     PostCallAnalyticsSettingsTypeDef,
-    AmazonTranscribeProcessorConfigurationOutputTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
-    AudioConcatenationConfigurationOutputTypeDef,
-    CompositedVideoConcatenationConfigurationOutputTypeDef,
-    ContentConcatenationConfigurationOutputTypeDef,
-    DataChannelConcatenationConfigurationOutputTypeDef,
-    MeetingEventsConcatenationConfigurationOutputTypeDef,
-    TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
-    VideoConcatenationConfigurationOutputTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
     ContentConcatenationConfigurationTypeDef,
     DataChannelConcatenationConfigurationTypeDef,
     MeetingEventsConcatenationConfigurationTypeDef,
     TranscriptionMessagesConcatenationConfigurationTypeDef,
     VideoConcatenationConfigurationTypeDef,
-    AudioArtifactsConfigurationOutputTypeDef,
-    ContentArtifactsConfigurationOutputTypeDef,
-    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
-    ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
-    S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
-    HorizontalLayoutConfigurationOutputTypeDef,
-    PresenterOnlyConfigurationOutputTypeDef,
-    VerticalLayoutConfigurationOutputTypeDef,
-    VideoAttributeOutputTypeDef,
     HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
     VerticalLayoutConfigurationTypeDef,
     VideoAttributeTypeDef,
-    IssueDetectionConfigurationOutputTypeDef,
     IssueDetectionConfigurationTypeDef,
     KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
-    KinesisDataStreamSinkConfigurationOutputTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
-    RecordingStreamConfigurationOutputTypeDef,
     RecordingStreamConfigurationTypeDef,
-    LambdaFunctionSinkConfigurationOutputTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationSummaryTypeDef,
     ListMediaPipelinesRequestRequestTypeDef,
     MediaPipelineSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    LiveConnectorRTMPConfigurationOutputTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
-    S3RecordingSinkConfigurationOutputTypeDef,
-    SnsTopicSinkConfigurationOutputTypeDef,
-    SqsQueueSinkConfigurationOutputTypeDef,
-    VoiceAnalyticsProcessorConfigurationOutputTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
-    S3RecordingSinkRuntimeConfigurationOutputTypeDef,
-    SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
-    ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
-    ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
-    GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LiveConnectorSinkConfigurationOutputTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
-    ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
     StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    CompositedVideoArtifactsConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
     RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
-    MediaCapturePipelineSourceConfigurationOutputTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-    ArtifactsConfigurationOutputTypeDef,
-    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
-    ConcatenationSourceOutputTypeDef,
     ConcatenationSourceTypeDef,
     MediaInsightsPipelineTypeDef,
     CreateMediaInsightsPipelineRequestRequestTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
-    LiveConnectorSourceConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
-    MediaConcatenationPipelineTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
+    MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     MediaCapturePipelineTypeDef,
-    MediaLiveConnectorPipelineTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
+    MediaLiveConnectorPipelineTypeDef,
     CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveSpeakerOnlyConfigurationOutputTypeDef:
+def get_structure() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime-sdk-media-pipelines service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationOutputTypeDef
+    from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationTypeDef
 
-    data: ActiveSpeakerOnlyConfigurationOutputTypeDef = {...}
+    data: ActiveSpeakerOnlyConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,210 +52,139 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
     "ActiveSpeakerOnlyConfigurationTypeDef",
-    "PostCallAnalyticsSettingsOutputTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
-    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
-    "AudioConcatenationConfigurationOutputTypeDef",
-    "CompositedVideoConcatenationConfigurationOutputTypeDef",
-    "ContentConcatenationConfigurationOutputTypeDef",
-    "DataChannelConcatenationConfigurationOutputTypeDef",
-    "MeetingEventsConcatenationConfigurationOutputTypeDef",
-    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
-    "VideoConcatenationConfigurationOutputTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
     "DataChannelConcatenationConfigurationTypeDef",
     "MeetingEventsConcatenationConfigurationTypeDef",
     "TranscriptionMessagesConcatenationConfigurationTypeDef",
     "VideoConcatenationConfigurationTypeDef",
-    "AudioArtifactsConfigurationOutputTypeDef",
-    "ContentArtifactsConfigurationOutputTypeDef",
-    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
-    "ChannelDefinitionOutputTypeDef",
     "ChannelDefinitionTypeDef",
-    "S3BucketSinkConfigurationOutputTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "TimestampRangeOutputTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
-    "HorizontalLayoutConfigurationOutputTypeDef",
-    "PresenterOnlyConfigurationOutputTypeDef",
-    "VerticalLayoutConfigurationOutputTypeDef",
-    "VideoAttributeOutputTypeDef",
     "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "VerticalLayoutConfigurationTypeDef",
     "VideoAttributeTypeDef",
-    "IssueDetectionConfigurationOutputTypeDef",
     "IssueDetectionConfigurationTypeDef",
     "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
-    "KinesisDataStreamSinkConfigurationOutputTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
-    "RecordingStreamConfigurationOutputTypeDef",
     "RecordingStreamConfigurationTypeDef",
-    "LambdaFunctionSinkConfigurationOutputTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     "ListMediaPipelinesRequestRequestTypeDef",
     "MediaPipelineSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "LiveConnectorRTMPConfigurationOutputTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
-    "S3RecordingSinkConfigurationOutputTypeDef",
-    "SnsTopicSinkConfigurationOutputTypeDef",
-    "SqsQueueSinkConfigurationOutputTypeDef",
-    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
-    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
-    "SentimentConfigurationOutputTypeDef",
     "SentimentConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
-    "ArtifactsConcatenationConfigurationOutputTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
-    "ConcatenationSinkOutputTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "FragmentSelectorOutputTypeDef",
     "FragmentSelectorTypeDef",
-    "GridViewConfigurationOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LiveConnectorSinkConfigurationOutputTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
     "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
-    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
-    "CompositedVideoArtifactsConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
     "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
-    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
-    "ArtifactsConfigurationOutputTypeDef",
-    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
-    "ConcatenationSourceOutputTypeDef",
     "ConcatenationSourceTypeDef",
     "MediaInsightsPipelineTypeDef",
     "CreateMediaInsightsPipelineRequestRequestTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
-    "LiveConnectorSourceConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
-    "MediaConcatenationPipelineTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
+    "MediaConcatenationPipelineTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
     "MediaCapturePipelineTypeDef",
-    "MediaLiveConnectorPipelineTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "MediaLiveConnectorPipelineTypeDef",
     "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
-ActiveSpeakerOnlyConfigurationOutputTypeDef = TypedDict(
-    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
-    {
-        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
-    },
-    total=False,
-)
-
 ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
     },
     total=False,
 )
 
-_RequiredPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
-    "_RequiredPostCallAnalyticsSettingsOutputTypeDef",
-    {
-        "OutputLocation": str,
-        "DataAccessRoleArn": str,
-    },
-)
-_OptionalPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
-    "_OptionalPostCallAnalyticsSettingsOutputTypeDef",
-    {
-        "ContentRedactionOutput": ContentRedactionOutputType,
-        "OutputEncryptionKMSKeyId": str,
-    },
-    total=False,
-)
-
-
-class PostCallAnalyticsSettingsOutputTypeDef(
-    _RequiredPostCallAnalyticsSettingsOutputTypeDef, _OptionalPostCallAnalyticsSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -271,38 +200,14 @@
 
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
 
-AmazonTranscribeProcessorConfigurationOutputTypeDef = TypedDict(
-    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
-    {
-        "LanguageCode": CallAnalyticsLanguageCodeType,
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "ShowSpeakerLabel": bool,
-        "EnablePartialResultsStabilization": bool,
-        "PartialResultsStability": PartialResultsStabilityType,
-        "ContentIdentificationType": Literal["PII"],
-        "ContentRedactionType": Literal["PII"],
-        "PiiEntityTypes": str,
-        "LanguageModelName": str,
-        "FilterPartialResults": bool,
-        "IdentifyLanguage": bool,
-        "LanguageOptions": str,
-        "PreferredLanguage": CallAnalyticsLanguageCodeType,
-        "VocabularyNames": str,
-        "VocabularyFilterNames": str,
-    },
-    total=False,
-)
-
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
@@ -319,63 +224,14 @@
         "PreferredLanguage": CallAnalyticsLanguageCodeType,
         "VocabularyNames": str,
         "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-AudioConcatenationConfigurationOutputTypeDef = TypedDict(
-    "AudioConcatenationConfigurationOutputTypeDef",
-    {
-        "State": Literal["Enabled"],
-    },
-)
-
-CompositedVideoConcatenationConfigurationOutputTypeDef = TypedDict(
-    "CompositedVideoConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-ContentConcatenationConfigurationOutputTypeDef = TypedDict(
-    "ContentConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-DataChannelConcatenationConfigurationOutputTypeDef = TypedDict(
-    "DataChannelConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-MeetingEventsConcatenationConfigurationOutputTypeDef = TypedDict(
-    "MeetingEventsConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-TranscriptionMessagesConcatenationConfigurationOutputTypeDef = TypedDict(
-    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-VideoConcatenationConfigurationOutputTypeDef = TypedDict(
-    "VideoConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
 AudioConcatenationConfigurationTypeDef = TypedDict(
     "AudioConcatenationConfigurationTypeDef",
     {
         "State": Literal["Enabled"],
     },
 )
 
@@ -417,65 +273,14 @@
 VideoConcatenationConfigurationTypeDef = TypedDict(
     "VideoConcatenationConfigurationTypeDef",
     {
         "State": ArtifactsConcatenationStateType,
     },
 )
 
-AudioArtifactsConfigurationOutputTypeDef = TypedDict(
-    "AudioArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": AudioMuxTypeType,
-    },
-)
-
-_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredContentArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalContentArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["ContentOnly"],
-    },
-    total=False,
-)
-
-
-class ContentArtifactsConfigurationOutputTypeDef(
-    _RequiredContentArtifactsConfigurationOutputTypeDef,
-    _OptionalContentArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-
-_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["VideoOnly"],
-    },
-    total=False,
-)
-
-
-class VideoArtifactsConfigurationOutputTypeDef(
-    _RequiredVideoArtifactsConfigurationOutputTypeDef,
-    _OptionalVideoArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -517,35 +322,14 @@
 
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
 
-_RequiredChannelDefinitionOutputTypeDef = TypedDict(
-    "_RequiredChannelDefinitionOutputTypeDef",
-    {
-        "ChannelId": int,
-    },
-)
-_OptionalChannelDefinitionOutputTypeDef = TypedDict(
-    "_OptionalChannelDefinitionOutputTypeDef",
-    {
-        "ParticipantRole": ParticipantRoleType,
-    },
-    total=False,
-)
-
-
-class ChannelDefinitionOutputTypeDef(
-    _RequiredChannelDefinitionOutputTypeDef, _OptionalChannelDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
@@ -559,21 +343,14 @@
 
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
 
-S3BucketSinkConfigurationOutputTypeDef = TypedDict(
-    "S3BucketSinkConfigurationOutputTypeDef",
-    {
-        "Destination": str,
-    },
-)
-
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -581,14 +358,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -610,21 +398,14 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimestampRangeOutputTypeDef = TypedDict(
     "TimestampRangeOutputTypeDef",
     {
         "StartTimestamp": datetime,
         "EndTimestamp": datetime,
     },
 )
@@ -654,55 +435,14 @@
 GetMediaPipelineRequestRequestTypeDef = TypedDict(
     "GetMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-HorizontalLayoutConfigurationOutputTypeDef = TypedDict(
-    "HorizontalLayoutConfigurationOutputTypeDef",
-    {
-        "TileOrder": TileOrderType,
-        "TilePosition": HorizontalTilePositionType,
-        "TileCount": int,
-        "TileAspectRatio": str,
-    },
-    total=False,
-)
-
-PresenterOnlyConfigurationOutputTypeDef = TypedDict(
-    "PresenterOnlyConfigurationOutputTypeDef",
-    {
-        "PresenterPosition": PresenterPositionType,
-    },
-    total=False,
-)
-
-VerticalLayoutConfigurationOutputTypeDef = TypedDict(
-    "VerticalLayoutConfigurationOutputTypeDef",
-    {
-        "TileOrder": TileOrderType,
-        "TilePosition": VerticalTilePositionType,
-        "TileCount": int,
-        "TileAspectRatio": str,
-    },
-    total=False,
-)
-
-VideoAttributeOutputTypeDef = TypedDict(
-    "VideoAttributeOutputTypeDef",
-    {
-        "CornerRadius": int,
-        "BorderColor": BorderColorType,
-        "HighlightColor": HighlightColorType,
-        "BorderThickness": int,
-    },
-    total=False,
-)
-
 HorizontalLayoutConfigurationTypeDef = TypedDict(
     "HorizontalLayoutConfigurationTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": HorizontalTilePositionType,
         "TileCount": int,
         "TileAspectRatio": str,
@@ -736,21 +476,14 @@
         "BorderColor": BorderColorType,
         "HighlightColor": HighlightColorType,
         "BorderThickness": int,
     },
     total=False,
 )
 
-IssueDetectionConfigurationOutputTypeDef = TypedDict(
-    "IssueDetectionConfigurationOutputTypeDef",
-    {
-        "RuleName": str,
-    },
-)
-
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
@@ -794,54 +527,30 @@
 
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
 
-KinesisDataStreamSinkConfigurationOutputTypeDef = TypedDict(
-    "KinesisDataStreamSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
 
-RecordingStreamConfigurationOutputTypeDef = TypedDict(
-    "RecordingStreamConfigurationOutputTypeDef",
-    {
-        "StreamArn": str,
-    },
-    total=False,
-)
-
 RecordingStreamConfigurationTypeDef = TypedDict(
     "RecordingStreamConfigurationTypeDef",
     {
         "StreamArn": str,
     },
     total=False,
 )
 
-LambdaFunctionSinkConfigurationOutputTypeDef = TypedDict(
-    "LambdaFunctionSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
 LambdaFunctionSinkConfigurationTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -904,45 +613,14 @@
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
-_RequiredLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLiveConnectorRTMPConfigurationOutputTypeDef",
-    {
-        "Url": str,
-    },
-)
-_OptionalLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLiveConnectorRTMPConfigurationOutputTypeDef",
-    {
-        "AudioChannels": AudioChannelsOptionType,
-        "AudioSampleRate": str,
-    },
-    total=False,
-)
-
-
-class LiveConnectorRTMPConfigurationOutputTypeDef(
-    _RequiredLiveConnectorRTMPConfigurationOutputTypeDef,
-    _OptionalLiveConnectorRTMPConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredLiveConnectorRTMPConfigurationTypeDef = TypedDict(
     "_RequiredLiveConnectorRTMPConfigurationTypeDef",
     {
         "Url": str,
     },
 )
 _OptionalLiveConnectorRTMPConfigurationTypeDef = TypedDict(
@@ -957,48 +635,14 @@
 
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
 
-S3RecordingSinkConfigurationOutputTypeDef = TypedDict(
-    "S3RecordingSinkConfigurationOutputTypeDef",
-    {
-        "Destination": str,
-        "RecordingFileFormat": RecordingFileFormatType,
-    },
-    total=False,
-)
-
-SnsTopicSinkConfigurationOutputTypeDef = TypedDict(
-    "SnsTopicSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
-SqsQueueSinkConfigurationOutputTypeDef = TypedDict(
-    "SqsQueueSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
-VoiceAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
-    {
-        "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
-        "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
-    },
-    total=False,
-)
-
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -1025,51 +669,23 @@
     {
         "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
         "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
     },
     total=False,
 )
 
-S3RecordingSinkRuntimeConfigurationOutputTypeDef = TypedDict(
-    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
-    {
-        "Destination": str,
-        "RecordingFileFormat": RecordingFileFormatType,
-    },
-)
-
-SentimentConfigurationOutputTypeDef = TypedDict(
-    "SentimentConfigurationOutputTypeDef",
-    {
-        "RuleName": str,
-        "SentimentType": Literal["NEGATIVE"],
-        "TimePeriod": int,
-    },
-)
-
 SentimentConfigurationTypeDef = TypedDict(
     "SentimentConfigurationTypeDef",
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
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
 SelectedVideoStreamsOutputTypeDef = TypedDict(
     "SelectedVideoStreamsOutputTypeDef",
     {
         "AttendeeIds": List[str],
         "ExternalUserIds": List[str],
     },
     total=False,
@@ -1115,15 +731,15 @@
         "LanguageModelName": str,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "FilterPartialResults": bool,
-        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsOutputTypeDef,
+        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
     total=False,
 )
 
 
 class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
@@ -1162,27 +778,14 @@
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
 
-ArtifactsConcatenationConfigurationOutputTypeDef = TypedDict(
-    "ArtifactsConcatenationConfigurationOutputTypeDef",
-    {
-        "Audio": AudioConcatenationConfigurationOutputTypeDef,
-        "Video": VideoConcatenationConfigurationOutputTypeDef,
-        "Content": ContentConcatenationConfigurationOutputTypeDef,
-        "DataChannel": DataChannelConcatenationConfigurationOutputTypeDef,
-        "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
-        "MeetingEvents": MeetingEventsConcatenationConfigurationOutputTypeDef,
-        "CompositedVideo": CompositedVideoConcatenationConfigurationOutputTypeDef,
-    },
-)
-
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -1197,15 +800,15 @@
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionOutputTypeDef",
     {
-        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
+        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
 
 class StreamChannelDefinitionOutputTypeDef(
     _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
@@ -1230,22 +833,14 @@
 
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
 
-ConcatenationSinkOutputTypeDef = TypedDict(
-    "ConcatenationSinkOutputTypeDef",
-    {
-        "Type": Literal["S3Bucket"],
-        "S3BucketSinkConfiguration": S3BucketSinkConfigurationOutputTypeDef,
-    },
-)
-
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -1254,14 +849,29 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
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
 FragmentSelectorOutputTypeDef = TypedDict(
     "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
@@ -1270,40 +880,14 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
-_RequiredGridViewConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGridViewConfigurationOutputTypeDef",
-    {
-        "ContentShareLayout": ContentShareLayoutOptionType,
-    },
-)
-_OptionalGridViewConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGridViewConfigurationOutputTypeDef",
-    {
-        "PresenterOnlyConfiguration": PresenterOnlyConfigurationOutputTypeDef,
-        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationOutputTypeDef,
-        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationOutputTypeDef,
-        "VerticalLayoutConfiguration": VerticalLayoutConfigurationOutputTypeDef,
-        "VideoAttribute": VideoAttributeOutputTypeDef,
-        "CanvasOrientation": CanvasOrientationType,
-    },
-    total=False,
-)
-
-
-class GridViewConfigurationOutputTypeDef(
-    _RequiredGridViewConfigurationOutputTypeDef, _OptionalGridViewConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -1327,51 +911,35 @@
 
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
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
-    },
-)
-
-LiveConnectorSinkConfigurationOutputTypeDef = TypedDict(
-    "LiveConnectorSinkConfigurationOutputTypeDef",
-    {
-        "SinkType": Literal["RTMP"],
-        "RTMPConfiguration": LiveConnectorRTMPConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
@@ -1385,16 +953,16 @@
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
     "_OptionalRealTimeAlertRuleOutputTypeDef",
     {
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
-        "SentimentConfiguration": SentimentConfigurationOutputTypeDef,
-        "IssueDetectionConfiguration": IssueDetectionConfigurationOutputTypeDef,
+        "SentimentConfiguration": SentimentConfigurationTypeDef,
+        "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class RealTimeAlertRuleOutputTypeDef(
     _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
@@ -1449,23 +1017,21 @@
 )
 _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
     "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
     {
         "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
             AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
         ),
-        "AmazonTranscribeProcessorConfiguration": (
-            AmazonTranscribeProcessorConfigurationOutputTypeDef
-        ),
-        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationOutputTypeDef,
-        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationOutputTypeDef,
-        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationOutputTypeDef,
-        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationOutputTypeDef,
-        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationOutputTypeDef,
-        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationOutputTypeDef,
+        "AmazonTranscribeProcessorConfiguration": AmazonTranscribeProcessorConfigurationTypeDef,
+        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationTypeDef,
+        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationTypeDef,
+        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationTypeDef,
+        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
+        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
+        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class MediaInsightsPipelineConfigurationElementOutputTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
@@ -1501,21 +1067,14 @@
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
 
-ChimeSdkMeetingConcatenationConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
-    {
-        "ArtifactsConfiguration": ArtifactsConcatenationConfigurationOutputTypeDef,
-    },
-)
-
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -1562,50 +1121,27 @@
 ):
     pass
 
 
 KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
-        "Streams": List[RecordingStreamConfigurationOutputTypeDef],
+        "Streams": List[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
 
 KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
 
-_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
-    },
-)
-_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "Layout": Literal["GridView"],
-        "Resolution": ResolutionOptionType,
-    },
-    total=False,
-)
-
-
-class CompositedVideoArtifactsConfigurationOutputTypeDef(
-    _RequiredCompositedVideoArtifactsConfigurationOutputTypeDef,
-    _OptionalCompositedVideoArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1639,22 +1175,14 @@
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
-MediaCapturePipelineSourceConfigurationOutputTypeDef = TypedDict(
-    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
-    {
-        "MediaPipelineArn": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
-    },
-)
-
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
@@ -1673,84 +1201,61 @@
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
 )
 
-_RequiredArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredArtifactsConfigurationOutputTypeDef",
+_RequiredArtifactsConfigurationTypeDef = TypedDict(
+    "_RequiredArtifactsConfigurationTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationOutputTypeDef,
-        "Video": VideoArtifactsConfigurationOutputTypeDef,
-        "Content": ContentArtifactsConfigurationOutputTypeDef,
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
     },
 )
-_OptionalArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalArtifactsConfigurationOutputTypeDef",
+_OptionalArtifactsConfigurationTypeDef = TypedDict(
+    "_OptionalArtifactsConfigurationTypeDef",
     {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ArtifactsConfigurationOutputTypeDef(
-    _RequiredArtifactsConfigurationOutputTypeDef, _OptionalArtifactsConfigurationOutputTypeDef
+class ArtifactsConfigurationTypeDef(
+    _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
 
 _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
 _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
 ):
     pass
 
 
-_RequiredArtifactsConfigurationTypeDef = TypedDict(
-    "_RequiredArtifactsConfigurationTypeDef",
-    {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
-    },
-)
-_OptionalArtifactsConfigurationTypeDef = TypedDict(
-    "_OptionalArtifactsConfigurationTypeDef",
-    {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class ArtifactsConfigurationTypeDef(
-    _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
-):
-    pass
-
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1832,24 +1337,14 @@
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-ConcatenationSourceOutputTypeDef = TypedDict(
-    "ConcatenationSourceOutputTypeDef",
-    {
-        "Type": Literal["MediaCapturePipeline"],
-        "MediaCapturePipelineSourceConfiguration": (
-            MediaCapturePipelineSourceConfigurationOutputTypeDef
-        ),
-    },
-)
-
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
@@ -1864,15 +1359,15 @@
         "KinesisVideoStreamSourceRuntimeConfiguration": (
             KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
         ),
         "MediaInsightsRuntimeMetadata": Dict[str, str],
         "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
             KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
         ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
 _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
@@ -1905,84 +1400,70 @@
     pass
 
 
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
+    },
+    total=False,
+)
+
+ChimeSdkMeetingConfigurationTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationOutputTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
         ),
     },
 )
 
-ChimeSdkMeetingConfigurationTypeDef = TypedDict(
-    "ChimeSdkMeetingConfigurationTypeDef",
-    {
-        "SourceConfiguration": SourceConfigurationTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
-    },
-    total=False,
-)
-
 LiveConnectorSourceConfigurationTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationTypeDef
         ),
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MediaConcatenationPipelineTypeDef = TypedDict(
-    "MediaConcatenationPipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "Sources": List[ConcatenationSourceOutputTypeDef],
-        "Sinks": List[ConcatenationSinkOutputTypeDef],
-        "Status": MediaPipelineStatusType,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
@@ -2001,19 +1482,33 @@
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
 
+MediaConcatenationPipelineTypeDef = TypedDict(
+    "MediaConcatenationPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Sources": List[ConcatenationSourceTypeDef],
+        "Sinks": List[ConcatenationSinkTypeDef],
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
@@ -2026,28 +1521,14 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-MediaLiveConnectorPipelineTypeDef = TypedDict(
-    "MediaLiveConnectorPipelineTypeDef",
-    {
-        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
-        "Sinks": List[LiveConnectorSinkConfigurationOutputTypeDef],
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "Status": MediaPipelineStatusType,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -2067,14 +1548,28 @@
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
 
+MediaLiveConnectorPipelineTypeDef = TypedDict(
+    "MediaLiveConnectorPipelineTypeDef",
+    {
+        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
+        "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
@@ -2095,39 +1590,39 @@
     pass
 
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
@@ -2138,10 +1633,10 @@
     total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime-sdk-media-pipelines service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationOutputTypeDef
+    from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationTypeDef
 
-    data: ActiveSpeakerOnlyConfigurationOutputTypeDef = {...}
+    data: ActiveSpeakerOnlyConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -51,208 +51,139 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
     "ActiveSpeakerOnlyConfigurationTypeDef",
-    "PostCallAnalyticsSettingsOutputTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
-    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
-    "AudioConcatenationConfigurationOutputTypeDef",
-    "CompositedVideoConcatenationConfigurationOutputTypeDef",
-    "ContentConcatenationConfigurationOutputTypeDef",
-    "DataChannelConcatenationConfigurationOutputTypeDef",
-    "MeetingEventsConcatenationConfigurationOutputTypeDef",
-    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
-    "VideoConcatenationConfigurationOutputTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
     "DataChannelConcatenationConfigurationTypeDef",
     "MeetingEventsConcatenationConfigurationTypeDef",
     "TranscriptionMessagesConcatenationConfigurationTypeDef",
     "VideoConcatenationConfigurationTypeDef",
-    "AudioArtifactsConfigurationOutputTypeDef",
-    "ContentArtifactsConfigurationOutputTypeDef",
-    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
-    "ChannelDefinitionOutputTypeDef",
     "ChannelDefinitionTypeDef",
-    "S3BucketSinkConfigurationOutputTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "TimestampRangeOutputTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
-    "HorizontalLayoutConfigurationOutputTypeDef",
-    "PresenterOnlyConfigurationOutputTypeDef",
-    "VerticalLayoutConfigurationOutputTypeDef",
-    "VideoAttributeOutputTypeDef",
     "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "VerticalLayoutConfigurationTypeDef",
     "VideoAttributeTypeDef",
-    "IssueDetectionConfigurationOutputTypeDef",
     "IssueDetectionConfigurationTypeDef",
     "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
-    "KinesisDataStreamSinkConfigurationOutputTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
-    "RecordingStreamConfigurationOutputTypeDef",
     "RecordingStreamConfigurationTypeDef",
-    "LambdaFunctionSinkConfigurationOutputTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     "ListMediaPipelinesRequestRequestTypeDef",
     "MediaPipelineSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "LiveConnectorRTMPConfigurationOutputTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
-    "S3RecordingSinkConfigurationOutputTypeDef",
-    "SnsTopicSinkConfigurationOutputTypeDef",
-    "SqsQueueSinkConfigurationOutputTypeDef",
-    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
-    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
-    "SentimentConfigurationOutputTypeDef",
     "SentimentConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
-    "ArtifactsConcatenationConfigurationOutputTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
-    "ConcatenationSinkOutputTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "FragmentSelectorOutputTypeDef",
     "FragmentSelectorTypeDef",
-    "GridViewConfigurationOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LiveConnectorSinkConfigurationOutputTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
     "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
-    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
-    "CompositedVideoArtifactsConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
     "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
-    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
-    "ArtifactsConfigurationOutputTypeDef",
-    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
-    "ConcatenationSourceOutputTypeDef",
     "ConcatenationSourceTypeDef",
     "MediaInsightsPipelineTypeDef",
     "CreateMediaInsightsPipelineRequestRequestTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
-    "LiveConnectorSourceConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
-    "MediaConcatenationPipelineTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
+    "MediaConcatenationPipelineTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
     "MediaCapturePipelineTypeDef",
-    "MediaLiveConnectorPipelineTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "MediaLiveConnectorPipelineTypeDef",
     "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
-ActiveSpeakerOnlyConfigurationOutputTypeDef = TypedDict(
-    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
-    {
-        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
-    },
-    total=False,
-)
-
 ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
     },
     total=False,
 )
 
-_RequiredPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
-    "_RequiredPostCallAnalyticsSettingsOutputTypeDef",
-    {
-        "OutputLocation": str,
-        "DataAccessRoleArn": str,
-    },
-)
-_OptionalPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
-    "_OptionalPostCallAnalyticsSettingsOutputTypeDef",
-    {
-        "ContentRedactionOutput": ContentRedactionOutputType,
-        "OutputEncryptionKMSKeyId": str,
-    },
-    total=False,
-)
-
-class PostCallAnalyticsSettingsOutputTypeDef(
-    _RequiredPostCallAnalyticsSettingsOutputTypeDef, _OptionalPostCallAnalyticsSettingsOutputTypeDef
-):
-    pass
-
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -266,38 +197,14 @@
 )
 
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-AmazonTranscribeProcessorConfigurationOutputTypeDef = TypedDict(
-    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
-    {
-        "LanguageCode": CallAnalyticsLanguageCodeType,
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "ShowSpeakerLabel": bool,
-        "EnablePartialResultsStabilization": bool,
-        "PartialResultsStability": PartialResultsStabilityType,
-        "ContentIdentificationType": Literal["PII"],
-        "ContentRedactionType": Literal["PII"],
-        "PiiEntityTypes": str,
-        "LanguageModelName": str,
-        "FilterPartialResults": bool,
-        "IdentifyLanguage": bool,
-        "LanguageOptions": str,
-        "PreferredLanguage": CallAnalyticsLanguageCodeType,
-        "VocabularyNames": str,
-        "VocabularyFilterNames": str,
-    },
-    total=False,
-)
-
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
@@ -314,63 +221,14 @@
         "PreferredLanguage": CallAnalyticsLanguageCodeType,
         "VocabularyNames": str,
         "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-AudioConcatenationConfigurationOutputTypeDef = TypedDict(
-    "AudioConcatenationConfigurationOutputTypeDef",
-    {
-        "State": Literal["Enabled"],
-    },
-)
-
-CompositedVideoConcatenationConfigurationOutputTypeDef = TypedDict(
-    "CompositedVideoConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-ContentConcatenationConfigurationOutputTypeDef = TypedDict(
-    "ContentConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-DataChannelConcatenationConfigurationOutputTypeDef = TypedDict(
-    "DataChannelConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-MeetingEventsConcatenationConfigurationOutputTypeDef = TypedDict(
-    "MeetingEventsConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-TranscriptionMessagesConcatenationConfigurationOutputTypeDef = TypedDict(
-    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
-VideoConcatenationConfigurationOutputTypeDef = TypedDict(
-    "VideoConcatenationConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsConcatenationStateType,
-    },
-)
-
 AudioConcatenationConfigurationTypeDef = TypedDict(
     "AudioConcatenationConfigurationTypeDef",
     {
         "State": Literal["Enabled"],
     },
 )
 
@@ -412,61 +270,14 @@
 VideoConcatenationConfigurationTypeDef = TypedDict(
     "VideoConcatenationConfigurationTypeDef",
     {
         "State": ArtifactsConcatenationStateType,
     },
 )
 
-AudioArtifactsConfigurationOutputTypeDef = TypedDict(
-    "AudioArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": AudioMuxTypeType,
-    },
-)
-
-_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredContentArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalContentArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["ContentOnly"],
-    },
-    total=False,
-)
-
-class ContentArtifactsConfigurationOutputTypeDef(
-    _RequiredContentArtifactsConfigurationOutputTypeDef,
-    _OptionalContentArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["VideoOnly"],
-    },
-    total=False,
-)
-
-class VideoArtifactsConfigurationOutputTypeDef(
-    _RequiredVideoArtifactsConfigurationOutputTypeDef,
-    _OptionalVideoArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -504,33 +315,14 @@
 )
 
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
-_RequiredChannelDefinitionOutputTypeDef = TypedDict(
-    "_RequiredChannelDefinitionOutputTypeDef",
-    {
-        "ChannelId": int,
-    },
-)
-_OptionalChannelDefinitionOutputTypeDef = TypedDict(
-    "_OptionalChannelDefinitionOutputTypeDef",
-    {
-        "ParticipantRole": ParticipantRoleType,
-    },
-    total=False,
-)
-
-class ChannelDefinitionOutputTypeDef(
-    _RequiredChannelDefinitionOutputTypeDef, _OptionalChannelDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
@@ -542,21 +334,14 @@
 )
 
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
-S3BucketSinkConfigurationOutputTypeDef = TypedDict(
-    "S3BucketSinkConfigurationOutputTypeDef",
-    {
-        "Destination": str,
-    },
-)
-
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -564,14 +349,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -593,21 +389,14 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimestampRangeOutputTypeDef = TypedDict(
     "TimestampRangeOutputTypeDef",
     {
         "StartTimestamp": datetime,
         "EndTimestamp": datetime,
     },
 )
@@ -637,55 +426,14 @@
 GetMediaPipelineRequestRequestTypeDef = TypedDict(
     "GetMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-HorizontalLayoutConfigurationOutputTypeDef = TypedDict(
-    "HorizontalLayoutConfigurationOutputTypeDef",
-    {
-        "TileOrder": TileOrderType,
-        "TilePosition": HorizontalTilePositionType,
-        "TileCount": int,
-        "TileAspectRatio": str,
-    },
-    total=False,
-)
-
-PresenterOnlyConfigurationOutputTypeDef = TypedDict(
-    "PresenterOnlyConfigurationOutputTypeDef",
-    {
-        "PresenterPosition": PresenterPositionType,
-    },
-    total=False,
-)
-
-VerticalLayoutConfigurationOutputTypeDef = TypedDict(
-    "VerticalLayoutConfigurationOutputTypeDef",
-    {
-        "TileOrder": TileOrderType,
-        "TilePosition": VerticalTilePositionType,
-        "TileCount": int,
-        "TileAspectRatio": str,
-    },
-    total=False,
-)
-
-VideoAttributeOutputTypeDef = TypedDict(
-    "VideoAttributeOutputTypeDef",
-    {
-        "CornerRadius": int,
-        "BorderColor": BorderColorType,
-        "HighlightColor": HighlightColorType,
-        "BorderThickness": int,
-    },
-    total=False,
-)
-
 HorizontalLayoutConfigurationTypeDef = TypedDict(
     "HorizontalLayoutConfigurationTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": HorizontalTilePositionType,
         "TileCount": int,
         "TileAspectRatio": str,
@@ -719,21 +467,14 @@
         "BorderColor": BorderColorType,
         "HighlightColor": HighlightColorType,
         "BorderThickness": int,
     },
     total=False,
 )
 
-IssueDetectionConfigurationOutputTypeDef = TypedDict(
-    "IssueDetectionConfigurationOutputTypeDef",
-    {
-        "RuleName": str,
-    },
-)
-
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
@@ -773,54 +514,30 @@
 )
 
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
-KinesisDataStreamSinkConfigurationOutputTypeDef = TypedDict(
-    "KinesisDataStreamSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
 
-RecordingStreamConfigurationOutputTypeDef = TypedDict(
-    "RecordingStreamConfigurationOutputTypeDef",
-    {
-        "StreamArn": str,
-    },
-    total=False,
-)
-
 RecordingStreamConfigurationTypeDef = TypedDict(
     "RecordingStreamConfigurationTypeDef",
     {
         "StreamArn": str,
     },
     total=False,
 )
 
-LambdaFunctionSinkConfigurationOutputTypeDef = TypedDict(
-    "LambdaFunctionSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
 LambdaFunctionSinkConfigurationTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -883,43 +600,14 @@
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
-_RequiredLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLiveConnectorRTMPConfigurationOutputTypeDef",
-    {
-        "Url": str,
-    },
-)
-_OptionalLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLiveConnectorRTMPConfigurationOutputTypeDef",
-    {
-        "AudioChannels": AudioChannelsOptionType,
-        "AudioSampleRate": str,
-    },
-    total=False,
-)
-
-class LiveConnectorRTMPConfigurationOutputTypeDef(
-    _RequiredLiveConnectorRTMPConfigurationOutputTypeDef,
-    _OptionalLiveConnectorRTMPConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredLiveConnectorRTMPConfigurationTypeDef = TypedDict(
     "_RequiredLiveConnectorRTMPConfigurationTypeDef",
     {
         "Url": str,
     },
 )
 _OptionalLiveConnectorRTMPConfigurationTypeDef = TypedDict(
@@ -932,48 +620,14 @@
 )
 
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
-S3RecordingSinkConfigurationOutputTypeDef = TypedDict(
-    "S3RecordingSinkConfigurationOutputTypeDef",
-    {
-        "Destination": str,
-        "RecordingFileFormat": RecordingFileFormatType,
-    },
-    total=False,
-)
-
-SnsTopicSinkConfigurationOutputTypeDef = TypedDict(
-    "SnsTopicSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
-SqsQueueSinkConfigurationOutputTypeDef = TypedDict(
-    "SqsQueueSinkConfigurationOutputTypeDef",
-    {
-        "InsightsTarget": str,
-    },
-    total=False,
-)
-
-VoiceAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
-    {
-        "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
-        "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
-    },
-    total=False,
-)
-
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -1000,51 +654,23 @@
     {
         "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
         "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
     },
     total=False,
 )
 
-S3RecordingSinkRuntimeConfigurationOutputTypeDef = TypedDict(
-    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
-    {
-        "Destination": str,
-        "RecordingFileFormat": RecordingFileFormatType,
-    },
-)
-
-SentimentConfigurationOutputTypeDef = TypedDict(
-    "SentimentConfigurationOutputTypeDef",
-    {
-        "RuleName": str,
-        "SentimentType": Literal["NEGATIVE"],
-        "TimePeriod": int,
-    },
-)
-
 SentimentConfigurationTypeDef = TypedDict(
     "SentimentConfigurationTypeDef",
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
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
 SelectedVideoStreamsOutputTypeDef = TypedDict(
     "SelectedVideoStreamsOutputTypeDef",
     {
         "AttendeeIds": List[str],
         "ExternalUserIds": List[str],
     },
     total=False,
@@ -1090,15 +716,15 @@
         "LanguageModelName": str,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "FilterPartialResults": bool,
-        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsOutputTypeDef,
+        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
     total=False,
 )
 
 class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
@@ -1133,27 +759,14 @@
 
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
-ArtifactsConcatenationConfigurationOutputTypeDef = TypedDict(
-    "ArtifactsConcatenationConfigurationOutputTypeDef",
-    {
-        "Audio": AudioConcatenationConfigurationOutputTypeDef,
-        "Video": VideoConcatenationConfigurationOutputTypeDef,
-        "Content": ContentConcatenationConfigurationOutputTypeDef,
-        "DataChannel": DataChannelConcatenationConfigurationOutputTypeDef,
-        "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
-        "MeetingEvents": MeetingEventsConcatenationConfigurationOutputTypeDef,
-        "CompositedVideo": CompositedVideoConcatenationConfigurationOutputTypeDef,
-    },
-)
-
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -1168,15 +781,15 @@
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionOutputTypeDef",
     {
-        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
+        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
 class StreamChannelDefinitionOutputTypeDef(
     _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
 ):
@@ -1197,22 +810,14 @@
 )
 
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
-ConcatenationSinkOutputTypeDef = TypedDict(
-    "ConcatenationSinkOutputTypeDef",
-    {
-        "Type": Literal["S3Bucket"],
-        "S3BucketSinkConfiguration": S3BucketSinkConfigurationOutputTypeDef,
-    },
-)
-
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -1221,14 +826,29 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
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
 FragmentSelectorOutputTypeDef = TypedDict(
     "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
@@ -1237,38 +857,14 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
-_RequiredGridViewConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGridViewConfigurationOutputTypeDef",
-    {
-        "ContentShareLayout": ContentShareLayoutOptionType,
-    },
-)
-_OptionalGridViewConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGridViewConfigurationOutputTypeDef",
-    {
-        "PresenterOnlyConfiguration": PresenterOnlyConfigurationOutputTypeDef,
-        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationOutputTypeDef,
-        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationOutputTypeDef,
-        "VerticalLayoutConfiguration": VerticalLayoutConfigurationOutputTypeDef,
-        "VideoAttribute": VideoAttributeOutputTypeDef,
-        "CanvasOrientation": CanvasOrientationType,
-    },
-    total=False,
-)
-
-class GridViewConfigurationOutputTypeDef(
-    _RequiredGridViewConfigurationOutputTypeDef, _OptionalGridViewConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -1290,51 +886,35 @@
     pass
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
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
-    },
-)
-
-LiveConnectorSinkConfigurationOutputTypeDef = TypedDict(
-    "LiveConnectorSinkConfigurationOutputTypeDef",
-    {
-        "SinkType": Literal["RTMP"],
-        "RTMPConfiguration": LiveConnectorRTMPConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
@@ -1348,16 +928,16 @@
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
     "_OptionalRealTimeAlertRuleOutputTypeDef",
     {
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
-        "SentimentConfiguration": SentimentConfigurationOutputTypeDef,
-        "IssueDetectionConfiguration": IssueDetectionConfigurationOutputTypeDef,
+        "SentimentConfiguration": SentimentConfigurationTypeDef,
+        "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
 class RealTimeAlertRuleOutputTypeDef(
     _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
 ):
@@ -1408,23 +988,21 @@
 )
 _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
     "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
     {
         "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
             AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
         ),
-        "AmazonTranscribeProcessorConfiguration": (
-            AmazonTranscribeProcessorConfigurationOutputTypeDef
-        ),
-        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationOutputTypeDef,
-        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationOutputTypeDef,
-        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationOutputTypeDef,
-        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationOutputTypeDef,
-        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationOutputTypeDef,
-        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationOutputTypeDef,
+        "AmazonTranscribeProcessorConfiguration": AmazonTranscribeProcessorConfigurationTypeDef,
+        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationTypeDef,
+        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationTypeDef,
+        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationTypeDef,
+        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
+        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
+        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
 class MediaInsightsPipelineConfigurationElementOutputTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
@@ -1456,21 +1034,14 @@
 
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
-ChimeSdkMeetingConcatenationConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
-    {
-        "ArtifactsConfiguration": ArtifactsConcatenationConfigurationOutputTypeDef,
-    },
-)
-
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -1513,48 +1084,27 @@
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
 KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
-        "Streams": List[RecordingStreamConfigurationOutputTypeDef],
+        "Streams": List[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
 
 KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
 
-_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
-    },
-)
-_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "Layout": Literal["GridView"],
-        "Resolution": ResolutionOptionType,
-    },
-    total=False,
-)
-
-class CompositedVideoArtifactsConfigurationOutputTypeDef(
-    _RequiredCompositedVideoArtifactsConfigurationOutputTypeDef,
-    _OptionalCompositedVideoArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1586,22 +1136,14 @@
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
-MediaCapturePipelineSourceConfigurationOutputTypeDef = TypedDict(
-    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
-    {
-        "MediaPipelineArn": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
-    },
-)
-
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
@@ -1620,78 +1162,57 @@
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
 )
 
-_RequiredArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredArtifactsConfigurationOutputTypeDef",
+_RequiredArtifactsConfigurationTypeDef = TypedDict(
+    "_RequiredArtifactsConfigurationTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationOutputTypeDef,
-        "Video": VideoArtifactsConfigurationOutputTypeDef,
-        "Content": ContentArtifactsConfigurationOutputTypeDef,
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
     },
 )
-_OptionalArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalArtifactsConfigurationOutputTypeDef",
+_OptionalArtifactsConfigurationTypeDef = TypedDict(
+    "_OptionalArtifactsConfigurationTypeDef",
     {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-class ArtifactsConfigurationOutputTypeDef(
-    _RequiredArtifactsConfigurationOutputTypeDef, _OptionalArtifactsConfigurationOutputTypeDef
+class ArtifactsConfigurationTypeDef(
+    _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
 _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
 _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
 ):
     pass
 
-_RequiredArtifactsConfigurationTypeDef = TypedDict(
-    "_RequiredArtifactsConfigurationTypeDef",
-    {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
-    },
-)
-_OptionalArtifactsConfigurationTypeDef = TypedDict(
-    "_OptionalArtifactsConfigurationTypeDef",
-    {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class ArtifactsConfigurationTypeDef(
-    _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
-):
-    pass
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1767,24 +1288,14 @@
 
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-ConcatenationSourceOutputTypeDef = TypedDict(
-    "ConcatenationSourceOutputTypeDef",
-    {
-        "Type": Literal["MediaCapturePipeline"],
-        "MediaCapturePipelineSourceConfiguration": (
-            MediaCapturePipelineSourceConfigurationOutputTypeDef
-        ),
-    },
-)
-
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
@@ -1799,15 +1310,15 @@
         "KinesisVideoStreamSourceRuntimeConfiguration": (
             KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
         ),
         "MediaInsightsRuntimeMetadata": Dict[str, str],
         "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
             KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
         ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
 _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
@@ -1838,86 +1349,72 @@
 ):
     pass
 
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
+    },
+    total=False,
+)
+
+ChimeSdkMeetingConfigurationTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationOutputTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
         ),
     },
 )
 
-ChimeSdkMeetingConfigurationTypeDef = TypedDict(
-    "ChimeSdkMeetingConfigurationTypeDef",
-    {
-        "SourceConfiguration": SourceConfigurationTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
-    },
-    total=False,
-)
-
 LiveConnectorSourceConfigurationTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationTypeDef
         ),
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MediaConcatenationPipelineTypeDef = TypedDict(
-    "MediaConcatenationPipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "Sources": List[ConcatenationSourceOutputTypeDef],
-        "Sinks": List[ConcatenationSinkOutputTypeDef],
-        "Status": MediaPipelineStatusType,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1932,19 +1429,33 @@
 
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
+MediaConcatenationPipelineTypeDef = TypedDict(
+    "MediaConcatenationPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Sources": List[ConcatenationSourceTypeDef],
+        "Sinks": List[ConcatenationSinkTypeDef],
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
@@ -1957,28 +1468,14 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-MediaLiveConnectorPipelineTypeDef = TypedDict(
-    "MediaLiveConnectorPipelineTypeDef",
-    {
-        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
-        "Sinks": List[LiveConnectorSinkConfigurationOutputTypeDef],
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "Status": MediaPipelineStatusType,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -1996,14 +1493,28 @@
 
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
+MediaLiveConnectorPipelineTypeDef = TypedDict(
+    "MediaLiveConnectorPipelineTypeDef",
+    {
+        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
+        "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
@@ -2022,39 +1533,39 @@
 ):
     pass
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
@@ -2065,10 +1576,10 @@
     total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,173 +305,133 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
-    ActiveSpeakerOnlyConfigurationOutputTypeDef,
     ActiveSpeakerOnlyConfigurationTypeDef,
-    PostCallAnalyticsSettingsOutputTypeDef,
     PostCallAnalyticsSettingsTypeDef,
-    AmazonTranscribeProcessorConfigurationOutputTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
-    AudioConcatenationConfigurationOutputTypeDef,
-    CompositedVideoConcatenationConfigurationOutputTypeDef,
-    ContentConcatenationConfigurationOutputTypeDef,
-    DataChannelConcatenationConfigurationOutputTypeDef,
-    MeetingEventsConcatenationConfigurationOutputTypeDef,
-    TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
-    VideoConcatenationConfigurationOutputTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
     ContentConcatenationConfigurationTypeDef,
     DataChannelConcatenationConfigurationTypeDef,
     MeetingEventsConcatenationConfigurationTypeDef,
     TranscriptionMessagesConcatenationConfigurationTypeDef,
     VideoConcatenationConfigurationTypeDef,
-    AudioArtifactsConfigurationOutputTypeDef,
-    ContentArtifactsConfigurationOutputTypeDef,
-    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
-    ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
-    S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
-    HorizontalLayoutConfigurationOutputTypeDef,
-    PresenterOnlyConfigurationOutputTypeDef,
-    VerticalLayoutConfigurationOutputTypeDef,
-    VideoAttributeOutputTypeDef,
     HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
     VerticalLayoutConfigurationTypeDef,
     VideoAttributeTypeDef,
-    IssueDetectionConfigurationOutputTypeDef,
     IssueDetectionConfigurationTypeDef,
     KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
-    KinesisDataStreamSinkConfigurationOutputTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
-    RecordingStreamConfigurationOutputTypeDef,
     RecordingStreamConfigurationTypeDef,
-    LambdaFunctionSinkConfigurationOutputTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationSummaryTypeDef,
     ListMediaPipelinesRequestRequestTypeDef,
     MediaPipelineSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    LiveConnectorRTMPConfigurationOutputTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
-    S3RecordingSinkConfigurationOutputTypeDef,
-    SnsTopicSinkConfigurationOutputTypeDef,
-    SqsQueueSinkConfigurationOutputTypeDef,
-    VoiceAnalyticsProcessorConfigurationOutputTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
-    S3RecordingSinkRuntimeConfigurationOutputTypeDef,
-    SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
-    ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
-    ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
-    GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LiveConnectorSinkConfigurationOutputTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
-    ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
     StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    CompositedVideoArtifactsConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
     RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
-    MediaCapturePipelineSourceConfigurationOutputTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-    ArtifactsConfigurationOutputTypeDef,
-    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
-    ConcatenationSourceOutputTypeDef,
     ConcatenationSourceTypeDef,
     MediaInsightsPipelineTypeDef,
     CreateMediaInsightsPipelineRequestRequestTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
-    LiveConnectorSourceConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
-    MediaConcatenationPipelineTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
+    MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     MediaCapturePipelineTypeDef,
-    MediaLiveConnectorPipelineTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
+    MediaLiveConnectorPipelineTypeDef,
     CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveSpeakerOnlyConfigurationOutputTypeDef:
+def get_structure() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.12/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

