# Comparing `tmp/mypy-boto3-medialive-1.28.12.tar.gz` & `tmp/mypy-boto3-medialive-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
```

## Comparing `mypy-boto3-medialive-1.28.12.tar` & `mypy-boto3-medialive-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43563 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42068 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.376443 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52938 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52848 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-07-27 05:26:14.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   214218 2023-07-27 05:26:19.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   214003 2023-07-27 05:26:17.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43563 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:26:12.000000 mypy-boto3-medialive-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38868 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37373 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.277474 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52938 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52848 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-07-28 20:31:26.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-07-28 20:31:26.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   172819 2023-07-28 20:31:33.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172642 2023-07-28 20:31:28.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38868 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/setup.py
```

### Comparing `mypy-boto3-medialive-1.28.12/LICENSE` & `mypy-boto3-medialive-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/PKG-INFO` & `mypy-boto3-medialive-1.28.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaLive 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -674,93 +674,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
-    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
-    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
-    AccountConfigurationOutputTypeDef,
     AccountConfigurationTypeDef,
-    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
-    ArchiveS3SettingsOutputTypeDef,
     ArchiveS3SettingsTypeDef,
-    OutputLocationRefOutputTypeDef,
     OutputLocationRefTypeDef,
-    InputChannelLevelOutputTypeDef,
     InputChannelLevelTypeDef,
-    Eac3AtmosSettingsOutputTypeDef,
-    Eac3SettingsOutputTypeDef,
-    Mp2SettingsOutputTypeDef,
-    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     WavSettingsTypeDef,
-    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
-    AudioDolbyEDecodeOutputTypeDef,
     AudioDolbyEDecodeTypeDef,
-    AudioHlsRenditionSelectionOutputTypeDef,
     AudioHlsRenditionSelectionTypeDef,
-    AudioLanguageSelectionOutputTypeDef,
     AudioLanguageSelectionTypeDef,
-    InputLocationOutputTypeDef,
-    AudioPidSelectionOutputTypeDef,
+    InputLocationTypeDef,
     AudioPidSelectionTypeDef,
-    AudioSilenceFailoverSettingsOutputTypeDef,
     AudioSilenceFailoverSettingsTypeDef,
-    AudioTrackOutputTypeDef,
     AudioTrackTypeDef,
-    InputLocationTypeDef,
-    EsamOutputTypeDef,
-    Scte35SpliceInsertOutputTypeDef,
-    Scte35TimeSignalAposOutputTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
+    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
-    EbuTtDDestinationSettingsOutputTypeDef,
-    TtmlDestinationSettingsOutputTypeDef,
-    WebvttDestinationSettingsOutputTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
-    CaptionLanguageMappingOutputTypeDef,
     CaptionLanguageMappingTypeDef,
-    CaptionRectangleOutputTypeDef,
     CaptionRectangleTypeDef,
-    DvbSubSourceSettingsOutputTypeDef,
-    EmbeddedSourceSettingsOutputTypeDef,
-    Scte20SourceSettingsOutputTypeDef,
-    Scte27SourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     Scte20SourceSettingsTypeDef,
     Scte27SourceSettingsTypeDef,
-    CdiInputSpecificationOutputTypeDef,
     CdiInputSpecificationTypeDef,
     ChannelEgressEndpointTypeDef,
-    InputSpecificationOutputTypeDef,
+    InputSpecificationTypeDef,
     MaintenanceStatusTypeDef,
     VpcOutputSettingsDescriptionTypeDef,
     PipelineDetailTypeDef,
     ClaimDeviceRequestRequestTypeDef,
-    InputSpecificationTypeDef,
     MaintenanceCreateSettingsTypeDef,
     VpcOutputSettingsTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputVpcRequestTypeDef,
     MediaConnectFlowRequestTypeDef,
@@ -771,218 +739,155 @@
     DeleteChannelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DeleteInputSecurityGroupRequestRequestTypeDef,
     DeleteMultiplexProgramRequestRequestTypeDef,
     MultiplexProgramPacketIdentifiersMapTypeDef,
     MultiplexProgramPipelineDetailTypeDef,
     DeleteMultiplexRequestRequestTypeDef,
-    MultiplexSettingsOutputTypeDef,
     DeleteReservationRequestRequestTypeDef,
-    RenewalSettingsOutputTypeDef,
+    RenewalSettingsTypeDef,
     ReservationResourceSpecificationTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
-    InputDeviceSettingsOutputTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeThumbnailsRequestRequestTypeDef,
-    DvbNitSettingsOutputTypeDef,
-    DvbSdtSettingsOutputTypeDef,
-    DvbTdtSettingsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FeatureActivationsOutputTypeDef,
-    NielsenConfigurationOutputTypeDef,
-    ThumbnailConfigurationOutputTypeDef,
-    TimecodeConfigOutputTypeDef,
+    DvbNitSettingsTypeDef,
+    DvbSdtSettingsTypeDef,
+    DvbTdtSettingsTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     TimecodeConfigTypeDef,
-    InputLossFailoverSettingsOutputTypeDef,
-    VideoBlackFailoverSettingsOutputTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
-    FecOutputSettingsOutputTypeDef,
-    FixedModeScheduleActionStartSettingsOutputTypeDef,
+    FecOutputSettingsTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
-    Fmp4HlsSettingsOutputTypeDef,
-    FollowModeScheduleActionStartSettingsOutputTypeDef,
+    Fmp4HlsSettingsTypeDef,
     FollowModeScheduleActionStartSettingsTypeDef,
-    FrameCaptureS3SettingsOutputTypeDef,
     FrameCaptureS3SettingsTypeDef,
-    FrameCaptureOutputSettingsOutputTypeDef,
-    TimecodeBurninSettingsOutputTypeDef,
+    FrameCaptureOutputSettingsTypeDef,
     TimecodeBurninSettingsTypeDef,
     H264ColorSpaceSettingsOutputTypeDef,
     H264ColorSpaceSettingsTypeDef,
-    TemporalFilterSettingsOutputTypeDef,
     TemporalFilterSettingsTypeDef,
-    Hdr10SettingsOutputTypeDef,
     Hdr10SettingsTypeDef,
-    HlsAkamaiSettingsOutputTypeDef,
     HlsAkamaiSettingsTypeDef,
-    HlsBasicPutSettingsOutputTypeDef,
     HlsBasicPutSettingsTypeDef,
-    HlsMediaStoreSettingsOutputTypeDef,
-    HlsS3SettingsOutputTypeDef,
-    HlsWebdavSettingsOutputTypeDef,
     HlsMediaStoreSettingsTypeDef,
     HlsS3SettingsTypeDef,
     HlsWebdavSettingsTypeDef,
-    HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
     HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
-    HlsInputSettingsOutputTypeDef,
     HlsInputSettingsTypeDef,
-    HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
-    StartTimecodeOutputTypeDef,
-    StopTimecodeOutputTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    M3u8SettingsOutputTypeDef,
+    M3u8SettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
-    MediaPackageOutputDestinationSettingsOutputTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
-    MotionGraphicsActivateScheduleActionSettingsOutputTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
     MotionGraphicsSettingsOutputTypeDef,
     MotionGraphicsSettingsTypeDef,
-    MsSmoothOutputSettingsOutputTypeDef,
+    MsSmoothOutputSettingsTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
-    MultiplexProgramChannelDestinationSettingsOutputTypeDef,
     MultiplexProgramChannelDestinationSettingsTypeDef,
-    MultiplexProgramServiceDescriptorOutputTypeDef,
     MultiplexProgramServiceDescriptorTypeDef,
     MultiplexSettingsSummaryTypeDef,
-    MultiplexStatmuxVideoSettingsOutputTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
-    NielsenCBETOutputTypeDef,
     NielsenCBETTypeDef,
-    NielsenNaesIiNwOutputTypeDef,
     NielsenNaesIiNwTypeDef,
-    OutputDestinationSettingsOutputTypeDef,
     OutputDestinationSettingsTypeDef,
     RtmpGroupSettingsOutputTypeDef,
-    UdpGroupSettingsOutputTypeDef,
-    RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    PipelinePauseStateSettingsOutputTypeDef,
+    RtmpGroupSettingsTypeDef,
     PipelinePauseStateSettingsTypeDef,
-    RenewalSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    Scte35InputScheduleActionSettingsOutputTypeDef,
-    Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
-    Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-    StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
-    Scte35DeliveryRestrictionsOutputTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
     StartMultiplexRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     StopMultiplexRequestRequestTypeDef,
     ThumbnailTypeDef,
     TransferInputDeviceRequestRequestTypeDef,
-    VideoSelectorPidOutputTypeDef,
     VideoSelectorPidTypeDef,
-    VideoSelectorProgramIdOutputTypeDef,
     VideoSelectorProgramIdTypeDef,
-    DescribeAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
-    ArchiveCdnSettingsOutputTypeDef,
     ArchiveCdnSettingsTypeDef,
-    MediaPackageGroupSettingsOutputTypeDef,
-    MsSmoothGroupSettingsOutputTypeDef,
-    MultiplexOutputSettingsOutputTypeDef,
-    RtmpOutputSettingsOutputTypeDef,
     MediaPackageGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    MultiplexOutputSettingsTypeDef,
+    RtmpOutputSettingsTypeDef,
     AudioChannelMappingOutputTypeDef,
     AudioChannelMappingTypeDef,
     AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
-    AudioOnlyHlsSettingsOutputTypeDef,
-    AvailBlankingOutputTypeDef,
-    BlackoutSlateOutputTypeDef,
-    BurnInDestinationSettingsOutputTypeDef,
-    DvbSubDestinationSettingsOutputTypeDef,
-    InputLossBehaviorOutputTypeDef,
-    StaticImageActivateScheduleActionSettingsOutputTypeDef,
-    StaticKeySettingsOutputTypeDef,
-    AudioTrackSelectionOutputTypeDef,
-    AudioTrackSelectionTypeDef,
+    AudioOnlyHlsSettingsTypeDef,
     AvailBlankingTypeDef,
     BlackoutSlateTypeDef,
     BurnInDestinationSettingsTypeDef,
     DvbSubDestinationSettingsTypeDef,
     InputLossBehaviorTypeDef,
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
-    AvailSettingsOutputTypeDef,
+    AudioTrackSelectionOutputTypeDef,
+    AudioTrackSelectionTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    TeletextSourceSettingsOutputTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
+    PurchaseOfferingRequestRequestTypeDef,
+    UpdateReservationRequestRequestTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     DescribeChannelRequestChannelCreatedWaitTypeDef,
     DescribeChannelRequestChannelDeletedWaitTypeDef,
@@ -996,160 +901,142 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    M2tsSettingsOutputTypeDef,
-    FailoverConditionSettingsOutputTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
+    M2tsSettingsTypeDef,
     FailoverConditionSettingsTypeDef,
     ScheduleActionStartSettingsOutputTypeDef,
     ScheduleActionStartSettingsTypeDef,
-    FrameCaptureCdnSettingsOutputTypeDef,
     FrameCaptureCdnSettingsTypeDef,
-    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
-    H264FilterSettingsOutputTypeDef,
-    H265FilterSettingsOutputTypeDef,
-    Mpeg2FilterSettingsOutputTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
     Mpeg2FilterSettingsTypeDef,
     H265ColorSpaceSettingsOutputTypeDef,
-    VideoSelectorColorSpaceSettingsOutputTypeDef,
     H265ColorSpaceSettingsTypeDef,
     VideoSelectorColorSpaceSettingsTypeDef,
-    HlsCdnSettingsOutputTypeDef,
     HlsCdnSettingsTypeDef,
-    NetworkInputSettingsOutputTypeDef,
     NetworkInputSettingsTypeDef,
-    InputClippingSettingsOutputTypeDef,
     InputClippingSettingsTypeDef,
     InputDestinationTypeDef,
     UpdateInputDeviceRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
-    StandardHlsSettingsOutputTypeDef,
+    StandardHlsSettingsTypeDef,
     MotionGraphicsConfigurationOutputTypeDef,
     MotionGraphicsConfigurationTypeDef,
     MultiplexOutputDestinationTypeDef,
     MultiplexSummaryTypeDef,
-    MultiplexVideoSettingsOutputTypeDef,
     MultiplexVideoSettingsTypeDef,
-    NielsenWatermarksSettingsOutputTypeDef,
     NielsenWatermarksSettingsTypeDef,
     OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
     PauseStateScheduleActionSettingsOutputTypeDef,
     PauseStateScheduleActionSettingsTypeDef,
-    PurchaseOfferingRequestRequestTypeDef,
-    UpdateReservationRequestRequestTypeDef,
-    Scte35SegmentationDescriptorOutputTypeDef,
     Scte35SegmentationDescriptorTypeDef,
     ThumbnailDetailTypeDef,
-    VideoSelectorSettingsOutputTypeDef,
     VideoSelectorSettingsTypeDef,
-    ArchiveGroupSettingsOutputTypeDef,
     ArchiveGroupSettingsTypeDef,
     RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
     CaptionDestinationSettingsOutputTypeDef,
-    GlobalConfigurationOutputTypeDef,
-    KeyProviderSettingsOutputTypeDef,
-    AudioSelectorSettingsOutputTypeDef,
-    AudioSelectorSettingsTypeDef,
     CaptionDestinationSettingsTypeDef,
     GlobalConfigurationTypeDef,
     KeyProviderSettingsTypeDef,
-    AvailConfigurationOutputTypeDef,
+    AudioSelectorSettingsOutputTypeDef,
+    AudioSelectorSettingsTypeDef,
     AvailConfigurationTypeDef,
     CaptionSelectorSettingsOutputTypeDef,
     CaptionSelectorSettingsTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     UpdateReservationResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
-    ArchiveContainerSettingsOutputTypeDef,
-    UdpContainerSettingsOutputTypeDef,
-    FailoverConditionOutputTypeDef,
+    ArchiveContainerSettingsTypeDef,
+    UdpContainerSettingsTypeDef,
     FailoverConditionTypeDef,
-    FrameCaptureGroupSettingsOutputTypeDef,
     FrameCaptureGroupSettingsTypeDef,
     H264SettingsOutputTypeDef,
-    Mpeg2SettingsOutputTypeDef,
     H264SettingsTypeDef,
     Mpeg2SettingsTypeDef,
     H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
     InputPrepareScheduleActionSettingsOutputTypeDef,
-    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputPrepareScheduleActionSettingsTypeDef,
+    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputSwitchScheduleActionSettingsTypeDef,
     DescribeInputResponseTypeDef,
     InputTypeDef,
-    HlsSettingsOutputTypeDef,
+    HlsSettingsTypeDef,
     DeleteMultiplexResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
-    MultiplexProgramSettingsOutputTypeDef,
     MultiplexProgramSettingsTypeDef,
-    AudioWatermarkSettingsOutputTypeDef,
     AudioWatermarkSettingsTypeDef,
     UpdateChannelClassRequestRequestTypeDef,
-    Scte35DescriptorSettingsOutputTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
-    VideoSelectorOutputTypeDef,
     VideoSelectorTypeDef,
     CaptionDescriptionOutputTypeDef,
+    CaptionDescriptionTypeDef,
     HlsGroupSettingsOutputTypeDef,
+    HlsGroupSettingsTypeDef,
     AudioSelectorOutputTypeDef,
     AudioSelectorTypeDef,
-    CaptionDescriptionTypeDef,
-    HlsGroupSettingsTypeDef,
     CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
-    ArchiveOutputSettingsOutputTypeDef,
-    UdpOutputSettingsOutputTypeDef,
+    ArchiveOutputSettingsTypeDef,
+    UdpOutputSettingsTypeDef,
     AutomaticInputFailoverSettingsOutputTypeDef,
     AutomaticInputFailoverSettingsTypeDef,
     VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     CreateInputResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     ListInputsResponseTypeDef,
     UpdateInputResponseTypeDef,
-    HlsOutputSettingsOutputTypeDef,
+    HlsOutputSettingsTypeDef,
     CreateMultiplexResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
+    CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
-    CreateMultiplexProgramRequestRequestTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
-    Scte35DescriptorOutputTypeDef,
     Scte35DescriptorTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
-    OutputSettingsOutputTypeDef,
+    OutputSettingsTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
     Scte35TimeSignalScheduleActionSettingsTypeDef,
     InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
@@ -1178,15 +1065,15 @@
     BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsOutputTypeDef:
+def get_structure() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.12/README.md` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-medialive
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -642,93 +674,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
-    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
-    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
-    AccountConfigurationOutputTypeDef,
     AccountConfigurationTypeDef,
-    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
-    ArchiveS3SettingsOutputTypeDef,
     ArchiveS3SettingsTypeDef,
-    OutputLocationRefOutputTypeDef,
     OutputLocationRefTypeDef,
-    InputChannelLevelOutputTypeDef,
     InputChannelLevelTypeDef,
-    Eac3AtmosSettingsOutputTypeDef,
-    Eac3SettingsOutputTypeDef,
-    Mp2SettingsOutputTypeDef,
-    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     WavSettingsTypeDef,
-    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
-    AudioDolbyEDecodeOutputTypeDef,
     AudioDolbyEDecodeTypeDef,
-    AudioHlsRenditionSelectionOutputTypeDef,
     AudioHlsRenditionSelectionTypeDef,
-    AudioLanguageSelectionOutputTypeDef,
     AudioLanguageSelectionTypeDef,
-    InputLocationOutputTypeDef,
-    AudioPidSelectionOutputTypeDef,
+    InputLocationTypeDef,
     AudioPidSelectionTypeDef,
-    AudioSilenceFailoverSettingsOutputTypeDef,
     AudioSilenceFailoverSettingsTypeDef,
-    AudioTrackOutputTypeDef,
     AudioTrackTypeDef,
-    InputLocationTypeDef,
-    EsamOutputTypeDef,
-    Scte35SpliceInsertOutputTypeDef,
-    Scte35TimeSignalAposOutputTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
+    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
-    EbuTtDDestinationSettingsOutputTypeDef,
-    TtmlDestinationSettingsOutputTypeDef,
-    WebvttDestinationSettingsOutputTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
-    CaptionLanguageMappingOutputTypeDef,
     CaptionLanguageMappingTypeDef,
-    CaptionRectangleOutputTypeDef,
     CaptionRectangleTypeDef,
-    DvbSubSourceSettingsOutputTypeDef,
-    EmbeddedSourceSettingsOutputTypeDef,
-    Scte20SourceSettingsOutputTypeDef,
-    Scte27SourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     Scte20SourceSettingsTypeDef,
     Scte27SourceSettingsTypeDef,
-    CdiInputSpecificationOutputTypeDef,
     CdiInputSpecificationTypeDef,
     ChannelEgressEndpointTypeDef,
-    InputSpecificationOutputTypeDef,
+    InputSpecificationTypeDef,
     MaintenanceStatusTypeDef,
     VpcOutputSettingsDescriptionTypeDef,
     PipelineDetailTypeDef,
     ClaimDeviceRequestRequestTypeDef,
-    InputSpecificationTypeDef,
     MaintenanceCreateSettingsTypeDef,
     VpcOutputSettingsTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputVpcRequestTypeDef,
     MediaConnectFlowRequestTypeDef,
@@ -739,218 +739,155 @@
     DeleteChannelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DeleteInputSecurityGroupRequestRequestTypeDef,
     DeleteMultiplexProgramRequestRequestTypeDef,
     MultiplexProgramPacketIdentifiersMapTypeDef,
     MultiplexProgramPipelineDetailTypeDef,
     DeleteMultiplexRequestRequestTypeDef,
-    MultiplexSettingsOutputTypeDef,
     DeleteReservationRequestRequestTypeDef,
-    RenewalSettingsOutputTypeDef,
+    RenewalSettingsTypeDef,
     ReservationResourceSpecificationTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
-    InputDeviceSettingsOutputTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeThumbnailsRequestRequestTypeDef,
-    DvbNitSettingsOutputTypeDef,
-    DvbSdtSettingsOutputTypeDef,
-    DvbTdtSettingsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FeatureActivationsOutputTypeDef,
-    NielsenConfigurationOutputTypeDef,
-    ThumbnailConfigurationOutputTypeDef,
-    TimecodeConfigOutputTypeDef,
+    DvbNitSettingsTypeDef,
+    DvbSdtSettingsTypeDef,
+    DvbTdtSettingsTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     TimecodeConfigTypeDef,
-    InputLossFailoverSettingsOutputTypeDef,
-    VideoBlackFailoverSettingsOutputTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
-    FecOutputSettingsOutputTypeDef,
-    FixedModeScheduleActionStartSettingsOutputTypeDef,
+    FecOutputSettingsTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
-    Fmp4HlsSettingsOutputTypeDef,
-    FollowModeScheduleActionStartSettingsOutputTypeDef,
+    Fmp4HlsSettingsTypeDef,
     FollowModeScheduleActionStartSettingsTypeDef,
-    FrameCaptureS3SettingsOutputTypeDef,
     FrameCaptureS3SettingsTypeDef,
-    FrameCaptureOutputSettingsOutputTypeDef,
-    TimecodeBurninSettingsOutputTypeDef,
+    FrameCaptureOutputSettingsTypeDef,
     TimecodeBurninSettingsTypeDef,
     H264ColorSpaceSettingsOutputTypeDef,
     H264ColorSpaceSettingsTypeDef,
-    TemporalFilterSettingsOutputTypeDef,
     TemporalFilterSettingsTypeDef,
-    Hdr10SettingsOutputTypeDef,
     Hdr10SettingsTypeDef,
-    HlsAkamaiSettingsOutputTypeDef,
     HlsAkamaiSettingsTypeDef,
-    HlsBasicPutSettingsOutputTypeDef,
     HlsBasicPutSettingsTypeDef,
-    HlsMediaStoreSettingsOutputTypeDef,
-    HlsS3SettingsOutputTypeDef,
-    HlsWebdavSettingsOutputTypeDef,
     HlsMediaStoreSettingsTypeDef,
     HlsS3SettingsTypeDef,
     HlsWebdavSettingsTypeDef,
-    HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
     HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
-    HlsInputSettingsOutputTypeDef,
     HlsInputSettingsTypeDef,
-    HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
-    StartTimecodeOutputTypeDef,
-    StopTimecodeOutputTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    M3u8SettingsOutputTypeDef,
+    M3u8SettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
-    MediaPackageOutputDestinationSettingsOutputTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
-    MotionGraphicsActivateScheduleActionSettingsOutputTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
     MotionGraphicsSettingsOutputTypeDef,
     MotionGraphicsSettingsTypeDef,
-    MsSmoothOutputSettingsOutputTypeDef,
+    MsSmoothOutputSettingsTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
-    MultiplexProgramChannelDestinationSettingsOutputTypeDef,
     MultiplexProgramChannelDestinationSettingsTypeDef,
-    MultiplexProgramServiceDescriptorOutputTypeDef,
     MultiplexProgramServiceDescriptorTypeDef,
     MultiplexSettingsSummaryTypeDef,
-    MultiplexStatmuxVideoSettingsOutputTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
-    NielsenCBETOutputTypeDef,
     NielsenCBETTypeDef,
-    NielsenNaesIiNwOutputTypeDef,
     NielsenNaesIiNwTypeDef,
-    OutputDestinationSettingsOutputTypeDef,
     OutputDestinationSettingsTypeDef,
     RtmpGroupSettingsOutputTypeDef,
-    UdpGroupSettingsOutputTypeDef,
-    RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    PipelinePauseStateSettingsOutputTypeDef,
+    RtmpGroupSettingsTypeDef,
     PipelinePauseStateSettingsTypeDef,
-    RenewalSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    Scte35InputScheduleActionSettingsOutputTypeDef,
-    Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
-    Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-    StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
-    Scte35DeliveryRestrictionsOutputTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
     StartMultiplexRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     StopMultiplexRequestRequestTypeDef,
     ThumbnailTypeDef,
     TransferInputDeviceRequestRequestTypeDef,
-    VideoSelectorPidOutputTypeDef,
     VideoSelectorPidTypeDef,
-    VideoSelectorProgramIdOutputTypeDef,
     VideoSelectorProgramIdTypeDef,
-    DescribeAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
-    ArchiveCdnSettingsOutputTypeDef,
     ArchiveCdnSettingsTypeDef,
-    MediaPackageGroupSettingsOutputTypeDef,
-    MsSmoothGroupSettingsOutputTypeDef,
-    MultiplexOutputSettingsOutputTypeDef,
-    RtmpOutputSettingsOutputTypeDef,
     MediaPackageGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    MultiplexOutputSettingsTypeDef,
+    RtmpOutputSettingsTypeDef,
     AudioChannelMappingOutputTypeDef,
     AudioChannelMappingTypeDef,
     AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
-    AudioOnlyHlsSettingsOutputTypeDef,
-    AvailBlankingOutputTypeDef,
-    BlackoutSlateOutputTypeDef,
-    BurnInDestinationSettingsOutputTypeDef,
-    DvbSubDestinationSettingsOutputTypeDef,
-    InputLossBehaviorOutputTypeDef,
-    StaticImageActivateScheduleActionSettingsOutputTypeDef,
-    StaticKeySettingsOutputTypeDef,
-    AudioTrackSelectionOutputTypeDef,
-    AudioTrackSelectionTypeDef,
+    AudioOnlyHlsSettingsTypeDef,
     AvailBlankingTypeDef,
     BlackoutSlateTypeDef,
     BurnInDestinationSettingsTypeDef,
     DvbSubDestinationSettingsTypeDef,
     InputLossBehaviorTypeDef,
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
-    AvailSettingsOutputTypeDef,
+    AudioTrackSelectionOutputTypeDef,
+    AudioTrackSelectionTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    TeletextSourceSettingsOutputTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
+    PurchaseOfferingRequestRequestTypeDef,
+    UpdateReservationRequestRequestTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     DescribeChannelRequestChannelCreatedWaitTypeDef,
     DescribeChannelRequestChannelDeletedWaitTypeDef,
@@ -964,160 +901,142 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    M2tsSettingsOutputTypeDef,
-    FailoverConditionSettingsOutputTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
+    M2tsSettingsTypeDef,
     FailoverConditionSettingsTypeDef,
     ScheduleActionStartSettingsOutputTypeDef,
     ScheduleActionStartSettingsTypeDef,
-    FrameCaptureCdnSettingsOutputTypeDef,
     FrameCaptureCdnSettingsTypeDef,
-    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
-    H264FilterSettingsOutputTypeDef,
-    H265FilterSettingsOutputTypeDef,
-    Mpeg2FilterSettingsOutputTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
     Mpeg2FilterSettingsTypeDef,
     H265ColorSpaceSettingsOutputTypeDef,
-    VideoSelectorColorSpaceSettingsOutputTypeDef,
     H265ColorSpaceSettingsTypeDef,
     VideoSelectorColorSpaceSettingsTypeDef,
-    HlsCdnSettingsOutputTypeDef,
     HlsCdnSettingsTypeDef,
-    NetworkInputSettingsOutputTypeDef,
     NetworkInputSettingsTypeDef,
-    InputClippingSettingsOutputTypeDef,
     InputClippingSettingsTypeDef,
     InputDestinationTypeDef,
     UpdateInputDeviceRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
-    StandardHlsSettingsOutputTypeDef,
+    StandardHlsSettingsTypeDef,
     MotionGraphicsConfigurationOutputTypeDef,
     MotionGraphicsConfigurationTypeDef,
     MultiplexOutputDestinationTypeDef,
     MultiplexSummaryTypeDef,
-    MultiplexVideoSettingsOutputTypeDef,
     MultiplexVideoSettingsTypeDef,
-    NielsenWatermarksSettingsOutputTypeDef,
     NielsenWatermarksSettingsTypeDef,
     OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
     PauseStateScheduleActionSettingsOutputTypeDef,
     PauseStateScheduleActionSettingsTypeDef,
-    PurchaseOfferingRequestRequestTypeDef,
-    UpdateReservationRequestRequestTypeDef,
-    Scte35SegmentationDescriptorOutputTypeDef,
     Scte35SegmentationDescriptorTypeDef,
     ThumbnailDetailTypeDef,
-    VideoSelectorSettingsOutputTypeDef,
     VideoSelectorSettingsTypeDef,
-    ArchiveGroupSettingsOutputTypeDef,
     ArchiveGroupSettingsTypeDef,
     RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
     CaptionDestinationSettingsOutputTypeDef,
-    GlobalConfigurationOutputTypeDef,
-    KeyProviderSettingsOutputTypeDef,
-    AudioSelectorSettingsOutputTypeDef,
-    AudioSelectorSettingsTypeDef,
     CaptionDestinationSettingsTypeDef,
     GlobalConfigurationTypeDef,
     KeyProviderSettingsTypeDef,
-    AvailConfigurationOutputTypeDef,
+    AudioSelectorSettingsOutputTypeDef,
+    AudioSelectorSettingsTypeDef,
     AvailConfigurationTypeDef,
     CaptionSelectorSettingsOutputTypeDef,
     CaptionSelectorSettingsTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     UpdateReservationResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
-    ArchiveContainerSettingsOutputTypeDef,
-    UdpContainerSettingsOutputTypeDef,
-    FailoverConditionOutputTypeDef,
+    ArchiveContainerSettingsTypeDef,
+    UdpContainerSettingsTypeDef,
     FailoverConditionTypeDef,
-    FrameCaptureGroupSettingsOutputTypeDef,
     FrameCaptureGroupSettingsTypeDef,
     H264SettingsOutputTypeDef,
-    Mpeg2SettingsOutputTypeDef,
     H264SettingsTypeDef,
     Mpeg2SettingsTypeDef,
     H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
     InputPrepareScheduleActionSettingsOutputTypeDef,
-    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputPrepareScheduleActionSettingsTypeDef,
+    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputSwitchScheduleActionSettingsTypeDef,
     DescribeInputResponseTypeDef,
     InputTypeDef,
-    HlsSettingsOutputTypeDef,
+    HlsSettingsTypeDef,
     DeleteMultiplexResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
-    MultiplexProgramSettingsOutputTypeDef,
     MultiplexProgramSettingsTypeDef,
-    AudioWatermarkSettingsOutputTypeDef,
     AudioWatermarkSettingsTypeDef,
     UpdateChannelClassRequestRequestTypeDef,
-    Scte35DescriptorSettingsOutputTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
-    VideoSelectorOutputTypeDef,
     VideoSelectorTypeDef,
     CaptionDescriptionOutputTypeDef,
+    CaptionDescriptionTypeDef,
     HlsGroupSettingsOutputTypeDef,
+    HlsGroupSettingsTypeDef,
     AudioSelectorOutputTypeDef,
     AudioSelectorTypeDef,
-    CaptionDescriptionTypeDef,
-    HlsGroupSettingsTypeDef,
     CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
-    ArchiveOutputSettingsOutputTypeDef,
-    UdpOutputSettingsOutputTypeDef,
+    ArchiveOutputSettingsTypeDef,
+    UdpOutputSettingsTypeDef,
     AutomaticInputFailoverSettingsOutputTypeDef,
     AutomaticInputFailoverSettingsTypeDef,
     VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     CreateInputResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     ListInputsResponseTypeDef,
     UpdateInputResponseTypeDef,
-    HlsOutputSettingsOutputTypeDef,
+    HlsOutputSettingsTypeDef,
     CreateMultiplexResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
+    CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
-    CreateMultiplexProgramRequestRequestTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
-    Scte35DescriptorOutputTypeDef,
     Scte35DescriptorTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
-    OutputSettingsOutputTypeDef,
+    OutputSettingsTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
     Scte35TimeSignalScheduleActionSettingsTypeDef,
     InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
@@ -1146,15 +1065,15 @@
     BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsOutputTypeDef:
+def get_structure() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaLive 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,120 +82,120 @@
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
     def paginate(
-        self, *, TransferType: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
 
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
 
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
 
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
 
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
-        self, *, MultiplexId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
 
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
 
@@ -214,15 +214,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
 
@@ -239,13 +239,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,113 +79,113 @@
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
     def paginate(
-        self, *, TransferType: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
-        self, *, MultiplexId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
 class ListOfferingsPaginator(Paginator):
@@ -203,15 +203,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
 class ListReservationsPaginator(Paginator):
@@ -227,13 +227,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for medialive service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_medialive.type_defs import AacSettingsOutputTypeDef
+    from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
 
-    data: AacSettingsOutputTypeDef = {...}
+    data: AacSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from botocore.response import StreamingBody
@@ -285,95 +285,62 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
-    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
-    "AccountConfigurationOutputTypeDef",
     "AccountConfigurationTypeDef",
-    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
-    "ArchiveS3SettingsOutputTypeDef",
     "ArchiveS3SettingsTypeDef",
-    "OutputLocationRefOutputTypeDef",
     "OutputLocationRefTypeDef",
-    "InputChannelLevelOutputTypeDef",
     "InputChannelLevelTypeDef",
-    "Eac3AtmosSettingsOutputTypeDef",
-    "Eac3SettingsOutputTypeDef",
-    "Mp2SettingsOutputTypeDef",
-    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "WavSettingsTypeDef",
-    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
-    "AudioDolbyEDecodeOutputTypeDef",
     "AudioDolbyEDecodeTypeDef",
-    "AudioHlsRenditionSelectionOutputTypeDef",
     "AudioHlsRenditionSelectionTypeDef",
-    "AudioLanguageSelectionOutputTypeDef",
     "AudioLanguageSelectionTypeDef",
-    "InputLocationOutputTypeDef",
-    "AudioPidSelectionOutputTypeDef",
+    "InputLocationTypeDef",
     "AudioPidSelectionTypeDef",
-    "AudioSilenceFailoverSettingsOutputTypeDef",
     "AudioSilenceFailoverSettingsTypeDef",
-    "AudioTrackOutputTypeDef",
     "AudioTrackTypeDef",
-    "InputLocationTypeDef",
-    "EsamOutputTypeDef",
-    "Scte35SpliceInsertOutputTypeDef",
-    "Scte35TimeSignalAposOutputTypeDef",
     "EsamTypeDef",
     "Scte35SpliceInsertTypeDef",
     "Scte35TimeSignalAposTypeDef",
     "BatchDeleteRequestRequestTypeDef",
     "BatchFailedResultModelTypeDef",
     "BatchSuccessfulResultModelTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchScheduleActionDeleteRequestTypeDef",
     "BatchStartRequestRequestTypeDef",
     "BatchStopRequestRequestTypeDef",
     "CancelInputDeviceTransferRequestRequestTypeDef",
-    "EbuTtDDestinationSettingsOutputTypeDef",
-    "TtmlDestinationSettingsOutputTypeDef",
-    "WebvttDestinationSettingsOutputTypeDef",
     "EbuTtDDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
-    "CaptionLanguageMappingOutputTypeDef",
     "CaptionLanguageMappingTypeDef",
-    "CaptionRectangleOutputTypeDef",
     "CaptionRectangleTypeDef",
-    "DvbSubSourceSettingsOutputTypeDef",
-    "EmbeddedSourceSettingsOutputTypeDef",
-    "Scte20SourceSettingsOutputTypeDef",
-    "Scte27SourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "Scte20SourceSettingsTypeDef",
     "Scte27SourceSettingsTypeDef",
-    "CdiInputSpecificationOutputTypeDef",
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
-    "InputSpecificationOutputTypeDef",
+    "InputSpecificationTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
-    "InputSpecificationTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
     "MediaConnectFlowRequestTypeDef",
@@ -384,218 +351,155 @@
     "DeleteChannelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DeleteInputSecurityGroupRequestRequestTypeDef",
     "DeleteMultiplexProgramRequestRequestTypeDef",
     "MultiplexProgramPacketIdentifiersMapTypeDef",
     "MultiplexProgramPipelineDetailTypeDef",
     "DeleteMultiplexRequestRequestTypeDef",
-    "MultiplexSettingsOutputTypeDef",
     "DeleteReservationRequestRequestTypeDef",
-    "RenewalSettingsOutputTypeDef",
+    "RenewalSettingsTypeDef",
     "ReservationResourceSpecificationTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
-    "DescribeInputDeviceThumbnailResponseTypeDef",
     "DescribeInputRequestRequestTypeDef",
-    "InputDeviceSettingsOutputTypeDef",
     "InputSourceTypeDef",
     "MediaConnectFlowTypeDef",
     "DescribeInputSecurityGroupRequestRequestTypeDef",
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
-    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DescribeThumbnailsRequestRequestTypeDef",
-    "DvbNitSettingsOutputTypeDef",
-    "DvbSdtSettingsOutputTypeDef",
-    "DvbTdtSettingsOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FeatureActivationsOutputTypeDef",
-    "NielsenConfigurationOutputTypeDef",
-    "ThumbnailConfigurationOutputTypeDef",
-    "TimecodeConfigOutputTypeDef",
+    "DvbNitSettingsTypeDef",
+    "DvbSdtSettingsTypeDef",
+    "DvbTdtSettingsTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
-    "InputLossFailoverSettingsOutputTypeDef",
-    "VideoBlackFailoverSettingsOutputTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
-    "FecOutputSettingsOutputTypeDef",
-    "FixedModeScheduleActionStartSettingsOutputTypeDef",
+    "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
-    "Fmp4HlsSettingsOutputTypeDef",
-    "FollowModeScheduleActionStartSettingsOutputTypeDef",
+    "Fmp4HlsSettingsTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
-    "FrameCaptureS3SettingsOutputTypeDef",
     "FrameCaptureS3SettingsTypeDef",
-    "FrameCaptureOutputSettingsOutputTypeDef",
-    "TimecodeBurninSettingsOutputTypeDef",
+    "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
     "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
-    "TemporalFilterSettingsOutputTypeDef",
     "TemporalFilterSettingsTypeDef",
-    "Hdr10SettingsOutputTypeDef",
     "Hdr10SettingsTypeDef",
-    "HlsAkamaiSettingsOutputTypeDef",
     "HlsAkamaiSettingsTypeDef",
-    "HlsBasicPutSettingsOutputTypeDef",
     "HlsBasicPutSettingsTypeDef",
-    "HlsMediaStoreSettingsOutputTypeDef",
-    "HlsS3SettingsOutputTypeDef",
-    "HlsWebdavSettingsOutputTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
     "HlsWebdavSettingsTypeDef",
-    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
-    "HlsInputSettingsOutputTypeDef",
     "HlsInputSettingsTypeDef",
-    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
-    "StartTimecodeOutputTypeDef",
-    "StopTimecodeOutputTypeDef",
     "StartTimecodeTypeDef",
     "StopTimecodeTypeDef",
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "InputDeviceRequestTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
-    "ListInputsRequestListInputsPaginateTypeDef",
     "ListInputsRequestRequestTypeDef",
-    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "M3u8SettingsOutputTypeDef",
+    "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
-    "MediaPackageOutputDestinationSettingsOutputTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
-    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
-    "MsSmoothOutputSettingsOutputTypeDef",
+    "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
-    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
-    "MultiplexProgramServiceDescriptorOutputTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
-    "MultiplexStatmuxVideoSettingsOutputTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
-    "NielsenCBETOutputTypeDef",
     "NielsenCBETTypeDef",
-    "NielsenNaesIiNwOutputTypeDef",
     "NielsenNaesIiNwTypeDef",
-    "OutputDestinationSettingsOutputTypeDef",
     "OutputDestinationSettingsTypeDef",
     "RtmpGroupSettingsOutputTypeDef",
-    "UdpGroupSettingsOutputTypeDef",
-    "RtmpGroupSettingsTypeDef",
     "UdpGroupSettingsTypeDef",
-    "PaginatorConfigTypeDef",
-    "PipelinePauseStateSettingsOutputTypeDef",
+    "RtmpGroupSettingsTypeDef",
     "PipelinePauseStateSettingsTypeDef",
-    "RenewalSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "Scte35InputScheduleActionSettingsOutputTypeDef",
-    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
-    "Scte35SpliceInsertScheduleActionSettingsOutputTypeDef",
-    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
-    "Scte35DeliveryRestrictionsOutputTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
-    "VideoSelectorPidOutputTypeDef",
     "VideoSelectorPidTypeDef",
-    "VideoSelectorProgramIdOutputTypeDef",
     "VideoSelectorProgramIdTypeDef",
-    "DescribeAccountConfigurationResponseTypeDef",
-    "UpdateAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
-    "ArchiveCdnSettingsOutputTypeDef",
     "ArchiveCdnSettingsTypeDef",
-    "MediaPackageGroupSettingsOutputTypeDef",
-    "MsSmoothGroupSettingsOutputTypeDef",
-    "MultiplexOutputSettingsOutputTypeDef",
-    "RtmpOutputSettingsOutputTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
+    "MultiplexOutputSettingsTypeDef",
+    "RtmpOutputSettingsTypeDef",
     "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
     "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
-    "AudioOnlyHlsSettingsOutputTypeDef",
-    "AvailBlankingOutputTypeDef",
-    "BlackoutSlateOutputTypeDef",
-    "BurnInDestinationSettingsOutputTypeDef",
-    "DvbSubDestinationSettingsOutputTypeDef",
-    "InputLossBehaviorOutputTypeDef",
-    "StaticImageActivateScheduleActionSettingsOutputTypeDef",
-    "StaticKeySettingsOutputTypeDef",
-    "AudioTrackSelectionOutputTypeDef",
-    "AudioTrackSelectionTypeDef",
+    "AudioOnlyHlsSettingsTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AvailSettingsOutputTypeDef",
+    "AudioTrackSelectionOutputTypeDef",
+    "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
-    "TeletextSourceSettingsOutputTypeDef",
+    "DescribeAccountConfigurationResponseTypeDef",
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateAccountConfigurationResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
+    "PurchaseOfferingRequestRequestTypeDef",
+    "UpdateReservationRequestRequestTypeDef",
     "DeleteReservationResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "DescribeChannelRequestChannelCreatedWaitTypeDef",
     "DescribeChannelRequestChannelDeletedWaitTypeDef",
@@ -609,160 +513,142 @@
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
-    "M2tsSettingsOutputTypeDef",
-    "FailoverConditionSettingsOutputTypeDef",
+    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    "ListInputsRequestListInputsPaginateTypeDef",
+    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    "M2tsSettingsTypeDef",
     "FailoverConditionSettingsTypeDef",
     "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
-    "FrameCaptureCdnSettingsOutputTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
-    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
-    "H264FilterSettingsOutputTypeDef",
-    "H265FilterSettingsOutputTypeDef",
-    "Mpeg2FilterSettingsOutputTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
     "H265ColorSpaceSettingsOutputTypeDef",
-    "VideoSelectorColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
-    "HlsCdnSettingsOutputTypeDef",
     "HlsCdnSettingsTypeDef",
-    "NetworkInputSettingsOutputTypeDef",
     "NetworkInputSettingsTypeDef",
-    "InputClippingSettingsOutputTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
-    "StandardHlsSettingsOutputTypeDef",
+    "StandardHlsSettingsTypeDef",
     "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
-    "MultiplexVideoSettingsOutputTypeDef",
     "MultiplexVideoSettingsTypeDef",
-    "NielsenWatermarksSettingsOutputTypeDef",
     "NielsenWatermarksSettingsTypeDef",
     "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
     "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
-    "PurchaseOfferingRequestRequestTypeDef",
-    "UpdateReservationRequestRequestTypeDef",
-    "Scte35SegmentationDescriptorOutputTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
     "ThumbnailDetailTypeDef",
-    "VideoSelectorSettingsOutputTypeDef",
     "VideoSelectorSettingsTypeDef",
-    "ArchiveGroupSettingsOutputTypeDef",
     "ArchiveGroupSettingsTypeDef",
     "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
     "CaptionDestinationSettingsOutputTypeDef",
-    "GlobalConfigurationOutputTypeDef",
-    "KeyProviderSettingsOutputTypeDef",
-    "AudioSelectorSettingsOutputTypeDef",
-    "AudioSelectorSettingsTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "GlobalConfigurationTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AvailConfigurationOutputTypeDef",
+    "AudioSelectorSettingsOutputTypeDef",
+    "AudioSelectorSettingsTypeDef",
     "AvailConfigurationTypeDef",
     "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
-    "ArchiveContainerSettingsOutputTypeDef",
-    "UdpContainerSettingsOutputTypeDef",
-    "FailoverConditionOutputTypeDef",
+    "ArchiveContainerSettingsTypeDef",
+    "UdpContainerSettingsTypeDef",
     "FailoverConditionTypeDef",
-    "FrameCaptureGroupSettingsOutputTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
     "H264SettingsOutputTypeDef",
-    "Mpeg2SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
     "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
     "InputPrepareScheduleActionSettingsOutputTypeDef",
-    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
-    "HlsSettingsOutputTypeDef",
+    "HlsSettingsTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
-    "MultiplexProgramSettingsOutputTypeDef",
     "MultiplexProgramSettingsTypeDef",
-    "AudioWatermarkSettingsOutputTypeDef",
     "AudioWatermarkSettingsTypeDef",
     "UpdateChannelClassRequestRequestTypeDef",
-    "Scte35DescriptorSettingsOutputTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
-    "VideoSelectorOutputTypeDef",
     "VideoSelectorTypeDef",
     "CaptionDescriptionOutputTypeDef",
+    "CaptionDescriptionTypeDef",
     "HlsGroupSettingsOutputTypeDef",
+    "HlsGroupSettingsTypeDef",
     "AudioSelectorOutputTypeDef",
     "AudioSelectorTypeDef",
-    "CaptionDescriptionTypeDef",
-    "HlsGroupSettingsTypeDef",
     "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
-    "ArchiveOutputSettingsOutputTypeDef",
-    "UdpOutputSettingsOutputTypeDef",
+    "ArchiveOutputSettingsTypeDef",
+    "UdpOutputSettingsTypeDef",
     "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
     "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
-    "HlsOutputSettingsOutputTypeDef",
+    "HlsOutputSettingsTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
+    "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
-    "CreateMultiplexProgramRequestRequestTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
     "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
-    "Scte35DescriptorOutputTypeDef",
     "Scte35DescriptorTypeDef",
     "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
     "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
     "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
-    "OutputSettingsOutputTypeDef",
+    "OutputSettingsTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
     "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
@@ -790,30 +676,14 @@
     "BatchUpdateScheduleResponseTypeDef",
     "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
-AacSettingsOutputTypeDef = TypedDict(
-    "AacSettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "CodingMode": AacCodingModeType,
-        "InputType": AacInputTypeType,
-        "Profile": AacProfileType,
-        "RateControlMode": AacRateControlModeType,
-        "RawFormat": AacRawFormatType,
-        "SampleRate": float,
-        "Spec": AacSpecType,
-        "VbrQuality": AacVbrQualityType,
-    },
-    total=False,
-)
-
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": AacCodingModeType,
         "InputType": AacInputTypeType,
         "Profile": AacProfileType,
@@ -822,28 +692,14 @@
         "SampleRate": float,
         "Spec": AacSpecType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
-Ac3SettingsOutputTypeDef = TypedDict(
-    "Ac3SettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "BitstreamMode": Ac3BitstreamModeType,
-        "CodingMode": Ac3CodingModeType,
-        "Dialnorm": int,
-        "DrcProfile": Ac3DrcProfileType,
-        "LfeFilter": Ac3LfeFilterType,
-        "MetadataControl": Ac3MetadataControlType,
-    },
-    total=False,
-)
-
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": float,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -857,155 +713,54 @@
 AcceptInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
-AccountConfigurationOutputTypeDef = TypedDict(
-    "AccountConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
 AccountConfigurationTypeDef = TypedDict(
     "AccountConfigurationTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-AncillarySourceSettingsOutputTypeDef = TypedDict(
-    "AncillarySourceSettingsOutputTypeDef",
-    {
-        "SourceAncillaryChannelNumber": int,
-    },
-    total=False,
-)
-
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "SourceAncillaryChannelNumber": int,
     },
     total=False,
 )
 
-ArchiveS3SettingsOutputTypeDef = TypedDict(
-    "ArchiveS3SettingsOutputTypeDef",
-    {
-        "CannedAcl": S3CannedAclType,
-    },
-    total=False,
-)
-
 ArchiveS3SettingsTypeDef = TypedDict(
     "ArchiveS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
-OutputLocationRefOutputTypeDef = TypedDict(
-    "OutputLocationRefOutputTypeDef",
-    {
-        "DestinationRefId": str,
-    },
-    total=False,
-)
-
 OutputLocationRefTypeDef = TypedDict(
     "OutputLocationRefTypeDef",
     {
         "DestinationRefId": str,
     },
     total=False,
 )
 
-InputChannelLevelOutputTypeDef = TypedDict(
-    "InputChannelLevelOutputTypeDef",
-    {
-        "Gain": int,
-        "InputChannel": int,
-    },
-)
-
 InputChannelLevelTypeDef = TypedDict(
     "InputChannelLevelTypeDef",
     {
         "Gain": int,
         "InputChannel": int,
     },
 )
 
-Eac3AtmosSettingsOutputTypeDef = TypedDict(
-    "Eac3AtmosSettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "CodingMode": Eac3AtmosCodingModeType,
-        "Dialnorm": int,
-        "DrcLine": Eac3AtmosDrcLineType,
-        "DrcRf": Eac3AtmosDrcRfType,
-        "HeightTrim": float,
-        "SurroundTrim": float,
-    },
-    total=False,
-)
-
-Eac3SettingsOutputTypeDef = TypedDict(
-    "Eac3SettingsOutputTypeDef",
-    {
-        "AttenuationControl": Eac3AttenuationControlType,
-        "Bitrate": float,
-        "BitstreamMode": Eac3BitstreamModeType,
-        "CodingMode": Eac3CodingModeType,
-        "DcFilter": Eac3DcFilterType,
-        "Dialnorm": int,
-        "DrcLine": Eac3DrcLineType,
-        "DrcRf": Eac3DrcRfType,
-        "LfeControl": Eac3LfeControlType,
-        "LfeFilter": Eac3LfeFilterType,
-        "LoRoCenterMixLevel": float,
-        "LoRoSurroundMixLevel": float,
-        "LtRtCenterMixLevel": float,
-        "LtRtSurroundMixLevel": float,
-        "MetadataControl": Eac3MetadataControlType,
-        "PassthroughControl": Eac3PassthroughControlType,
-        "PhaseControl": Eac3PhaseControlType,
-        "StereoDownmix": Eac3StereoDownmixType,
-        "SurroundExMode": Eac3SurroundExModeType,
-        "SurroundMode": Eac3SurroundModeType,
-    },
-    total=False,
-)
-
-Mp2SettingsOutputTypeDef = TypedDict(
-    "Mp2SettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "CodingMode": Mp2CodingModeType,
-        "SampleRate": float,
-    },
-    total=False,
-)
-
-WavSettingsOutputTypeDef = TypedDict(
-    "WavSettingsOutputTypeDef",
-    {
-        "BitDepth": float,
-        "CodingMode": WavCodingModeType,
-        "SampleRate": float,
-    },
-    total=False,
-)
-
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": Eac3AtmosCodingModeType,
         "Dialnorm": int,
         "DrcLine": Eac3AtmosDrcLineType,
@@ -1059,262 +814,109 @@
         "BitDepth": float,
         "CodingMode": WavCodingModeType,
         "SampleRate": float,
     },
     total=False,
 )
 
-AudioNormalizationSettingsOutputTypeDef = TypedDict(
-    "AudioNormalizationSettingsOutputTypeDef",
-    {
-        "Algorithm": AudioNormalizationAlgorithmType,
-        "AlgorithmControl": Literal["CORRECT_AUDIO"],
-        "TargetLkfs": float,
-    },
-    total=False,
-)
-
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": Literal["CORRECT_AUDIO"],
         "TargetLkfs": float,
     },
     total=False,
 )
 
-AudioDolbyEDecodeOutputTypeDef = TypedDict(
-    "AudioDolbyEDecodeOutputTypeDef",
-    {
-        "ProgramSelection": DolbyEProgramSelectionType,
-    },
-)
-
 AudioDolbyEDecodeTypeDef = TypedDict(
     "AudioDolbyEDecodeTypeDef",
     {
         "ProgramSelection": DolbyEProgramSelectionType,
     },
 )
 
-AudioHlsRenditionSelectionOutputTypeDef = TypedDict(
-    "AudioHlsRenditionSelectionOutputTypeDef",
-    {
-        "GroupId": str,
-        "Name": str,
-    },
-)
-
 AudioHlsRenditionSelectionTypeDef = TypedDict(
     "AudioHlsRenditionSelectionTypeDef",
     {
         "GroupId": str,
         "Name": str,
     },
 )
 
-_RequiredAudioLanguageSelectionOutputTypeDef = TypedDict(
-    "_RequiredAudioLanguageSelectionOutputTypeDef",
-    {
-        "LanguageCode": str,
-    },
-)
-_OptionalAudioLanguageSelectionOutputTypeDef = TypedDict(
-    "_OptionalAudioLanguageSelectionOutputTypeDef",
-    {
-        "LanguageSelectionPolicy": AudioLanguageSelectionPolicyType,
-    },
-    total=False,
-)
-
-
-class AudioLanguageSelectionOutputTypeDef(
-    _RequiredAudioLanguageSelectionOutputTypeDef, _OptionalAudioLanguageSelectionOutputTypeDef
-):
-    pass
-
-
 _RequiredAudioLanguageSelectionTypeDef = TypedDict(
     "_RequiredAudioLanguageSelectionTypeDef",
     {
         "LanguageCode": str,
     },
 )
 _OptionalAudioLanguageSelectionTypeDef = TypedDict(
     "_OptionalAudioLanguageSelectionTypeDef",
     {
         "LanguageSelectionPolicy": AudioLanguageSelectionPolicyType,
     },
     total=False,
 )
 
-
 class AudioLanguageSelectionTypeDef(
     _RequiredAudioLanguageSelectionTypeDef, _OptionalAudioLanguageSelectionTypeDef
 ):
     pass
 
-
-_RequiredInputLocationOutputTypeDef = TypedDict(
-    "_RequiredInputLocationOutputTypeDef",
+_RequiredInputLocationTypeDef = TypedDict(
+    "_RequiredInputLocationTypeDef",
     {
         "Uri": str,
     },
 )
-_OptionalInputLocationOutputTypeDef = TypedDict(
-    "_OptionalInputLocationOutputTypeDef",
+_OptionalInputLocationTypeDef = TypedDict(
+    "_OptionalInputLocationTypeDef",
     {
         "PasswordParam": str,
         "Username": str,
     },
     total=False,
 )
 
-
-class InputLocationOutputTypeDef(
-    _RequiredInputLocationOutputTypeDef, _OptionalInputLocationOutputTypeDef
-):
+class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
     pass
 
-
-AudioPidSelectionOutputTypeDef = TypedDict(
-    "AudioPidSelectionOutputTypeDef",
-    {
-        "Pid": int,
-    },
-)
-
 AudioPidSelectionTypeDef = TypedDict(
     "AudioPidSelectionTypeDef",
     {
         "Pid": int,
     },
 )
 
-_RequiredAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
-    "_RequiredAudioSilenceFailoverSettingsOutputTypeDef",
-    {
-        "AudioSelectorName": str,
-    },
-)
-_OptionalAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
-    "_OptionalAudioSilenceFailoverSettingsOutputTypeDef",
-    {
-        "AudioSilenceThresholdMsec": int,
-    },
-    total=False,
-)
-
-
-class AudioSilenceFailoverSettingsOutputTypeDef(
-    _RequiredAudioSilenceFailoverSettingsOutputTypeDef,
-    _OptionalAudioSilenceFailoverSettingsOutputTypeDef,
-):
-    pass
-
-
 _RequiredAudioSilenceFailoverSettingsTypeDef = TypedDict(
     "_RequiredAudioSilenceFailoverSettingsTypeDef",
     {
         "AudioSelectorName": str,
     },
 )
 _OptionalAudioSilenceFailoverSettingsTypeDef = TypedDict(
     "_OptionalAudioSilenceFailoverSettingsTypeDef",
     {
         "AudioSilenceThresholdMsec": int,
     },
     total=False,
 )
 
-
 class AudioSilenceFailoverSettingsTypeDef(
     _RequiredAudioSilenceFailoverSettingsTypeDef, _OptionalAudioSilenceFailoverSettingsTypeDef
 ):
     pass
 
-
-AudioTrackOutputTypeDef = TypedDict(
-    "AudioTrackOutputTypeDef",
-    {
-        "Track": int,
-    },
-)
-
 AudioTrackTypeDef = TypedDict(
     "AudioTrackTypeDef",
     {
         "Track": int,
     },
 )
 
-_RequiredInputLocationTypeDef = TypedDict(
-    "_RequiredInputLocationTypeDef",
-    {
-        "Uri": str,
-    },
-)
-_OptionalInputLocationTypeDef = TypedDict(
-    "_OptionalInputLocationTypeDef",
-    {
-        "PasswordParam": str,
-        "Username": str,
-    },
-    total=False,
-)
-
-
-class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
-    pass
-
-
-_RequiredEsamOutputTypeDef = TypedDict(
-    "_RequiredEsamOutputTypeDef",
-    {
-        "AcquisitionPointId": str,
-        "PoisEndpoint": str,
-    },
-)
-_OptionalEsamOutputTypeDef = TypedDict(
-    "_OptionalEsamOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "PasswordParam": str,
-        "Username": str,
-        "ZoneIdentity": str,
-    },
-    total=False,
-)
-
-
-class EsamOutputTypeDef(_RequiredEsamOutputTypeDef, _OptionalEsamOutputTypeDef):
-    pass
-
-
-Scte35SpliceInsertOutputTypeDef = TypedDict(
-    "Scte35SpliceInsertOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "NoRegionalBlackoutFlag": Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
-        "WebDeliveryAllowedFlag": Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
-    },
-    total=False,
-)
-
-Scte35TimeSignalAposOutputTypeDef = TypedDict(
-    "Scte35TimeSignalAposOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "NoRegionalBlackoutFlag": Scte35AposNoRegionalBlackoutBehaviorType,
-        "WebDeliveryAllowedFlag": Scte35AposWebDeliveryAllowedBehaviorType,
-    },
-    total=False,
-)
-
 _RequiredEsamTypeDef = TypedDict(
     "_RequiredEsamTypeDef",
     {
         "AcquisitionPointId": str,
         "PoisEndpoint": str,
     },
 )
@@ -1325,19 +927,17 @@
         "PasswordParam": str,
         "Username": str,
         "ZoneIdentity": str,
     },
     total=False,
 )
 
-
 class EsamTypeDef(_RequiredEsamTypeDef, _OptionalEsamTypeDef):
     pass
 
-
 Scte35SpliceInsertTypeDef = TypedDict(
     "Scte35SpliceInsertTypeDef",
     {
         "AdAvailOffset": int,
         "NoRegionalBlackoutFlag": Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
         "WebDeliveryAllowedFlag": Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
     },
@@ -1382,14 +982,25 @@
         "Arn": str,
         "Id": str,
         "State": str,
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
 BatchScheduleActionDeleteRequestTypeDef = TypedDict(
     "BatchScheduleActionDeleteRequestTypeDef",
     {
         "ActionNames": Sequence[str],
     },
 )
 
@@ -1414,41 +1025,14 @@
 CancelInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "CancelInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
-EbuTtDDestinationSettingsOutputTypeDef = TypedDict(
-    "EbuTtDDestinationSettingsOutputTypeDef",
-    {
-        "CopyrightHolder": str,
-        "FillLineGap": EbuTtDFillLineGapControlType,
-        "FontFamily": str,
-        "StyleControl": EbuTtDDestinationStyleControlType,
-    },
-    total=False,
-)
-
-TtmlDestinationSettingsOutputTypeDef = TypedDict(
-    "TtmlDestinationSettingsOutputTypeDef",
-    {
-        "StyleControl": TtmlDestinationStyleControlType,
-    },
-    total=False,
-)
-
-WebvttDestinationSettingsOutputTypeDef = TypedDict(
-    "WebvttDestinationSettingsOutputTypeDef",
-    {
-        "StyleControl": WebvttDestinationStyleControlType,
-    },
-    total=False,
-)
-
 EbuTtDDestinationSettingsTypeDef = TypedDict(
     "EbuTtDDestinationSettingsTypeDef",
     {
         "CopyrightHolder": str,
         "FillLineGap": EbuTtDFillLineGapControlType,
         "FontFamily": str,
         "StyleControl": EbuTtDDestinationStyleControlType,
@@ -1468,90 +1052,33 @@
     "WebvttDestinationSettingsTypeDef",
     {
         "StyleControl": WebvttDestinationStyleControlType,
     },
     total=False,
 )
 
-CaptionLanguageMappingOutputTypeDef = TypedDict(
-    "CaptionLanguageMappingOutputTypeDef",
-    {
-        "CaptionChannel": int,
-        "LanguageCode": str,
-        "LanguageDescription": str,
-    },
-)
-
 CaptionLanguageMappingTypeDef = TypedDict(
     "CaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "LanguageCode": str,
         "LanguageDescription": str,
     },
 )
 
-CaptionRectangleOutputTypeDef = TypedDict(
-    "CaptionRectangleOutputTypeDef",
-    {
-        "Height": float,
-        "LeftOffset": float,
-        "TopOffset": float,
-        "Width": float,
-    },
-)
-
 CaptionRectangleTypeDef = TypedDict(
     "CaptionRectangleTypeDef",
     {
         "Height": float,
         "LeftOffset": float,
         "TopOffset": float,
         "Width": float,
     },
 )
 
-DvbSubSourceSettingsOutputTypeDef = TypedDict(
-    "DvbSubSourceSettingsOutputTypeDef",
-    {
-        "OcrLanguage": DvbSubOcrLanguageType,
-        "Pid": int,
-    },
-    total=False,
-)
-
-EmbeddedSourceSettingsOutputTypeDef = TypedDict(
-    "EmbeddedSourceSettingsOutputTypeDef",
-    {
-        "Convert608To708": EmbeddedConvert608To708Type,
-        "Scte20Detection": EmbeddedScte20DetectionType,
-        "Source608ChannelNumber": int,
-        "Source608TrackNumber": int,
-    },
-    total=False,
-)
-
-Scte20SourceSettingsOutputTypeDef = TypedDict(
-    "Scte20SourceSettingsOutputTypeDef",
-    {
-        "Convert608To708": Scte20Convert608To708Type,
-        "Source608ChannelNumber": int,
-    },
-    total=False,
-)
-
-Scte27SourceSettingsOutputTypeDef = TypedDict(
-    "Scte27SourceSettingsOutputTypeDef",
-    {
-        "OcrLanguage": Scte27OcrLanguageType,
-        "Pid": int,
-    },
-    total=False,
-)
-
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "OcrLanguage": DvbSubOcrLanguageType,
         "Pid": int,
     },
     total=False,
@@ -1582,22 +1109,14 @@
     {
         "OcrLanguage": Scte27OcrLanguageType,
         "Pid": int,
     },
     total=False,
 )
 
-CdiInputSpecificationOutputTypeDef = TypedDict(
-    "CdiInputSpecificationOutputTypeDef",
-    {
-        "Resolution": CdiInputResolutionType,
-    },
-    total=False,
-)
-
 CdiInputSpecificationTypeDef = TypedDict(
     "CdiInputSpecificationTypeDef",
     {
         "Resolution": CdiInputResolutionType,
     },
     total=False,
 )
@@ -1606,16 +1125,16 @@
     "ChannelEgressEndpointTypeDef",
     {
         "SourceIp": str,
     },
     total=False,
 )
 
-InputSpecificationOutputTypeDef = TypedDict(
-    "InputSpecificationOutputTypeDef",
+InputSpecificationTypeDef = TypedDict(
+    "InputSpecificationTypeDef",
     {
         "Codec": InputCodecType,
         "MaximumBitrate": InputMaximumBitrateType,
         "Resolution": InputResolutionType,
     },
     total=False,
 )
@@ -1658,24 +1177,14 @@
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-InputSpecificationTypeDef = TypedDict(
-    "InputSpecificationTypeDef",
-    {
-        "Codec": InputCodecType,
-        "MaximumBitrate": InputMaximumBitrateType,
-        "Resolution": InputResolutionType,
-    },
-    total=False,
-)
-
 MaintenanceCreateSettingsTypeDef = TypedDict(
     "MaintenanceCreateSettingsTypeDef",
     {
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceStartTime": str,
     },
     total=False,
@@ -1692,21 +1201,19 @@
     {
         "PublicAddressAllocationIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcOutputSettingsTypeDef(
     _RequiredVpcOutputSettingsTypeDef, _OptionalVpcOutputSettingsTypeDef
 ):
     pass
 
-
 InputDestinationRequestTypeDef = TypedDict(
     "InputDestinationRequestTypeDef",
     {
         "StreamName": str,
     },
     total=False,
 )
@@ -1739,19 +1246,17 @@
     "_OptionalInputVpcRequestTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class InputVpcRequestTypeDef(_RequiredInputVpcRequestTypeDef, _OptionalInputVpcRequestTypeDef):
     pass
 
-
 MediaConnectFlowRequestTypeDef = TypedDict(
     "MediaConnectFlowRequestTypeDef",
     {
         "FlowArn": str,
     },
     total=False,
 )
@@ -1776,21 +1281,19 @@
     {
         "MaximumVideoBufferDelayMilliseconds": int,
         "TransportStreamReservedBitrate": int,
     },
     total=False,
 )
 
-
 class MultiplexSettingsTypeDef(
     _RequiredMultiplexSettingsTypeDef, _OptionalMultiplexSettingsTypeDef
 ):
     pass
 
-
 _RequiredCreatePartnerInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartnerInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalCreatePartnerInputRequestRequestTypeDef = TypedDict(
@@ -1798,43 +1301,39 @@
     {
         "RequestId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePartnerInputRequestRequestTypeDef(
     _RequiredCreatePartnerInputRequestRequestTypeDef,
     _OptionalCreatePartnerInputRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateTagsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalCreateTagsRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTagsRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateTagsRequestRequestTypeDef(
     _RequiredCreateTagsRequestRequestTypeDef, _OptionalCreateTagsRequestRequestTypeDef
 ):
     pass
 
-
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 
@@ -1892,46 +1391,23 @@
 DeleteMultiplexRequestRequestTypeDef = TypedDict(
     "DeleteMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 
-_RequiredMultiplexSettingsOutputTypeDef = TypedDict(
-    "_RequiredMultiplexSettingsOutputTypeDef",
-    {
-        "TransportStreamBitrate": int,
-        "TransportStreamId": int,
-    },
-)
-_OptionalMultiplexSettingsOutputTypeDef = TypedDict(
-    "_OptionalMultiplexSettingsOutputTypeDef",
-    {
-        "MaximumVideoBufferDelayMilliseconds": int,
-        "TransportStreamReservedBitrate": int,
-    },
-    total=False,
-)
-
-
-class MultiplexSettingsOutputTypeDef(
-    _RequiredMultiplexSettingsOutputTypeDef, _OptionalMultiplexSettingsOutputTypeDef
-):
-    pass
-
-
 DeleteReservationRequestRequestTypeDef = TypedDict(
     "DeleteReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-RenewalSettingsOutputTypeDef = TypedDict(
-    "RenewalSettingsOutputTypeDef",
+RenewalSettingsTypeDef = TypedDict(
+    "RenewalSettingsTypeDef",
     {
         "AutomaticRenewal": ReservationAutomaticRenewalType,
         "RenewalCount": int,
     },
     total=False,
 )
 
@@ -2036,41 +1512,21 @@
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
     {
         "InputDeviceId": str,
         "Accept": Literal["image/jpeg"],
     },
 )
 
-DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ContentType": Literal["image/jpeg"],
-        "ContentLength": int,
-        "ETag": str,
-        "LastModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 
-InputDeviceSettingsOutputTypeDef = TypedDict(
-    "InputDeviceSettingsOutputTypeDef",
-    {
-        "Id": str,
-    },
-    total=False,
-)
-
 InputSourceTypeDef = TypedDict(
     "InputSourceTypeDef",
     {
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
@@ -2125,36 +1581,24 @@
 DescribeReservationRequestRequestTypeDef = TypedDict(
     "DescribeReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "ChannelId": str,
-    },
-)
-_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
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
-class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
-    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeScheduleRequestRequestTypeDef = TypedDict(
@@ -2162,123 +1606,65 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScheduleRequestRequestTypeDef(
     _RequiredDescribeScheduleRequestRequestTypeDef, _OptionalDescribeScheduleRequestRequestTypeDef
 ):
     pass
 
-
 DescribeThumbnailsRequestRequestTypeDef = TypedDict(
     "DescribeThumbnailsRequestRequestTypeDef",
     {
         "ChannelId": str,
         "PipelineId": str,
         "ThumbnailType": str,
     },
 )
 
-_RequiredDvbNitSettingsOutputTypeDef = TypedDict(
-    "_RequiredDvbNitSettingsOutputTypeDef",
+_RequiredDvbNitSettingsTypeDef = TypedDict(
+    "_RequiredDvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
     },
 )
-_OptionalDvbNitSettingsOutputTypeDef = TypedDict(
-    "_OptionalDvbNitSettingsOutputTypeDef",
+_OptionalDvbNitSettingsTypeDef = TypedDict(
+    "_OptionalDvbNitSettingsTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
-
-class DvbNitSettingsOutputTypeDef(
-    _RequiredDvbNitSettingsOutputTypeDef, _OptionalDvbNitSettingsOutputTypeDef
-):
+class DvbNitSettingsTypeDef(_RequiredDvbNitSettingsTypeDef, _OptionalDvbNitSettingsTypeDef):
     pass
 
-
-DvbSdtSettingsOutputTypeDef = TypedDict(
-    "DvbSdtSettingsOutputTypeDef",
+DvbSdtSettingsTypeDef = TypedDict(
+    "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": DvbSdtOutputSdtType,
         "RepInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
-DvbTdtSettingsOutputTypeDef = TypedDict(
-    "DvbTdtSettingsOutputTypeDef",
+DvbTdtSettingsTypeDef = TypedDict(
+    "DvbTdtSettingsTypeDef",
     {
         "RepInterval": int,
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
-FeatureActivationsOutputTypeDef = TypedDict(
-    "FeatureActivationsOutputTypeDef",
-    {
-        "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
-    },
-    total=False,
-)
-
-NielsenConfigurationOutputTypeDef = TypedDict(
-    "NielsenConfigurationOutputTypeDef",
-    {
-        "DistributorId": str,
-        "NielsenPcmToId3Tagging": NielsenPcmToId3TaggingStateType,
-    },
-    total=False,
-)
-
-ThumbnailConfigurationOutputTypeDef = TypedDict(
-    "ThumbnailConfigurationOutputTypeDef",
-    {
-        "State": ThumbnailStateType,
-    },
-)
-
-_RequiredTimecodeConfigOutputTypeDef = TypedDict(
-    "_RequiredTimecodeConfigOutputTypeDef",
-    {
-        "Source": TimecodeConfigSourceType,
-    },
-)
-_OptionalTimecodeConfigOutputTypeDef = TypedDict(
-    "_OptionalTimecodeConfigOutputTypeDef",
-    {
-        "SyncThreshold": int,
-    },
-    total=False,
-)
-
-
-class TimecodeConfigOutputTypeDef(
-    _RequiredTimecodeConfigOutputTypeDef, _OptionalTimecodeConfigOutputTypeDef
-):
-    pass
-
-
 FeatureActivationsTypeDef = TypedDict(
     "FeatureActivationsTypeDef",
     {
         "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
     },
     total=False,
 )
@@ -2309,36 +1695,17 @@
     "_OptionalTimecodeConfigTypeDef",
     {
         "SyncThreshold": int,
     },
     total=False,
 )
 
-
 class TimecodeConfigTypeDef(_RequiredTimecodeConfigTypeDef, _OptionalTimecodeConfigTypeDef):
     pass
 
-
-InputLossFailoverSettingsOutputTypeDef = TypedDict(
-    "InputLossFailoverSettingsOutputTypeDef",
-    {
-        "InputLossThresholdMsec": int,
-    },
-    total=False,
-)
-
-VideoBlackFailoverSettingsOutputTypeDef = TypedDict(
-    "VideoBlackFailoverSettingsOutputTypeDef",
-    {
-        "BlackDetectThreshold": float,
-        "VideoBlackThresholdMsec": int,
-    },
-    total=False,
-)
-
 InputLossFailoverSettingsTypeDef = TypedDict(
     "InputLossFailoverSettingsTypeDef",
     {
         "InputLossThresholdMsec": int,
     },
     total=False,
 )
@@ -2348,110 +1715,65 @@
     {
         "BlackDetectThreshold": float,
         "VideoBlackThresholdMsec": int,
     },
     total=False,
 )
 
-FecOutputSettingsOutputTypeDef = TypedDict(
-    "FecOutputSettingsOutputTypeDef",
+FecOutputSettingsTypeDef = TypedDict(
+    "FecOutputSettingsTypeDef",
     {
         "ColumnDepth": int,
         "IncludeFec": FecOutputIncludeFecType,
         "RowLength": int,
     },
     total=False,
 )
 
-FixedModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
-    "FixedModeScheduleActionStartSettingsOutputTypeDef",
-    {
-        "Time": str,
-    },
-)
-
 FixedModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FixedModeScheduleActionStartSettingsTypeDef",
     {
         "Time": str,
     },
 )
 
-Fmp4HlsSettingsOutputTypeDef = TypedDict(
-    "Fmp4HlsSettingsOutputTypeDef",
+Fmp4HlsSettingsTypeDef = TypedDict(
+    "Fmp4HlsSettingsTypeDef",
     {
         "AudioRenditionSets": str,
         "NielsenId3Behavior": Fmp4NielsenId3BehaviorType,
         "TimedMetadataBehavior": Fmp4TimedMetadataBehaviorType,
     },
     total=False,
 )
 
-FollowModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
-    "FollowModeScheduleActionStartSettingsOutputTypeDef",
-    {
-        "FollowPoint": FollowPointType,
-        "ReferenceActionName": str,
-    },
-)
-
 FollowModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FollowModeScheduleActionStartSettingsTypeDef",
     {
         "FollowPoint": FollowPointType,
         "ReferenceActionName": str,
     },
 )
 
-FrameCaptureS3SettingsOutputTypeDef = TypedDict(
-    "FrameCaptureS3SettingsOutputTypeDef",
-    {
-        "CannedAcl": S3CannedAclType,
-    },
-    total=False,
-)
-
 FrameCaptureS3SettingsTypeDef = TypedDict(
     "FrameCaptureS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
-FrameCaptureOutputSettingsOutputTypeDef = TypedDict(
-    "FrameCaptureOutputSettingsOutputTypeDef",
+FrameCaptureOutputSettingsTypeDef = TypedDict(
+    "FrameCaptureOutputSettingsTypeDef",
     {
         "NameModifier": str,
     },
     total=False,
 )
 
-_RequiredTimecodeBurninSettingsOutputTypeDef = TypedDict(
-    "_RequiredTimecodeBurninSettingsOutputTypeDef",
-    {
-        "FontSize": TimecodeBurninFontSizeType,
-        "Position": TimecodeBurninPositionType,
-    },
-)
-_OptionalTimecodeBurninSettingsOutputTypeDef = TypedDict(
-    "_OptionalTimecodeBurninSettingsOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-
-class TimecodeBurninSettingsOutputTypeDef(
-    _RequiredTimecodeBurninSettingsOutputTypeDef, _OptionalTimecodeBurninSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredTimecodeBurninSettingsTypeDef = TypedDict(
     "_RequiredTimecodeBurninSettingsTypeDef",
     {
         "FontSize": TimecodeBurninFontSizeType,
         "Position": TimecodeBurninPositionType,
     },
 )
@@ -2459,21 +1781,19 @@
     "_OptionalTimecodeBurninSettingsTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
-
 class TimecodeBurninSettingsTypeDef(
     _RequiredTimecodeBurninSettingsTypeDef, _OptionalTimecodeBurninSettingsTypeDef
 ):
     pass
 
-
 H264ColorSpaceSettingsOutputTypeDef = TypedDict(
     "H264ColorSpaceSettingsOutputTypeDef",
     {
         "ColorSpacePassthroughSettings": Dict[str, Any],
         "Rec601Settings": Dict[str, Any],
         "Rec709Settings": Dict[str, Any],
     },
@@ -2486,132 +1806,57 @@
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "Rec601Settings": Mapping[str, Any],
         "Rec709Settings": Mapping[str, Any],
     },
     total=False,
 )
 
-TemporalFilterSettingsOutputTypeDef = TypedDict(
-    "TemporalFilterSettingsOutputTypeDef",
-    {
-        "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
-        "Strength": TemporalFilterStrengthType,
-    },
-    total=False,
-)
-
 TemporalFilterSettingsTypeDef = TypedDict(
     "TemporalFilterSettingsTypeDef",
     {
         "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
         "Strength": TemporalFilterStrengthType,
     },
     total=False,
 )
 
-Hdr10SettingsOutputTypeDef = TypedDict(
-    "Hdr10SettingsOutputTypeDef",
-    {
-        "MaxCll": int,
-        "MaxFall": int,
-    },
-    total=False,
-)
-
 Hdr10SettingsTypeDef = TypedDict(
     "Hdr10SettingsTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
-HlsAkamaiSettingsOutputTypeDef = TypedDict(
-    "HlsAkamaiSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "HttpTransferMode": HlsAkamaiHttpTransferModeType,
-        "NumRetries": int,
-        "RestartDelay": int,
-        "Salt": str,
-        "Token": str,
-    },
-    total=False,
-)
-
 HlsAkamaiSettingsTypeDef = TypedDict(
     "HlsAkamaiSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "HttpTransferMode": HlsAkamaiHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
         "Salt": str,
         "Token": str,
     },
     total=False,
 )
 
-HlsBasicPutSettingsOutputTypeDef = TypedDict(
-    "HlsBasicPutSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "NumRetries": int,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
 HlsBasicPutSettingsTypeDef = TypedDict(
     "HlsBasicPutSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
-HlsMediaStoreSettingsOutputTypeDef = TypedDict(
-    "HlsMediaStoreSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "MediaStoreStorageClass": Literal["TEMPORAL"],
-        "NumRetries": int,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
-HlsS3SettingsOutputTypeDef = TypedDict(
-    "HlsS3SettingsOutputTypeDef",
-    {
-        "CannedAcl": S3CannedAclType,
-    },
-    total=False,
-)
-
-HlsWebdavSettingsOutputTypeDef = TypedDict(
-    "HlsWebdavSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "HttpTransferMode": HlsWebdavHttpTransferModeType,
-        "NumRetries": int,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
 HlsMediaStoreSettingsTypeDef = TypedDict(
     "HlsMediaStoreSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "MediaStoreStorageClass": Literal["TEMPORAL"],
         "NumRetries": int,
@@ -2636,87 +1881,42 @@
         "HttpTransferMode": HlsWebdavHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
-HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef = TypedDict(
-    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
-    {
-        "Tag": str,
-        "Id3": str,
-    },
-    total=False,
-)
-
 HlsId3SegmentTaggingScheduleActionSettingsTypeDef = TypedDict(
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
     {
         "Tag": str,
         "Id3": str,
     },
     total=False,
 )
 
-HlsInputSettingsOutputTypeDef = TypedDict(
-    "HlsInputSettingsOutputTypeDef",
-    {
-        "Bandwidth": int,
-        "BufferSegments": int,
-        "Retries": int,
-        "RetryInterval": int,
-        "Scte35Source": HlsScte35SourceTypeType,
-    },
-    total=False,
-)
-
 HlsInputSettingsTypeDef = TypedDict(
     "HlsInputSettingsTypeDef",
     {
         "Bandwidth": int,
         "BufferSegments": int,
         "Retries": int,
         "RetryInterval": int,
         "Scte35Source": HlsScte35SourceTypeType,
     },
     total=False,
 )
 
-HlsTimedMetadataScheduleActionSettingsOutputTypeDef = TypedDict(
-    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
-    {
-        "Id3": str,
-    },
-)
-
 HlsTimedMetadataScheduleActionSettingsTypeDef = TypedDict(
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
     {
         "Id3": str,
     },
 )
 
-StartTimecodeOutputTypeDef = TypedDict(
-    "StartTimecodeOutputTypeDef",
-    {
-        "Timecode": str,
-    },
-    total=False,
-)
-
-StopTimecodeOutputTypeDef = TypedDict(
-    "StopTimecodeOutputTypeDef",
-    {
-        "LastFrameClippingBehavior": LastFrameClippingBehaviorType,
-        "Timecode": str,
-    },
-    total=False,
-)
-
 StartTimecodeTypeDef = TypedDict(
     "StartTimecodeTypeDef",
     {
         "Timecode": str,
     },
     total=False,
 )
@@ -2753,53 +1953,23 @@
     "InputDeviceRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "TransferType": str,
-    },
-)
-_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
-    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "_RequiredListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
     },
 )
 _OptionalListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
@@ -2807,106 +1977,58 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListInputDeviceTransfersRequestRequestTypeDef(
     _RequiredListInputDeviceTransfersRequestRequestTypeDef,
     _OptionalListInputDeviceTransfersRequestRequestTypeDef,
 ):
     pass
 
-
 TransferringInputDeviceSummaryTypeDef = TypedDict(
     "TransferringInputDeviceSummaryTypeDef",
     {
         "Id": str,
         "Message": str,
         "TargetCustomerId": str,
         "TransferType": InputDeviceTransferTypeType,
     },
     total=False,
 )
 
-ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInputDevicesRequestRequestTypeDef = TypedDict(
     "ListInputDevicesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInputSecurityGroupsRequestRequestTypeDef = TypedDict(
     "ListInputSecurityGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListInputsRequestListInputsPaginateTypeDef = TypedDict(
-    "ListInputsRequestListInputsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInputsRequestRequestTypeDef = TypedDict(
     "ListInputsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "MultiplexId": str,
-    },
-)
-_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
-    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMultiplexProgramsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiplexProgramsRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalListMultiplexProgramsRequestRequestTypeDef = TypedDict(
@@ -2914,66 +2036,38 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListMultiplexProgramsRequestRequestTypeDef(
     _RequiredListMultiplexProgramsRequestRequestTypeDef,
     _OptionalListMultiplexProgramsRequestRequestTypeDef,
 ):
     pass
 
-
 MultiplexProgramSummaryTypeDef = TypedDict(
     "MultiplexProgramSummaryTypeDef",
     {
         "ChannelId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
-ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMultiplexesRequestRequestTypeDef = TypedDict(
     "ListMultiplexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "ChannelConfiguration": str,
-        "Codec": str,
-        "Duration": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "ChannelConfiguration": str,
         "Codec": str,
         "Duration": str,
@@ -2985,30 +2079,14 @@
         "ResourceType": str,
         "SpecialFeature": str,
         "VideoQuality": str,
     },
     total=False,
 )
 
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "Codec": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "Codec": str,
         "MaxResults": int,
         "MaximumBitrate": str,
@@ -3025,24 +2103,16 @@
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
-M3u8SettingsOutputTypeDef = TypedDict(
-    "M3u8SettingsOutputTypeDef",
+M3u8SettingsTypeDef = TypedDict(
+    "M3u8SettingsTypeDef",
     {
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "EcmPid": str,
         "NielsenId3Behavior": M3u8NielsenId3BehaviorType,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
@@ -3067,41 +2137,22 @@
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceScheduledDate": str,
         "MaintenanceStartTime": str,
     },
     total=False,
 )
 
-MediaPackageOutputDestinationSettingsOutputTypeDef = TypedDict(
-    "MediaPackageOutputDestinationSettingsOutputTypeDef",
-    {
-        "ChannelId": str,
-    },
-    total=False,
-)
-
 MediaPackageOutputDestinationSettingsTypeDef = TypedDict(
     "MediaPackageOutputDestinationSettingsTypeDef",
     {
         "ChannelId": str,
     },
     total=False,
 )
 
-MotionGraphicsActivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
-    {
-        "Duration": int,
-        "PasswordParam": str,
-        "Url": str,
-        "Username": str,
-    },
-    total=False,
-)
-
 MotionGraphicsActivateScheduleActionSettingsTypeDef = TypedDict(
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     {
         "Duration": int,
         "PasswordParam": str,
         "Url": str,
         "Username": str,
@@ -3121,16 +2172,16 @@
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-MsSmoothOutputSettingsOutputTypeDef = TypedDict(
-    "MsSmoothOutputSettingsOutputTypeDef",
+MsSmoothOutputSettingsTypeDef = TypedDict(
+    "MsSmoothOutputSettingsTypeDef",
     {
         "H265PackagingType": MsSmoothH265PackagingTypeType,
         "NameModifier": str,
     },
     total=False,
 )
 
@@ -3138,40 +2189,23 @@
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     {
         "EntitlementArn": str,
     },
     total=False,
 )
 
-MultiplexProgramChannelDestinationSettingsOutputTypeDef = TypedDict(
-    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
-    {
-        "MultiplexId": str,
-        "ProgramName": str,
-    },
-    total=False,
-)
-
 MultiplexProgramChannelDestinationSettingsTypeDef = TypedDict(
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
-MultiplexProgramServiceDescriptorOutputTypeDef = TypedDict(
-    "MultiplexProgramServiceDescriptorOutputTypeDef",
-    {
-        "ProviderName": str,
-        "ServiceName": str,
-    },
-)
-
 MultiplexProgramServiceDescriptorTypeDef = TypedDict(
     "MultiplexProgramServiceDescriptorTypeDef",
     {
         "ProviderName": str,
         "ServiceName": str,
     },
 )
@@ -3180,74 +2214,33 @@
     "MultiplexSettingsSummaryTypeDef",
     {
         "TransportStreamBitrate": int,
     },
     total=False,
 )
 
-MultiplexStatmuxVideoSettingsOutputTypeDef = TypedDict(
-    "MultiplexStatmuxVideoSettingsOutputTypeDef",
-    {
-        "MaximumBitrate": int,
-        "MinimumBitrate": int,
-        "Priority": int,
-    },
-    total=False,
-)
-
 MultiplexStatmuxVideoSettingsTypeDef = TypedDict(
     "MultiplexStatmuxVideoSettingsTypeDef",
     {
         "MaximumBitrate": int,
         "MinimumBitrate": int,
         "Priority": int,
     },
     total=False,
 )
 
-NielsenCBETOutputTypeDef = TypedDict(
-    "NielsenCBETOutputTypeDef",
-    {
-        "CbetCheckDigitString": str,
-        "CbetStepaside": NielsenWatermarksCbetStepasideType,
-        "Csid": str,
-    },
-)
-
 NielsenCBETTypeDef = TypedDict(
     "NielsenCBETTypeDef",
     {
         "CbetCheckDigitString": str,
         "CbetStepaside": NielsenWatermarksCbetStepasideType,
         "Csid": str,
     },
 )
 
-_RequiredNielsenNaesIiNwOutputTypeDef = TypedDict(
-    "_RequiredNielsenNaesIiNwOutputTypeDef",
-    {
-        "CheckDigitString": str,
-        "Sid": float,
-    },
-)
-_OptionalNielsenNaesIiNwOutputTypeDef = TypedDict(
-    "_OptionalNielsenNaesIiNwOutputTypeDef",
-    {
-        "Timezone": NielsenWatermarkTimezonesType,
-    },
-    total=False,
-)
-
-
-class NielsenNaesIiNwOutputTypeDef(
-    _RequiredNielsenNaesIiNwOutputTypeDef, _OptionalNielsenNaesIiNwOutputTypeDef
-):
-    pass
-
-
 _RequiredNielsenNaesIiNwTypeDef = TypedDict(
     "_RequiredNielsenNaesIiNwTypeDef",
     {
         "CheckDigitString": str,
         "Sid": float,
     },
 )
@@ -3255,30 +2248,17 @@
     "_OptionalNielsenNaesIiNwTypeDef",
     {
         "Timezone": NielsenWatermarkTimezonesType,
     },
     total=False,
 )
 
-
 class NielsenNaesIiNwTypeDef(_RequiredNielsenNaesIiNwTypeDef, _OptionalNielsenNaesIiNwTypeDef):
     pass
 
-
-OutputDestinationSettingsOutputTypeDef = TypedDict(
-    "OutputDestinationSettingsOutputTypeDef",
-    {
-        "PasswordParam": str,
-        "StreamName": str,
-        "Url": str,
-        "Username": str,
-    },
-    total=False,
-)
-
 OutputDestinationSettingsTypeDef = TypedDict(
     "OutputDestinationSettingsTypeDef",
     {
         "PasswordParam": str,
         "StreamName": str,
         "Url": str,
         "Username": str,
@@ -3296,16 +2276,16 @@
         "CaptionData": RtmpCaptionDataType,
         "InputLossAction": InputLossActionForRtmpOutType,
         "RestartDelay": int,
     },
     total=False,
 )
 
-UdpGroupSettingsOutputTypeDef = TypedDict(
-    "UdpGroupSettingsOutputTypeDef",
+UdpGroupSettingsTypeDef = TypedDict(
+    "UdpGroupSettingsTypeDef",
     {
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
     },
     total=False,
 )
@@ -3320,178 +2300,67 @@
         "CaptionData": RtmpCaptionDataType,
         "InputLossAction": InputLossActionForRtmpOutType,
         "RestartDelay": int,
     },
     total=False,
 )
 
-UdpGroupSettingsTypeDef = TypedDict(
-    "UdpGroupSettingsTypeDef",
-    {
-        "InputLossAction": InputLossActionForUdpOutType,
-        "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-    },
-    total=False,
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
-PipelinePauseStateSettingsOutputTypeDef = TypedDict(
-    "PipelinePauseStateSettingsOutputTypeDef",
-    {
-        "PipelineId": PipelineIdType,
-    },
-)
-
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
-RenewalSettingsTypeDef = TypedDict(
-    "RenewalSettingsTypeDef",
-    {
-        "AutomaticRenewal": ReservationAutomaticRenewalType,
-        "RenewalCount": int,
-    },
-    total=False,
-)
-
 _RequiredRebootInputDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredRebootInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 _OptionalRebootInputDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalRebootInputDeviceRequestRequestTypeDef",
     {
         "Force": RebootInputDeviceForceType,
     },
     total=False,
 )
 
-
 class RebootInputDeviceRequestRequestTypeDef(
     _RequiredRebootInputDeviceRequestRequestTypeDef, _OptionalRebootInputDeviceRequestRequestTypeDef
 ):
     pass
 
-
 RejectInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "RejectInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
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
-_RequiredScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredScte35InputScheduleActionSettingsOutputTypeDef",
-    {
-        "Mode": Scte35InputModeType,
-    },
-)
-_OptionalScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalScte35InputScheduleActionSettingsOutputTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-    },
-    total=False,
-)
-
-
-class Scte35InputScheduleActionSettingsOutputTypeDef(
-    _RequiredScte35InputScheduleActionSettingsOutputTypeDef,
-    _OptionalScte35InputScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
-
-Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef = TypedDict(
-    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
-    {
-        "SpliceEventId": int,
-    },
-)
-
-_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
-    {
-        "SpliceEventId": int,
-    },
-)
-_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
-    {
-        "Duration": int,
-    },
-    total=False,
-)
-
-
-class Scte35SpliceInsertScheduleActionSettingsOutputTypeDef(
-    _RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-    _OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
-
-StaticImageDeactivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
-    {
-        "FadeOut": int,
-        "Layer": int,
-    },
-    total=False,
-)
-
 _RequiredScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredScte35InputScheduleActionSettingsTypeDef",
     {
         "Mode": Scte35InputModeType,
     },
 )
 _OptionalScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_OptionalScte35InputScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
     total=False,
 )
 
-
 class Scte35InputScheduleActionSettingsTypeDef(
     _RequiredScte35InputScheduleActionSettingsTypeDef,
     _OptionalScte35InputScheduleActionSettingsTypeDef,
 ):
     pass
 
-
 Scte35ReturnToNetworkScheduleActionSettingsTypeDef = TypedDict(
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     {
         "SpliceEventId": int,
     },
 )
 
@@ -3505,41 +2374,29 @@
     "_OptionalScte35SpliceInsertScheduleActionSettingsTypeDef",
     {
         "Duration": int,
     },
     total=False,
 )
 
-
 class Scte35SpliceInsertScheduleActionSettingsTypeDef(
     _RequiredScte35SpliceInsertScheduleActionSettingsTypeDef,
     _OptionalScte35SpliceInsertScheduleActionSettingsTypeDef,
 ):
     pass
 
-
 StaticImageDeactivateScheduleActionSettingsTypeDef = TypedDict(
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     {
         "FadeOut": int,
         "Layer": int,
     },
     total=False,
 )
 
-Scte35DeliveryRestrictionsOutputTypeDef = TypedDict(
-    "Scte35DeliveryRestrictionsOutputTypeDef",
-    {
-        "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
-        "DeviceRestrictions": Scte35DeviceRestrictionsType,
-        "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
-        "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
-    },
-)
-
 Scte35DeliveryRestrictionsTypeDef = TypedDict(
     "Scte35DeliveryRestrictionsTypeDef",
     {
         "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
         "DeviceRestrictions": Scte35DeviceRestrictionsType,
         "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
         "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
@@ -3604,109 +2461,67 @@
         "TargetCustomerId": str,
         "TargetRegion": str,
         "TransferMessage": str,
     },
     total=False,
 )
 
-
 class TransferInputDeviceRequestRequestTypeDef(
     _RequiredTransferInputDeviceRequestRequestTypeDef,
     _OptionalTransferInputDeviceRequestRequestTypeDef,
 ):
     pass
 
-
-VideoSelectorPidOutputTypeDef = TypedDict(
-    "VideoSelectorPidOutputTypeDef",
-    {
-        "Pid": int,
-    },
-    total=False,
-)
-
 VideoSelectorPidTypeDef = TypedDict(
     "VideoSelectorPidTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
 
-VideoSelectorProgramIdOutputTypeDef = TypedDict(
-    "VideoSelectorProgramIdOutputTypeDef",
-    {
-        "ProgramId": int,
-    },
-    total=False,
-)
-
 VideoSelectorProgramIdTypeDef = TypedDict(
     "VideoSelectorProgramIdTypeDef",
     {
         "ProgramId": int,
     },
     total=False,
 )
 
-DescribeAccountConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccountConfigurationResponseTypeDef",
-    {
-        "AccountConfiguration": AccountConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
-    {
-        "AccountConfiguration": AccountConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
     },
     total=False,
 )
 
-ArchiveCdnSettingsOutputTypeDef = TypedDict(
-    "ArchiveCdnSettingsOutputTypeDef",
-    {
-        "ArchiveS3Settings": ArchiveS3SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": ArchiveS3SettingsTypeDef,
     },
     total=False,
 )
 
-MediaPackageGroupSettingsOutputTypeDef = TypedDict(
-    "MediaPackageGroupSettingsOutputTypeDef",
+MediaPackageGroupSettingsTypeDef = TypedDict(
+    "MediaPackageGroupSettingsTypeDef",
     {
-        "Destination": OutputLocationRefOutputTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
 
-_RequiredMsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredMsSmoothGroupSettingsOutputTypeDef",
+_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_RequiredMsSmoothGroupSettingsTypeDef",
     {
-        "Destination": OutputLocationRefOutputTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalMsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalMsSmoothGroupSettingsOutputTypeDef",
+_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_OptionalMsSmoothGroupSettingsTypeDef",
     {
         "AcquisitionPointId": str,
         "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
         "CertificateMode": SmoothGroupCertificateModeType,
         "ConnectionRetryInterval": int,
         "EventId": str,
         "EventIdMode": SmoothGroupEventIdModeType,
@@ -3722,100 +2537,51 @@
         "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
         "TimestampOffset": str,
         "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
-
-class MsSmoothGroupSettingsOutputTypeDef(
-    _RequiredMsSmoothGroupSettingsOutputTypeDef, _OptionalMsSmoothGroupSettingsOutputTypeDef
-):
-    pass
-
-
-MultiplexOutputSettingsOutputTypeDef = TypedDict(
-    "MultiplexOutputSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-
-_RequiredRtmpOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredRtmpOutputSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-_OptionalRtmpOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalRtmpOutputSettingsOutputTypeDef",
-    {
-        "CertificateMode": RtmpOutputCertificateModeType,
-        "ConnectionRetryInterval": int,
-        "NumRetries": int,
-    },
-    total=False,
-)
-
-
-class RtmpOutputSettingsOutputTypeDef(
-    _RequiredRtmpOutputSettingsOutputTypeDef, _OptionalRtmpOutputSettingsOutputTypeDef
+class MsSmoothGroupSettingsTypeDef(
+    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
 ):
     pass
 
-
-MediaPackageGroupSettingsTypeDef = TypedDict(
-    "MediaPackageGroupSettingsTypeDef",
+MultiplexOutputSettingsTypeDef = TypedDict(
+    "MultiplexOutputSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 
-_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_RequiredMsSmoothGroupSettingsTypeDef",
+_RequiredRtmpOutputSettingsTypeDef = TypedDict(
+    "_RequiredRtmpOutputSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_OptionalMsSmoothGroupSettingsTypeDef",
+_OptionalRtmpOutputSettingsTypeDef = TypedDict(
+    "_OptionalRtmpOutputSettingsTypeDef",
     {
-        "AcquisitionPointId": str,
-        "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
-        "CertificateMode": SmoothGroupCertificateModeType,
+        "CertificateMode": RtmpOutputCertificateModeType,
         "ConnectionRetryInterval": int,
-        "EventId": str,
-        "EventIdMode": SmoothGroupEventIdModeType,
-        "EventStopBehavior": SmoothGroupEventStopBehaviorType,
-        "FilecacheDuration": int,
-        "FragmentLength": int,
-        "InputLossAction": InputLossActionForMsSmoothOutType,
         "NumRetries": int,
-        "RestartDelay": int,
-        "SegmentationMode": SmoothGroupSegmentationModeType,
-        "SendDelayMs": int,
-        "SparseTrackType": SmoothGroupSparseTrackTypeType,
-        "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
-        "TimestampOffset": str,
-        "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
-
-class MsSmoothGroupSettingsTypeDef(
-    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
+class RtmpOutputSettingsTypeDef(
+    _RequiredRtmpOutputSettingsTypeDef, _OptionalRtmpOutputSettingsTypeDef
 ):
     pass
 
-
 AudioChannelMappingOutputTypeDef = TypedDict(
     "AudioChannelMappingOutputTypeDef",
     {
-        "InputChannelLevels": List[InputChannelLevelOutputTypeDef],
+        "InputChannelLevels": List[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
 
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
@@ -3823,21 +2589,21 @@
         "OutputChannel": int,
     },
 )
 
 AudioCodecSettingsOutputTypeDef = TypedDict(
     "AudioCodecSettingsOutputTypeDef",
     {
-        "AacSettings": AacSettingsOutputTypeDef,
-        "Ac3Settings": Ac3SettingsOutputTypeDef,
-        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
-        "Eac3Settings": Eac3SettingsOutputTypeDef,
-        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "AacSettings": AacSettingsTypeDef,
+        "Ac3Settings": Ac3SettingsTypeDef,
+        "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
+        "Eac3Settings": Eac3SettingsTypeDef,
+        "Mp2Settings": Mp2SettingsTypeDef,
         "PassThroughSettings": Dict[str, Any],
-        "WavSettings": WavSettingsOutputTypeDef,
+        "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
@@ -3848,199 +2614,25 @@
         "Mp2Settings": Mp2SettingsTypeDef,
         "PassThroughSettings": Mapping[str, Any],
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
-AudioOnlyHlsSettingsOutputTypeDef = TypedDict(
-    "AudioOnlyHlsSettingsOutputTypeDef",
+AudioOnlyHlsSettingsTypeDef = TypedDict(
+    "AudioOnlyHlsSettingsTypeDef",
     {
         "AudioGroupId": str,
-        "AudioOnlyImage": InputLocationOutputTypeDef,
+        "AudioOnlyImage": InputLocationTypeDef,
         "AudioTrackType": AudioOnlyHlsTrackTypeType,
         "SegmentType": AudioOnlyHlsSegmentTypeType,
     },
     total=False,
 )
 
-AvailBlankingOutputTypeDef = TypedDict(
-    "AvailBlankingOutputTypeDef",
-    {
-        "AvailBlankingImage": InputLocationOutputTypeDef,
-        "State": AvailBlankingStateType,
-    },
-    total=False,
-)
-
-BlackoutSlateOutputTypeDef = TypedDict(
-    "BlackoutSlateOutputTypeDef",
-    {
-        "BlackoutSlateImage": InputLocationOutputTypeDef,
-        "NetworkEndBlackout": BlackoutSlateNetworkEndBlackoutType,
-        "NetworkEndBlackoutImage": InputLocationOutputTypeDef,
-        "NetworkId": str,
-        "State": BlackoutSlateStateType,
-    },
-    total=False,
-)
-
-BurnInDestinationSettingsOutputTypeDef = TypedDict(
-    "BurnInDestinationSettingsOutputTypeDef",
-    {
-        "Alignment": BurnInAlignmentType,
-        "BackgroundColor": BurnInBackgroundColorType,
-        "BackgroundOpacity": int,
-        "Font": InputLocationOutputTypeDef,
-        "FontColor": BurnInFontColorType,
-        "FontOpacity": int,
-        "FontResolution": int,
-        "FontSize": str,
-        "OutlineColor": BurnInOutlineColorType,
-        "OutlineSize": int,
-        "ShadowColor": BurnInShadowColorType,
-        "ShadowOpacity": int,
-        "ShadowXOffset": int,
-        "ShadowYOffset": int,
-        "TeletextGridControl": BurnInTeletextGridControlType,
-        "XPosition": int,
-        "YPosition": int,
-    },
-    total=False,
-)
-
-DvbSubDestinationSettingsOutputTypeDef = TypedDict(
-    "DvbSubDestinationSettingsOutputTypeDef",
-    {
-        "Alignment": DvbSubDestinationAlignmentType,
-        "BackgroundColor": DvbSubDestinationBackgroundColorType,
-        "BackgroundOpacity": int,
-        "Font": InputLocationOutputTypeDef,
-        "FontColor": DvbSubDestinationFontColorType,
-        "FontOpacity": int,
-        "FontResolution": int,
-        "FontSize": str,
-        "OutlineColor": DvbSubDestinationOutlineColorType,
-        "OutlineSize": int,
-        "ShadowColor": DvbSubDestinationShadowColorType,
-        "ShadowOpacity": int,
-        "ShadowXOffset": int,
-        "ShadowYOffset": int,
-        "TeletextGridControl": DvbSubDestinationTeletextGridControlType,
-        "XPosition": int,
-        "YPosition": int,
-    },
-    total=False,
-)
-
-InputLossBehaviorOutputTypeDef = TypedDict(
-    "InputLossBehaviorOutputTypeDef",
-    {
-        "BlackFrameMsec": int,
-        "InputLossImageColor": str,
-        "InputLossImageSlate": InputLocationOutputTypeDef,
-        "InputLossImageType": InputLossImageTypeType,
-        "RepeatFrameMsec": int,
-    },
-    total=False,
-)
-
-_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef",
-    {
-        "Image": InputLocationOutputTypeDef,
-    },
-)
-_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef",
-    {
-        "Duration": int,
-        "FadeIn": int,
-        "FadeOut": int,
-        "Height": int,
-        "ImageX": int,
-        "ImageY": int,
-        "Layer": int,
-        "Opacity": int,
-        "Width": int,
-    },
-    total=False,
-)
-
-
-class StaticImageActivateScheduleActionSettingsOutputTypeDef(
-    _RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef,
-    _OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
-
-_RequiredStaticKeySettingsOutputTypeDef = TypedDict(
-    "_RequiredStaticKeySettingsOutputTypeDef",
-    {
-        "StaticKeyValue": str,
-    },
-)
-_OptionalStaticKeySettingsOutputTypeDef = TypedDict(
-    "_OptionalStaticKeySettingsOutputTypeDef",
-    {
-        "KeyProviderServer": InputLocationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class StaticKeySettingsOutputTypeDef(
-    _RequiredStaticKeySettingsOutputTypeDef, _OptionalStaticKeySettingsOutputTypeDef
-):
-    pass
-
-
-_RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
-    "_RequiredAudioTrackSelectionOutputTypeDef",
-    {
-        "Tracks": List[AudioTrackOutputTypeDef],
-    },
-)
-_OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
-    "_OptionalAudioTrackSelectionOutputTypeDef",
-    {
-        "DolbyEDecode": AudioDolbyEDecodeOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AudioTrackSelectionOutputTypeDef(
-    _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
-):
-    pass
-
-
-_RequiredAudioTrackSelectionTypeDef = TypedDict(
-    "_RequiredAudioTrackSelectionTypeDef",
-    {
-        "Tracks": Sequence[AudioTrackTypeDef],
-    },
-)
-_OptionalAudioTrackSelectionTypeDef = TypedDict(
-    "_OptionalAudioTrackSelectionTypeDef",
-    {
-        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
-    },
-    total=False,
-)
-
-
-class AudioTrackSelectionTypeDef(
-    _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
-):
-    pass
-
-
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": InputLocationTypeDef,
         "State": AvailBlankingStateType,
     },
     total=False,
@@ -4136,53 +2728,77 @@
         "Layer": int,
         "Opacity": int,
         "Width": int,
     },
     total=False,
 )
 
-
 class StaticImageActivateScheduleActionSettingsTypeDef(
     _RequiredStaticImageActivateScheduleActionSettingsTypeDef,
     _OptionalStaticImageActivateScheduleActionSettingsTypeDef,
 ):
     pass
 
-
 _RequiredStaticKeySettingsTypeDef = TypedDict(
     "_RequiredStaticKeySettingsTypeDef",
     {
         "StaticKeyValue": str,
     },
 )
 _OptionalStaticKeySettingsTypeDef = TypedDict(
     "_OptionalStaticKeySettingsTypeDef",
     {
         "KeyProviderServer": InputLocationTypeDef,
     },
     total=False,
 )
 
-
 class StaticKeySettingsTypeDef(
     _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
 ):
     pass
 
+_RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
+    "_RequiredAudioTrackSelectionOutputTypeDef",
+    {
+        "Tracks": List[AudioTrackTypeDef],
+    },
+)
+_OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
+    "_OptionalAudioTrackSelectionOutputTypeDef",
+    {
+        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
+    },
+    total=False,
+)
+
+class AudioTrackSelectionOutputTypeDef(
+    _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
+):
+    pass
 
-AvailSettingsOutputTypeDef = TypedDict(
-    "AvailSettingsOutputTypeDef",
+_RequiredAudioTrackSelectionTypeDef = TypedDict(
+    "_RequiredAudioTrackSelectionTypeDef",
+    {
+        "Tracks": Sequence[AudioTrackTypeDef],
+    },
+)
+_OptionalAudioTrackSelectionTypeDef = TypedDict(
+    "_OptionalAudioTrackSelectionTypeDef",
     {
-        "Esam": EsamOutputTypeDef,
-        "Scte35SpliceInsert": Scte35SpliceInsertOutputTypeDef,
-        "Scte35TimeSignalApos": Scte35TimeSignalAposOutputTypeDef,
+        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
     },
     total=False,
 )
 
+class AudioTrackSelectionTypeDef(
+    _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
+):
+    pass
+
 AvailSettingsTypeDef = TypedDict(
     "AvailSettingsTypeDef",
     {
         "Esam": EsamTypeDef,
         "Scte35SpliceInsert": Scte35SpliceInsertTypeDef,
         "Scte35TimeSignalApos": Scte35TimeSignalAposTypeDef,
     },
@@ -4190,43 +2806,77 @@
 )
 
 BatchDeleteResponseTypeDef = TypedDict(
     "BatchDeleteResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartResponseTypeDef = TypedDict(
     "BatchStartResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStopResponseTypeDef = TypedDict(
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TeletextSourceSettingsOutputTypeDef = TypedDict(
-    "TeletextSourceSettingsOutputTypeDef",
+DescribeAccountConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccountConfigurationResponseTypeDef",
     {
-        "OutputRectangle": CaptionRectangleOutputTypeDef,
-        "PageNumber": str,
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ContentType": Literal["image/jpeg"],
+        "ContentLength": int,
+        "ETag": str,
+        "LastModified": datetime,
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
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
         "PageNumber": str,
@@ -4272,22 +2922,20 @@
     {
         "Tags": Mapping[str, str],
         "WhitelistRules": Sequence[InputWhitelistRuleCidrTypeDef],
     },
     total=False,
 )
 
-
 class UpdateInputSecurityGroupRequestRequestTypeDef(
     _RequiredUpdateInputSecurityGroupRequestRequestTypeDef,
     _OptionalUpdateInputSecurityGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMultiplexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultiplexRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "RequestId": str,
@@ -4297,21 +2945,19 @@
     "_OptionalCreateMultiplexRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateMultiplexRequestRequestTypeDef(
     _RequiredCreateMultiplexRequestRequestTypeDef, _OptionalCreateMultiplexRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateMultiplexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalUpdateMultiplexRequestRequestTypeDef = TypedDict(
@@ -4319,20 +2965,62 @@
     {
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateMultiplexRequestRequestTypeDef(
     _RequiredUpdateMultiplexRequestRequestTypeDef, _OptionalUpdateMultiplexRequestRequestTypeDef
 ):
     pass
 
+_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_RequiredPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Count": int,
+        "OfferingId": str,
+    },
+)
+_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_OptionalPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+        "RequestId": str,
+        "Start": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PurchaseOfferingRequestRequestTypeDef(
+    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReservationRequestRequestTypeDef",
+    {
+        "ReservationId": str,
+    },
+)
+_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReservationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+    },
+    total=False,
+)
+
+class UpdateReservationRequestRequestTypeDef(
+    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
+):
+    pass
 
 DeleteReservationResponseTypeDef = TypedDict(
     "DeleteReservationResponseTypeDef",
     {
         "Arn": str,
         "Count": int,
         "CurrencyCode": str,
@@ -4341,22 +3029,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsOutputTypeDef,
+        "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Arn": str,
@@ -4366,15 +3054,15 @@
         "FixedPrice": float,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "UsagePrice": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Arn": str,
@@ -4385,22 +3073,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsOutputTypeDef,
+        "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "Arn": str,
@@ -4429,15 +3117,15 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsOutputTypeDef,
+        "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
     },
@@ -4454,242 +3142,220 @@
     "_OptionalDescribeChannelRequestChannelCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeChannelRequestChannelCreatedWaitTypeDef(
     _RequiredDescribeChannelRequestChannelCreatedWaitTypeDef,
     _OptionalDescribeChannelRequestChannelCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeChannelRequestChannelDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeChannelRequestChannelDeletedWaitTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeChannelRequestChannelDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeChannelRequestChannelDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeChannelRequestChannelDeletedWaitTypeDef(
     _RequiredDescribeChannelRequestChannelDeletedWaitTypeDef,
     _OptionalDescribeChannelRequestChannelDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeChannelRequestChannelRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeChannelRequestChannelRunningWaitTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeChannelRequestChannelRunningWaitTypeDef = TypedDict(
     "_OptionalDescribeChannelRequestChannelRunningWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeChannelRequestChannelRunningWaitTypeDef(
     _RequiredDescribeChannelRequestChannelRunningWaitTypeDef,
     _OptionalDescribeChannelRequestChannelRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeChannelRequestChannelStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeChannelRequestChannelStoppedWaitTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeChannelRequestChannelStoppedWaitTypeDef = TypedDict(
     "_OptionalDescribeChannelRequestChannelStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeChannelRequestChannelStoppedWaitTypeDef(
     _RequiredDescribeChannelRequestChannelStoppedWaitTypeDef,
     _OptionalDescribeChannelRequestChannelStoppedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInputRequestInputAttachedWaitTypeDef = TypedDict(
     "_RequiredDescribeInputRequestInputAttachedWaitTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalDescribeInputRequestInputAttachedWaitTypeDef = TypedDict(
     "_OptionalDescribeInputRequestInputAttachedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInputRequestInputAttachedWaitTypeDef(
     _RequiredDescribeInputRequestInputAttachedWaitTypeDef,
     _OptionalDescribeInputRequestInputAttachedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInputRequestInputDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeInputRequestInputDeletedWaitTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalDescribeInputRequestInputDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeInputRequestInputDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInputRequestInputDeletedWaitTypeDef(
     _RequiredDescribeInputRequestInputDeletedWaitTypeDef,
     _OptionalDescribeInputRequestInputDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInputRequestInputDetachedWaitTypeDef = TypedDict(
     "_RequiredDescribeInputRequestInputDetachedWaitTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalDescribeInputRequestInputDetachedWaitTypeDef = TypedDict(
     "_OptionalDescribeInputRequestInputDetachedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInputRequestInputDetachedWaitTypeDef(
     _RequiredDescribeInputRequestInputDetachedWaitTypeDef,
     _OptionalDescribeInputRequestInputDetachedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMultiplexRequestMultiplexCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexCreatedWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexCreatedWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMultiplexRequestMultiplexCreatedWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexCreatedWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMultiplexRequestMultiplexDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexDeletedWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMultiplexRequestMultiplexDeletedWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexDeletedWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMultiplexRequestMultiplexRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexRunningWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMultiplexRequestMultiplexRunningWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMultiplexRequestMultiplexStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexStoppedWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMultiplexRequestMultiplexStoppedWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
 ):
     pass
 
-
 DescribeInputDeviceResponseTypeDef = TypedDict(
     "DescribeInputDeviceResponseTypeDef",
     {
         "Arn": str,
         "ConnectionState": InputDeviceConnectionStateType,
         "DeviceSettingsSyncState": DeviceSettingsSyncStateType,
         "DeviceUpdateStatus": DeviceUpdateStatusType,
@@ -4698,15 +3364,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
         "Arn": str,
@@ -4738,28 +3404,28 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputSecurityGroupTypeDef = TypedDict(
     "InputSecurityGroupTypeDef",
     {
         "Arn": str,
@@ -4768,32 +3434,166 @@
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
     },
     total=False,
 )
 
-M2tsSettingsOutputTypeDef = TypedDict(
-    "M2tsSettingsOutputTypeDef",
+_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "ChannelId": str,
+    },
+)
+_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
+    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+):
+    pass
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "TransferType": str,
+    },
+)
+_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
+    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+):
+    pass
+
+ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInputsRequestListInputsPaginateTypeDef = TypedDict(
+    "ListInputsRequestListInputsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "MultiplexId": str,
+    },
+)
+_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
+    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+):
+    pass
+
+ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "ChannelConfiguration": str,
+        "Codec": str,
+        "Duration": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "Codec": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+M2tsSettingsTypeDef = TypedDict(
+    "M2tsSettingsTypeDef",
     {
         "AbsentInputAudioBehavior": M2tsAbsentInputAudioBehaviorType,
         "Arib": M2tsAribType,
         "AribCaptionsPid": str,
         "AribCaptionsPidControl": M2tsAribCaptionsPidControlType,
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "AudioStreamType": M2tsAudioStreamTypeType,
         "Bitrate": int,
         "BufferModel": M2tsBufferModelType,
         "CcDescriptor": M2tsCcDescriptorType,
-        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
+        "DvbNitSettings": DvbNitSettingsTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsTypeDef,
         "DvbSubPids": str,
-        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
+        "DvbTdtSettings": DvbTdtSettingsTypeDef,
         "DvbTeletextPid": str,
         "Ebif": M2tsEbifControlType,
         "EbpAudioInterval": M2tsAudioIntervalType,
         "EbpLookaheadMs": int,
         "EbpPlacement": M2tsEbpPlacementType,
         "EcmPid": str,
         "EsRateInPes": M2tsEsRateInPesType,
@@ -4823,39 +3623,29 @@
         "TransportStreamId": int,
         "VideoPid": str,
         "Scte35PrerollPullupMilliseconds": float,
     },
     total=False,
 )
 
-FailoverConditionSettingsOutputTypeDef = TypedDict(
-    "FailoverConditionSettingsOutputTypeDef",
-    {
-        "AudioSilenceSettings": AudioSilenceFailoverSettingsOutputTypeDef,
-        "InputLossSettings": InputLossFailoverSettingsOutputTypeDef,
-        "VideoBlackSettings": VideoBlackFailoverSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": AudioSilenceFailoverSettingsTypeDef,
         "InputLossSettings": InputLossFailoverSettingsTypeDef,
         "VideoBlackSettings": VideoBlackFailoverSettingsTypeDef,
     },
     total=False,
 )
 
 ScheduleActionStartSettingsOutputTypeDef = TypedDict(
     "ScheduleActionStartSettingsOutputTypeDef",
     {
-        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsOutputTypeDef,
-        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsOutputTypeDef,
+        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
+        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Dict[str, Any],
     },
     total=False,
 )
 
 ScheduleActionStartSettingsTypeDef = TypedDict(
     "ScheduleActionStartSettingsTypeDef",
@@ -4863,74 +3653,32 @@
         "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
         "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-FrameCaptureCdnSettingsOutputTypeDef = TypedDict(
-    "FrameCaptureCdnSettingsOutputTypeDef",
-    {
-        "FrameCaptureS3Settings": FrameCaptureS3SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 FrameCaptureCdnSettingsTypeDef = TypedDict(
     "FrameCaptureCdnSettingsTypeDef",
     {
         "FrameCaptureS3Settings": FrameCaptureS3SettingsTypeDef,
     },
     total=False,
 )
 
-FrameCaptureSettingsOutputTypeDef = TypedDict(
-    "FrameCaptureSettingsOutputTypeDef",
-    {
-        "CaptureInterval": int,
-        "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "CaptureInterval": int,
         "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-H264FilterSettingsOutputTypeDef = TypedDict(
-    "H264FilterSettingsOutputTypeDef",
-    {
-        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-H265FilterSettingsOutputTypeDef = TypedDict(
-    "H265FilterSettingsOutputTypeDef",
-    {
-        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-Mpeg2FilterSettingsOutputTypeDef = TypedDict(
-    "Mpeg2FilterSettingsOutputTypeDef",
-    {
-        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 H264FilterSettingsTypeDef = TypedDict(
     "H264FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
@@ -4952,29 +3700,21 @@
 )
 
 H265ColorSpaceSettingsOutputTypeDef = TypedDict(
     "H265ColorSpaceSettingsOutputTypeDef",
     {
         "ColorSpacePassthroughSettings": Dict[str, Any],
         "DolbyVision81Settings": Dict[str, Any],
-        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
+        "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Dict[str, Any],
         "Rec709Settings": Dict[str, Any],
     },
     total=False,
 )
 
-VideoSelectorColorSpaceSettingsOutputTypeDef = TypedDict(
-    "VideoSelectorColorSpaceSettingsOutputTypeDef",
-    {
-        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "DolbyVision81Settings": Mapping[str, Any],
         "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Mapping[str, Any],
@@ -4987,78 +3727,35 @@
     "VideoSelectorColorSpaceSettingsTypeDef",
     {
         "Hdr10Settings": Hdr10SettingsTypeDef,
     },
     total=False,
 )
 
-HlsCdnSettingsOutputTypeDef = TypedDict(
-    "HlsCdnSettingsOutputTypeDef",
-    {
-        "HlsAkamaiSettings": HlsAkamaiSettingsOutputTypeDef,
-        "HlsBasicPutSettings": HlsBasicPutSettingsOutputTypeDef,
-        "HlsMediaStoreSettings": HlsMediaStoreSettingsOutputTypeDef,
-        "HlsS3Settings": HlsS3SettingsOutputTypeDef,
-        "HlsWebdavSettings": HlsWebdavSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 HlsCdnSettingsTypeDef = TypedDict(
     "HlsCdnSettingsTypeDef",
     {
         "HlsAkamaiSettings": HlsAkamaiSettingsTypeDef,
         "HlsBasicPutSettings": HlsBasicPutSettingsTypeDef,
         "HlsMediaStoreSettings": HlsMediaStoreSettingsTypeDef,
         "HlsS3Settings": HlsS3SettingsTypeDef,
         "HlsWebdavSettings": HlsWebdavSettingsTypeDef,
     },
     total=False,
 )
 
-NetworkInputSettingsOutputTypeDef = TypedDict(
-    "NetworkInputSettingsOutputTypeDef",
-    {
-        "HlsInputSettings": HlsInputSettingsOutputTypeDef,
-        "ServerValidation": NetworkInputServerValidationType,
-    },
-    total=False,
-)
-
 NetworkInputSettingsTypeDef = TypedDict(
     "NetworkInputSettingsTypeDef",
     {
         "HlsInputSettings": HlsInputSettingsTypeDef,
         "ServerValidation": NetworkInputServerValidationType,
     },
     total=False,
 )
 
-_RequiredInputClippingSettingsOutputTypeDef = TypedDict(
-    "_RequiredInputClippingSettingsOutputTypeDef",
-    {
-        "InputTimecodeSource": InputTimecodeSourceType,
-    },
-)
-_OptionalInputClippingSettingsOutputTypeDef = TypedDict(
-    "_OptionalInputClippingSettingsOutputTypeDef",
-    {
-        "StartTimecode": StartTimecodeOutputTypeDef,
-        "StopTimecode": StopTimecodeOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class InputClippingSettingsOutputTypeDef(
-    _RequiredInputClippingSettingsOutputTypeDef, _OptionalInputClippingSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredInputClippingSettingsTypeDef = TypedDict(
     "_RequiredInputClippingSettingsTypeDef",
     {
         "InputTimecodeSource": InputTimecodeSourceType,
     },
 )
 _OptionalInputClippingSettingsTypeDef = TypedDict(
@@ -5066,21 +3763,19 @@
     {
         "StartTimecode": StartTimecodeTypeDef,
         "StopTimecode": StopTimecodeTypeDef,
     },
     total=False,
 )
 
-
 class InputClippingSettingsTypeDef(
     _RequiredInputClippingSettingsTypeDef, _OptionalInputClippingSettingsTypeDef
 ):
     pass
 
-
 InputDestinationTypeDef = TypedDict(
     "InputDestinationTypeDef",
     {
         "Ip": str,
         "Port": str,
         "Url": str,
         "Vpc": InputDestinationVpcTypeDef,
@@ -5100,21 +3795,19 @@
         "HdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
         "Name": str,
         "UhdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateInputDeviceRequestRequestTypeDef(
     _RequiredUpdateInputDeviceRequestRequestTypeDef, _OptionalUpdateInputDeviceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalUpdateInputRequestRequestTypeDef = TypedDict(
@@ -5127,103 +3820,95 @@
         "Name": str,
         "RoleArn": str,
         "Sources": Sequence[InputSourceRequestTypeDef],
     },
     total=False,
 )
 
-
 class UpdateInputRequestRequestTypeDef(
     _RequiredUpdateInputRequestRequestTypeDef, _OptionalUpdateInputRequestRequestTypeDef
 ):
     pass
 
-
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStandardHlsSettingsOutputTypeDef = TypedDict(
-    "_RequiredStandardHlsSettingsOutputTypeDef",
+_RequiredStandardHlsSettingsTypeDef = TypedDict(
+    "_RequiredStandardHlsSettingsTypeDef",
     {
-        "M3u8Settings": M3u8SettingsOutputTypeDef,
+        "M3u8Settings": M3u8SettingsTypeDef,
     },
 )
-_OptionalStandardHlsSettingsOutputTypeDef = TypedDict(
-    "_OptionalStandardHlsSettingsOutputTypeDef",
+_OptionalStandardHlsSettingsTypeDef = TypedDict(
+    "_OptionalStandardHlsSettingsTypeDef",
     {
         "AudioRenditionSets": str,
     },
     total=False,
 )
 
-
-class StandardHlsSettingsOutputTypeDef(
-    _RequiredStandardHlsSettingsOutputTypeDef, _OptionalStandardHlsSettingsOutputTypeDef
+class StandardHlsSettingsTypeDef(
+    _RequiredStandardHlsSettingsTypeDef, _OptionalStandardHlsSettingsTypeDef
 ):
     pass
 
-
 _RequiredMotionGraphicsConfigurationOutputTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationOutputTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
     },
 )
 _OptionalMotionGraphicsConfigurationOutputTypeDef = TypedDict(
     "_OptionalMotionGraphicsConfigurationOutputTypeDef",
     {
         "MotionGraphicsInsertion": MotionGraphicsInsertionType,
     },
     total=False,
 )
 
-
 class MotionGraphicsConfigurationOutputTypeDef(
     _RequiredMotionGraphicsConfigurationOutputTypeDef,
     _OptionalMotionGraphicsConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredMotionGraphicsConfigurationTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
     },
 )
 _OptionalMotionGraphicsConfigurationTypeDef = TypedDict(
     "_OptionalMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsInsertion": MotionGraphicsInsertionType,
     },
     total=False,
 )
 
-
 class MotionGraphicsConfigurationTypeDef(
     _RequiredMotionGraphicsConfigurationTypeDef, _OptionalMotionGraphicsConfigurationTypeDef
 ):
     pass
 
-
 MultiplexOutputDestinationTypeDef = TypedDict(
     "MultiplexOutputDestinationTypeDef",
     {
         "MediaConnectSettings": MultiplexMediaConnectOutputDestinationSettingsTypeDef,
     },
     total=False,
 )
@@ -5240,59 +3925,40 @@
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-MultiplexVideoSettingsOutputTypeDef = TypedDict(
-    "MultiplexVideoSettingsOutputTypeDef",
-    {
-        "ConstantBitrate": int,
-        "StatmuxSettings": MultiplexStatmuxVideoSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 MultiplexVideoSettingsTypeDef = TypedDict(
     "MultiplexVideoSettingsTypeDef",
     {
         "ConstantBitrate": int,
         "StatmuxSettings": MultiplexStatmuxVideoSettingsTypeDef,
     },
     total=False,
 )
 
-NielsenWatermarksSettingsOutputTypeDef = TypedDict(
-    "NielsenWatermarksSettingsOutputTypeDef",
-    {
-        "NielsenCbetSettings": NielsenCBETOutputTypeDef,
-        "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
-        "NielsenNaesIiNwSettings": NielsenNaesIiNwOutputTypeDef,
-    },
-    total=False,
-)
-
 NielsenWatermarksSettingsTypeDef = TypedDict(
     "NielsenWatermarksSettingsTypeDef",
     {
         "NielsenCbetSettings": NielsenCBETTypeDef,
         "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
         "NielsenNaesIiNwSettings": NielsenNaesIiNwTypeDef,
     },
     total=False,
 )
 
 OutputDestinationOutputTypeDef = TypedDict(
     "OutputDestinationOutputTypeDef",
     {
         "Id": str,
-        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsOutputTypeDef],
-        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsOutputTypeDef,
-        "Settings": List[OutputDestinationSettingsOutputTypeDef],
+        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsTypeDef],
+        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
+        "Settings": List[OutputDestinationSettingsTypeDef],
     },
     total=False,
 )
 
 OutputDestinationTypeDef = TypedDict(
     "OutputDestinationTypeDef",
     {
@@ -5303,106 +3969,27 @@
     },
     total=False,
 )
 
 PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsOutputTypeDef",
     {
-        "Pipelines": List[PipelinePauseStateSettingsOutputTypeDef],
+        "Pipelines": List[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
 
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
         "Pipelines": Sequence[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
 
-_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_RequiredPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Count": int,
-        "OfferingId": str,
-    },
-)
-_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_OptionalPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-        "RequestId": str,
-        "Start": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PurchaseOfferingRequestRequestTypeDef(
-    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReservationRequestRequestTypeDef",
-    {
-        "ReservationId": str,
-    },
-)
-_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReservationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateReservationRequestRequestTypeDef(
-    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredScte35SegmentationDescriptorOutputTypeDef = TypedDict(
-    "_RequiredScte35SegmentationDescriptorOutputTypeDef",
-    {
-        "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
-        "SegmentationEventId": int,
-    },
-)
-_OptionalScte35SegmentationDescriptorOutputTypeDef = TypedDict(
-    "_OptionalScte35SegmentationDescriptorOutputTypeDef",
-    {
-        "DeliveryRestrictions": Scte35DeliveryRestrictionsOutputTypeDef,
-        "SegmentNum": int,
-        "SegmentationDuration": int,
-        "SegmentationTypeId": int,
-        "SegmentationUpid": str,
-        "SegmentationUpidType": int,
-        "SegmentsExpected": int,
-        "SubSegmentNum": int,
-        "SubSegmentsExpected": int,
-    },
-    total=False,
-)
-
-
-class Scte35SegmentationDescriptorOutputTypeDef(
-    _RequiredScte35SegmentationDescriptorOutputTypeDef,
-    _OptionalScte35SegmentationDescriptorOutputTypeDef,
-):
-    pass
-
-
 _RequiredScte35SegmentationDescriptorTypeDef = TypedDict(
     "_RequiredScte35SegmentationDescriptorTypeDef",
     {
         "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
         "SegmentationEventId": int,
     },
 )
@@ -5418,70 +4005,37 @@
         "SegmentsExpected": int,
         "SubSegmentNum": int,
         "SubSegmentsExpected": int,
     },
     total=False,
 )
 
-
 class Scte35SegmentationDescriptorTypeDef(
     _RequiredScte35SegmentationDescriptorTypeDef, _OptionalScte35SegmentationDescriptorTypeDef
 ):
     pass
 
-
 ThumbnailDetailTypeDef = TypedDict(
     "ThumbnailDetailTypeDef",
     {
         "PipelineId": str,
         "Thumbnails": List[ThumbnailTypeDef],
     },
     total=False,
 )
 
-VideoSelectorSettingsOutputTypeDef = TypedDict(
-    "VideoSelectorSettingsOutputTypeDef",
-    {
-        "VideoSelectorPid": VideoSelectorPidOutputTypeDef,
-        "VideoSelectorProgramId": VideoSelectorProgramIdOutputTypeDef,
-    },
-    total=False,
-)
-
 VideoSelectorSettingsTypeDef = TypedDict(
     "VideoSelectorSettingsTypeDef",
     {
         "VideoSelectorPid": VideoSelectorPidTypeDef,
         "VideoSelectorProgramId": VideoSelectorProgramIdTypeDef,
     },
     total=False,
 )
 
-_RequiredArchiveGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredArchiveGroupSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-_OptionalArchiveGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalArchiveGroupSettingsOutputTypeDef",
-    {
-        "ArchiveCdnSettings": ArchiveCdnSettingsOutputTypeDef,
-        "RolloverInterval": int,
-    },
-    total=False,
-)
-
-
-class ArchiveGroupSettingsOutputTypeDef(
-    _RequiredArchiveGroupSettingsOutputTypeDef, _OptionalArchiveGroupSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredArchiveGroupSettingsTypeDef = TypedDict(
     "_RequiredArchiveGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalArchiveGroupSettingsTypeDef = TypedDict(
@@ -5489,21 +4043,19 @@
     {
         "ArchiveCdnSettings": ArchiveCdnSettingsTypeDef,
         "RolloverInterval": int,
     },
     total=False,
 )
 
-
 class ArchiveGroupSettingsTypeDef(
     _RequiredArchiveGroupSettingsTypeDef, _OptionalArchiveGroupSettingsTypeDef
 ):
     pass
 
-
 _RequiredRemixSettingsOutputTypeDef = TypedDict(
     "_RequiredRemixSettingsOutputTypeDef",
     {
         "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
     },
 )
 _OptionalRemixSettingsOutputTypeDef = TypedDict(
@@ -5511,21 +4063,19 @@
     {
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
-
 class RemixSettingsOutputTypeDef(
     _RequiredRemixSettingsOutputTypeDef, _OptionalRemixSettingsOutputTypeDef
 ):
     pass
 
-
 _RequiredRemixSettingsTypeDef = TypedDict(
     "_RequiredRemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
     },
 )
 _OptionalRemixSettingsTypeDef = TypedDict(
@@ -5533,78 +4083,33 @@
     {
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
-
 class RemixSettingsTypeDef(_RequiredRemixSettingsTypeDef, _OptionalRemixSettingsTypeDef):
     pass
 
-
 CaptionDestinationSettingsOutputTypeDef = TypedDict(
     "CaptionDestinationSettingsOutputTypeDef",
     {
         "AribDestinationSettings": Dict[str, Any],
-        "BurnInDestinationSettings": BurnInDestinationSettingsOutputTypeDef,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
-        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsOutputTypeDef,
+        "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
+        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": Dict[str, Any],
         "EmbeddedPlusScte20DestinationSettings": Dict[str, Any],
         "RtmpCaptionInfoDestinationSettings": Dict[str, Any],
         "Scte20PlusEmbeddedDestinationSettings": Dict[str, Any],
         "Scte27DestinationSettings": Dict[str, Any],
         "SmpteTtDestinationSettings": Dict[str, Any],
         "TeletextDestinationSettings": Dict[str, Any],
-        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-GlobalConfigurationOutputTypeDef = TypedDict(
-    "GlobalConfigurationOutputTypeDef",
-    {
-        "InitialAudioGain": int,
-        "InputEndAction": GlobalConfigurationInputEndActionType,
-        "InputLossBehavior": InputLossBehaviorOutputTypeDef,
-        "OutputLockingMode": GlobalConfigurationOutputLockingModeType,
-        "OutputTimingSource": GlobalConfigurationOutputTimingSourceType,
-        "SupportLowFramerateInputs": GlobalConfigurationLowFramerateInputsType,
-    },
-    total=False,
-)
-
-KeyProviderSettingsOutputTypeDef = TypedDict(
-    "KeyProviderSettingsOutputTypeDef",
-    {
-        "StaticKeySettings": StaticKeySettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-AudioSelectorSettingsOutputTypeDef = TypedDict(
-    "AudioSelectorSettingsOutputTypeDef",
-    {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionOutputTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionOutputTypeDef,
-        "AudioPidSelection": AudioPidSelectionOutputTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
-AudioSelectorSettingsTypeDef = TypedDict(
-    "AudioSelectorSettingsTypeDef",
-    {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
-        "AudioPidSelection": AudioPidSelectionTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
     },
     total=False,
 )
 
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
@@ -5642,18 +4147,32 @@
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": StaticKeySettingsTypeDef,
     },
     total=False,
 )
 
-AvailConfigurationOutputTypeDef = TypedDict(
-    "AvailConfigurationOutputTypeDef",
+AudioSelectorSettingsOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsOutputTypeDef",
+    {
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
+        "AudioPidSelection": AudioPidSelectionTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+AudioSelectorSettingsTypeDef = TypedDict(
+    "AudioSelectorSettingsTypeDef",
     {
-        "AvailSettings": AvailSettingsOutputTypeDef,
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
+        "AudioPidSelection": AudioPidSelectionTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionTypeDef,
     },
     total=False,
 )
 
 AvailConfigurationTypeDef = TypedDict(
     "AvailConfigurationTypeDef",
     {
@@ -5661,21 +4180,21 @@
     },
     total=False,
 )
 
 CaptionSelectorSettingsOutputTypeDef = TypedDict(
     "CaptionSelectorSettingsOutputTypeDef",
     {
-        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "AribSourceSettings": Dict[str, Any],
-        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
-        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
-        "Scte20SourceSettings": Scte20SourceSettingsOutputTypeDef,
-        "Scte27SourceSettings": Scte27SourceSettingsOutputTypeDef,
-        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+        "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
+        "Scte20SourceSettings": Scte20SourceSettingsTypeDef,
+        "Scte27SourceSettings": Scte27SourceSettingsTypeDef,
+        "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
     },
     total=False,
 )
 
 CaptionSelectorSettingsTypeDef = TypedDict(
     "CaptionSelectorSettingsTypeDef",
     {
@@ -5691,164 +4210,133 @@
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReservationResponseTypeDef = TypedDict(
     "UpdateReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInputSecurityGroupResponseTypeDef = TypedDict(
     "CreateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ArchiveContainerSettingsOutputTypeDef = TypedDict(
-    "ArchiveContainerSettingsOutputTypeDef",
-    {
-        "M2tsSettings": M2tsSettingsOutputTypeDef,
-        "RawSettings": Dict[str, Any],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UdpContainerSettingsOutputTypeDef = TypedDict(
-    "UdpContainerSettingsOutputTypeDef",
+ArchiveContainerSettingsTypeDef = TypedDict(
+    "ArchiveContainerSettingsTypeDef",
     {
-        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "M2tsSettings": M2tsSettingsTypeDef,
+        "RawSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-FailoverConditionOutputTypeDef = TypedDict(
-    "FailoverConditionOutputTypeDef",
+UdpContainerSettingsTypeDef = TypedDict(
+    "UdpContainerSettingsTypeDef",
     {
-        "FailoverConditionSettings": FailoverConditionSettingsOutputTypeDef,
+        "M2tsSettings": M2tsSettingsTypeDef,
     },
     total=False,
 )
 
 FailoverConditionTypeDef = TypedDict(
     "FailoverConditionTypeDef",
     {
         "FailoverConditionSettings": FailoverConditionSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredFrameCaptureGroupSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-_OptionalFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalFrameCaptureGroupSettingsOutputTypeDef",
-    {
-        "FrameCaptureCdnSettings": FrameCaptureCdnSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FrameCaptureGroupSettingsOutputTypeDef(
-    _RequiredFrameCaptureGroupSettingsOutputTypeDef, _OptionalFrameCaptureGroupSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredFrameCaptureGroupSettingsTypeDef = TypedDict(
     "_RequiredFrameCaptureGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalFrameCaptureGroupSettingsTypeDef = TypedDict(
     "_OptionalFrameCaptureGroupSettingsTypeDef",
     {
         "FrameCaptureCdnSettings": FrameCaptureCdnSettingsTypeDef,
     },
     total=False,
 )
 
-
 class FrameCaptureGroupSettingsTypeDef(
     _RequiredFrameCaptureGroupSettingsTypeDef, _OptionalFrameCaptureGroupSettingsTypeDef
 ):
     pass
 
-
 H264SettingsOutputTypeDef = TypedDict(
     "H264SettingsOutputTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
         "BufSize": int,
         "ColorMetadata": H264ColorMetadataType,
         "ColorSpaceSettings": H264ColorSpaceSettingsOutputTypeDef,
         "EntropyEncoding": H264EntropyEncodingType,
-        "FilterSettings": H264FilterSettingsOutputTypeDef,
+        "FilterSettings": H264FilterSettingsTypeDef,
         "FixedAfd": FixedAfdType,
         "FlickerAq": H264FlickerAqType,
         "ForceFieldPictures": H264ForceFieldPicturesType,
         "FramerateControl": H264FramerateControlType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "GopBReference": H264GopBReferenceType,
@@ -5873,55 +4361,19 @@
         "Slices": int,
         "Softness": int,
         "SpatialAq": H264SpatialAqType,
         "SubgopLength": H264SubGopLengthType,
         "Syntax": H264SyntaxType,
         "TemporalAq": H264TemporalAqType,
         "TimecodeInsertion": H264TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredMpeg2SettingsOutputTypeDef = TypedDict(
-    "_RequiredMpeg2SettingsOutputTypeDef",
-    {
-        "FramerateDenominator": int,
-        "FramerateNumerator": int,
-    },
-)
-_OptionalMpeg2SettingsOutputTypeDef = TypedDict(
-    "_OptionalMpeg2SettingsOutputTypeDef",
-    {
-        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
-        "AfdSignaling": AfdSignalingType,
-        "ColorMetadata": Mpeg2ColorMetadataType,
-        "ColorSpace": Mpeg2ColorSpaceType,
-        "DisplayAspectRatio": Mpeg2DisplayRatioType,
-        "FilterSettings": Mpeg2FilterSettingsOutputTypeDef,
-        "FixedAfd": FixedAfdType,
-        "GopClosedCadence": int,
-        "GopNumBFrames": int,
-        "GopSize": float,
-        "GopSizeUnits": Mpeg2GopSizeUnitsType,
-        "ScanType": Mpeg2ScanTypeType,
-        "SubgopLength": Mpeg2SubGopLengthType,
-        "TimecodeInsertion": Mpeg2TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-
-class Mpeg2SettingsOutputTypeDef(
-    _RequiredMpeg2SettingsOutputTypeDef, _OptionalMpeg2SettingsOutputTypeDef
-):
-    pass
-
-
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
@@ -5992,19 +4444,17 @@
         "SubgopLength": Mpeg2SubGopLengthType,
         "TimecodeInsertion": Mpeg2TimecodeInsertionBehaviorType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-
 class Mpeg2SettingsTypeDef(_RequiredMpeg2SettingsTypeDef, _OptionalMpeg2SettingsTypeDef):
     pass
 
-
 _RequiredH265SettingsOutputTypeDef = TypedDict(
     "_RequiredH265SettingsOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -6014,15 +4464,15 @@
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "AlternativeTransferFunction": H265AlternativeTransferFunctionType,
         "Bitrate": int,
         "BufSize": int,
         "ColorMetadata": H265ColorMetadataType,
         "ColorSpaceSettings": H265ColorSpaceSettingsOutputTypeDef,
-        "FilterSettings": H265FilterSettingsOutputTypeDef,
+        "FilterSettings": H265FilterSettingsTypeDef,
         "FixedAfd": FixedAfdType,
         "FlickerAq": H265FlickerAqType,
         "GopClosedCadence": int,
         "GopSize": float,
         "GopSizeUnits": H265GopSizeUnitsType,
         "Level": H265LevelType,
         "LookAheadRateControl": H265LookAheadRateControlType,
@@ -6034,26 +4484,24 @@
         "QvbrQualityLevel": int,
         "RateControlMode": H265RateControlModeType,
         "ScanType": H265ScanTypeType,
         "SceneChangeDetect": H265SceneChangeDetectType,
         "Slices": int,
         "Tier": H265TierType,
         "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-
 class H265SettingsOutputTypeDef(
     _RequiredH265SettingsOutputTypeDef, _OptionalH265SettingsOutputTypeDef
 ):
     pass
 
-
 _RequiredH265SettingsTypeDef = TypedDict(
     "_RequiredH265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -6088,62 +4536,58 @@
         "Tier": H265TierType,
         "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-
 class H265SettingsTypeDef(_RequiredH265SettingsTypeDef, _OptionalH265SettingsTypeDef):
     pass
 
-
 InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": str,
-        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": List[str],
     },
     total=False,
 )
 
+InputPrepareScheduleActionSettingsTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+        "InputClippingSettings": InputClippingSettingsTypeDef,
+        "UrlPath": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
     "_RequiredInputSwitchScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
 )
 _OptionalInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
     "_OptionalInputSwitchScheduleActionSettingsOutputTypeDef",
     {
-        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": List[str],
     },
     total=False,
 )
 
-
 class InputSwitchScheduleActionSettingsOutputTypeDef(
     _RequiredInputSwitchScheduleActionSettingsOutputTypeDef,
     _OptionalInputSwitchScheduleActionSettingsOutputTypeDef,
 ):
     pass
 
-
-InputPrepareScheduleActionSettingsTypeDef = TypedDict(
-    "InputPrepareScheduleActionSettingsTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-        "InputClippingSettings": InputClippingSettingsTypeDef,
-        "UrlPath": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredInputSwitchScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredInputSwitchScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
 )
 _OptionalInputSwitchScheduleActionSettingsTypeDef = TypedDict(
@@ -6151,121 +4595,119 @@
     {
         "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": Sequence[str],
     },
     total=False,
 )
 
-
 class InputSwitchScheduleActionSettingsTypeDef(
     _RequiredInputSwitchScheduleActionSettingsTypeDef,
     _OptionalInputSwitchScheduleActionSettingsTypeDef,
 ):
     pass
 
-
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
+        "InputDevices": List[InputDeviceSettingsTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
+        "InputDevices": List[InputDeviceSettingsTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
     },
     total=False,
 )
 
-HlsSettingsOutputTypeDef = TypedDict(
-    "HlsSettingsOutputTypeDef",
+HlsSettingsTypeDef = TypedDict(
+    "HlsSettingsTypeDef",
     {
-        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsOutputTypeDef,
-        "Fmp4HlsSettings": Fmp4HlsSettingsOutputTypeDef,
-        "FrameCaptureHlsSettings": Dict[str, Any],
-        "StandardHlsSettings": StandardHlsSettingsOutputTypeDef,
+        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsTypeDef,
+        "Fmp4HlsSettings": Fmp4HlsSettingsTypeDef,
+        "FrameCaptureHlsSettings": Mapping[str, Any],
+        "StandardHlsSettings": StandardHlsSettingsTypeDef,
     },
     total=False,
 )
 
 DeleteMultiplexResponseTypeDef = TypedDict(
     "DeleteMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMultiplexResponseTypeDef = TypedDict(
     "DescribeMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MultiplexTypeDef = TypedDict(
     "MultiplexTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
@@ -6274,73 +4716,50 @@
 StartMultiplexResponseTypeDef = TypedDict(
     "StartMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopMultiplexResponseTypeDef = TypedDict(
     "StopMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredMultiplexProgramSettingsOutputTypeDef = TypedDict(
-    "_RequiredMultiplexProgramSettingsOutputTypeDef",
-    {
-        "ProgramNumber": int,
-    },
-)
-_OptionalMultiplexProgramSettingsOutputTypeDef = TypedDict(
-    "_OptionalMultiplexProgramSettingsOutputTypeDef",
-    {
-        "PreferredChannelPipeline": PreferredChannelPipelineType,
-        "ServiceDescriptor": MultiplexProgramServiceDescriptorOutputTypeDef,
-        "VideoSettings": MultiplexVideoSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class MultiplexProgramSettingsOutputTypeDef(
-    _RequiredMultiplexProgramSettingsOutputTypeDef, _OptionalMultiplexProgramSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredMultiplexProgramSettingsTypeDef = TypedDict(
     "_RequiredMultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
     },
 )
 _OptionalMultiplexProgramSettingsTypeDef = TypedDict(
@@ -6349,29 +4768,19 @@
         "PreferredChannelPipeline": PreferredChannelPipelineType,
         "ServiceDescriptor": MultiplexProgramServiceDescriptorTypeDef,
         "VideoSettings": MultiplexVideoSettingsTypeDef,
     },
     total=False,
 )
 
-
 class MultiplexProgramSettingsTypeDef(
     _RequiredMultiplexProgramSettingsTypeDef, _OptionalMultiplexProgramSettingsTypeDef
 ):
     pass
 
-
-AudioWatermarkSettingsOutputTypeDef = TypedDict(
-    "AudioWatermarkSettingsOutputTypeDef",
-    {
-        "NielsenWatermarksSettings": NielsenWatermarksSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 AudioWatermarkSettingsTypeDef = TypedDict(
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
@@ -6387,55 +4796,35 @@
     "_OptionalUpdateChannelClassRequestRequestTypeDef",
     {
         "Destinations": Sequence[OutputDestinationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateChannelClassRequestRequestTypeDef(
     _RequiredUpdateChannelClassRequestRequestTypeDef,
     _OptionalUpdateChannelClassRequestRequestTypeDef,
 ):
     pass
 
-
-Scte35DescriptorSettingsOutputTypeDef = TypedDict(
-    "Scte35DescriptorSettingsOutputTypeDef",
-    {
-        "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorOutputTypeDef,
-    },
-)
-
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
 DescribeThumbnailsResponseTypeDef = TypedDict(
     "DescribeThumbnailsResponseTypeDef",
     {
         "ThumbnailDetails": List[ThumbnailDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VideoSelectorOutputTypeDef = TypedDict(
-    "VideoSelectorOutputTypeDef",
-    {
-        "ColorSpace": VideoSelectorColorSpaceType,
-        "ColorSpaceSettings": VideoSelectorColorSpaceSettingsOutputTypeDef,
-        "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
-        "SelectorSettings": VideoSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 VideoSelectorTypeDef = TypedDict(
     "VideoSelectorTypeDef",
     {
         "ColorSpace": VideoSelectorColorSpaceType,
         "ColorSpaceSettings": VideoSelectorColorSpaceSettingsTypeDef,
         "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
         "SelectorSettings": VideoSelectorSettingsTypeDef,
@@ -6457,55 +4846,76 @@
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": str,
         "LanguageDescription": str,
     },
     total=False,
 )
 
-
 class CaptionDescriptionOutputTypeDef(
     _RequiredCaptionDescriptionOutputTypeDef, _OptionalCaptionDescriptionOutputTypeDef
 ):
     pass
 
+_RequiredCaptionDescriptionTypeDef = TypedDict(
+    "_RequiredCaptionDescriptionTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "Name": str,
+    },
+)
+_OptionalCaptionDescriptionTypeDef = TypedDict(
+    "_OptionalCaptionDescriptionTypeDef",
+    {
+        "Accessibility": AccessibilityTypeType,
+        "DestinationSettings": CaptionDestinationSettingsTypeDef,
+        "LanguageCode": str,
+        "LanguageDescription": str,
+    },
+    total=False,
+)
+
+class CaptionDescriptionTypeDef(
+    _RequiredCaptionDescriptionTypeDef, _OptionalCaptionDescriptionTypeDef
+):
+    pass
 
 _RequiredHlsGroupSettingsOutputTypeDef = TypedDict(
     "_RequiredHlsGroupSettingsOutputTypeDef",
     {
-        "Destination": OutputLocationRefOutputTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalHlsGroupSettingsOutputTypeDef = TypedDict(
     "_OptionalHlsGroupSettingsOutputTypeDef",
     {
         "AdMarkers": List[HlsAdMarkersType],
         "BaseUrlContent": str,
         "BaseUrlContent1": str,
         "BaseUrlManifest": str,
         "BaseUrlManifest1": str,
-        "CaptionLanguageMappings": List[CaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageMappings": List[CaptionLanguageMappingTypeDef],
         "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
         "ClientCache": HlsClientCacheType,
         "CodecSpecification": HlsCodecSpecificationType,
         "ConstantIv": str,
         "DirectoryStructure": HlsDirectoryStructureType,
         "DiscontinuityTags": HlsDiscontinuityTagsType,
         "EncryptionType": HlsEncryptionTypeType,
-        "HlsCdnSettings": HlsCdnSettingsOutputTypeDef,
+        "HlsCdnSettings": HlsCdnSettingsTypeDef,
         "HlsId3SegmentTagging": HlsId3SegmentTaggingStateType,
         "IFrameOnlyPlaylists": IFrameOnlyPlaylistTypeType,
         "IncompleteSegmentBehavior": HlsIncompleteSegmentBehaviorType,
         "IndexNSegments": int,
         "InputLossAction": InputLossActionForHlsOutType,
         "IvInManifest": HlsIvInManifestType,
         "IvSource": HlsIvSourceType,
         "KeepSegments": int,
         "KeyFormat": str,
         "KeyFormatVersions": str,
-        "KeyProviderSettings": KeyProviderSettingsOutputTypeDef,
+        "KeyProviderSettings": KeyProviderSettingsTypeDef,
         "ManifestCompression": HlsManifestCompressionType,
         "ManifestDurationFormat": HlsManifestDurationFormatType,
         "MinSegmentLength": int,
         "Mode": HlsModeType,
         "OutputSelection": HlsOutputSelectionType,
         "ProgramDateTime": HlsProgramDateTimeType,
         "ProgramDateTimeClock": HlsProgramDateTimeClockType,
@@ -6519,86 +4929,19 @@
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
         "TsFileMode": HlsTsFileModeType,
     },
     total=False,
 )
 
-
 class HlsGroupSettingsOutputTypeDef(
     _RequiredHlsGroupSettingsOutputTypeDef, _OptionalHlsGroupSettingsOutputTypeDef
 ):
     pass
 
-
-_RequiredAudioSelectorOutputTypeDef = TypedDict(
-    "_RequiredAudioSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAudioSelectorOutputTypeDef = TypedDict(
-    "_OptionalAudioSelectorOutputTypeDef",
-    {
-        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AudioSelectorOutputTypeDef(
-    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
-):
-    pass
-
-
-_RequiredAudioSelectorTypeDef = TypedDict(
-    "_RequiredAudioSelectorTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAudioSelectorTypeDef = TypedDict(
-    "_OptionalAudioSelectorTypeDef",
-    {
-        "SelectorSettings": AudioSelectorSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
-    pass
-
-
-_RequiredCaptionDescriptionTypeDef = TypedDict(
-    "_RequiredCaptionDescriptionTypeDef",
-    {
-        "CaptionSelectorName": str,
-        "Name": str,
-    },
-)
-_OptionalCaptionDescriptionTypeDef = TypedDict(
-    "_OptionalCaptionDescriptionTypeDef",
-    {
-        "Accessibility": AccessibilityTypeType,
-        "DestinationSettings": CaptionDestinationSettingsTypeDef,
-        "LanguageCode": str,
-        "LanguageDescription": str,
-    },
-    total=False,
-)
-
-
-class CaptionDescriptionTypeDef(
-    _RequiredCaptionDescriptionTypeDef, _OptionalCaptionDescriptionTypeDef
-):
-    pass
-
-
 _RequiredHlsGroupSettingsTypeDef = TypedDict(
     "_RequiredHlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalHlsGroupSettingsTypeDef = TypedDict(
@@ -6646,18 +4989,52 @@
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
         "TsFileMode": HlsTsFileModeType,
     },
     total=False,
 )
 
-
 class HlsGroupSettingsTypeDef(_RequiredHlsGroupSettingsTypeDef, _OptionalHlsGroupSettingsTypeDef):
     pass
 
+_RequiredAudioSelectorOutputTypeDef = TypedDict(
+    "_RequiredAudioSelectorOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorOutputTypeDef = TypedDict(
+    "_OptionalAudioSelectorOutputTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class AudioSelectorOutputTypeDef(
+    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
+):
+    pass
+
+_RequiredAudioSelectorTypeDef = TypedDict(
+    "_RequiredAudioSelectorTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorTypeDef = TypedDict(
+    "_OptionalAudioSelectorTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsTypeDef,
+    },
+    total=False,
+)
+
+class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
+    pass
 
 _RequiredCaptionSelectorOutputTypeDef = TypedDict(
     "_RequiredCaptionSelectorOutputTypeDef",
     {
         "Name": str,
     },
 )
@@ -6666,21 +5043,19 @@
     {
         "LanguageCode": str,
         "SelectorSettings": CaptionSelectorSettingsOutputTypeDef,
     },
     total=False,
 )
 
-
 class CaptionSelectorOutputTypeDef(
     _RequiredCaptionSelectorOutputTypeDef, _OptionalCaptionSelectorOutputTypeDef
 ):
     pass
 
-
 _RequiredCaptionSelectorTypeDef = TypedDict(
     "_RequiredCaptionSelectorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCaptionSelectorTypeDef = TypedDict(
@@ -6688,88 +5063,80 @@
     {
         "LanguageCode": str,
         "SelectorSettings": CaptionSelectorSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CaptionSelectorTypeDef(_RequiredCaptionSelectorTypeDef, _OptionalCaptionSelectorTypeDef):
     pass
 
-
-_RequiredArchiveOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredArchiveOutputSettingsOutputTypeDef",
+_RequiredArchiveOutputSettingsTypeDef = TypedDict(
+    "_RequiredArchiveOutputSettingsTypeDef",
     {
-        "ContainerSettings": ArchiveContainerSettingsOutputTypeDef,
+        "ContainerSettings": ArchiveContainerSettingsTypeDef,
     },
 )
-_OptionalArchiveOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalArchiveOutputSettingsOutputTypeDef",
+_OptionalArchiveOutputSettingsTypeDef = TypedDict(
+    "_OptionalArchiveOutputSettingsTypeDef",
     {
         "Extension": str,
         "NameModifier": str,
     },
     total=False,
 )
 
-
-class ArchiveOutputSettingsOutputTypeDef(
-    _RequiredArchiveOutputSettingsOutputTypeDef, _OptionalArchiveOutputSettingsOutputTypeDef
+class ArchiveOutputSettingsTypeDef(
+    _RequiredArchiveOutputSettingsTypeDef, _OptionalArchiveOutputSettingsTypeDef
 ):
     pass
 
-
-_RequiredUdpOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredUdpOutputSettingsOutputTypeDef",
+_RequiredUdpOutputSettingsTypeDef = TypedDict(
+    "_RequiredUdpOutputSettingsTypeDef",
     {
-        "ContainerSettings": UdpContainerSettingsOutputTypeDef,
-        "Destination": OutputLocationRefOutputTypeDef,
+        "ContainerSettings": UdpContainerSettingsTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalUdpOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalUdpOutputSettingsOutputTypeDef",
+_OptionalUdpOutputSettingsTypeDef = TypedDict(
+    "_OptionalUdpOutputSettingsTypeDef",
     {
         "BufferMsec": int,
-        "FecOutputSettings": FecOutputSettingsOutputTypeDef,
+        "FecOutputSettings": FecOutputSettingsTypeDef,
     },
     total=False,
 )
 
-
-class UdpOutputSettingsOutputTypeDef(
-    _RequiredUdpOutputSettingsOutputTypeDef, _OptionalUdpOutputSettingsOutputTypeDef
+class UdpOutputSettingsTypeDef(
+    _RequiredUdpOutputSettingsTypeDef, _OptionalUdpOutputSettingsTypeDef
 ):
     pass
 
-
 _RequiredAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsOutputTypeDef",
     {
         "SecondaryInputId": str,
     },
 )
 _OptionalAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
     "_OptionalAutomaticInputFailoverSettingsOutputTypeDef",
     {
         "ErrorClearTimeMsec": int,
-        "FailoverConditions": List[FailoverConditionOutputTypeDef],
+        "FailoverConditions": List[FailoverConditionTypeDef],
         "InputPreference": InputPreferenceType,
     },
     total=False,
 )
 
-
 class AutomaticInputFailoverSettingsOutputTypeDef(
     _RequiredAutomaticInputFailoverSettingsOutputTypeDef,
     _OptionalAutomaticInputFailoverSettingsOutputTypeDef,
 ):
     pass
 
-
 _RequiredAutomaticInputFailoverSettingsTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsTypeDef",
     {
         "SecondaryInputId": str,
     },
 )
 _OptionalAutomaticInputFailoverSettingsTypeDef = TypedDict(
@@ -6778,28 +5145,26 @@
         "ErrorClearTimeMsec": int,
         "FailoverConditions": Sequence[FailoverConditionTypeDef],
         "InputPreference": InputPreferenceType,
     },
     total=False,
 )
 
-
 class AutomaticInputFailoverSettingsTypeDef(
     _RequiredAutomaticInputFailoverSettingsTypeDef, _OptionalAutomaticInputFailoverSettingsTypeDef
 ):
     pass
 
-
 VideoCodecSettingsOutputTypeDef = TypedDict(
     "VideoCodecSettingsOutputTypeDef",
     {
-        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
         "H264Settings": H264SettingsOutputTypeDef,
         "H265Settings": H265SettingsOutputTypeDef,
-        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsTypeDef,
     },
     total=False,
 )
 
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
@@ -6811,128 +5176,126 @@
     total=False,
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePartnerInputResponseTypeDef = TypedDict(
     "CreatePartnerInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHlsOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredHlsOutputSettingsOutputTypeDef",
+_RequiredHlsOutputSettingsTypeDef = TypedDict(
+    "_RequiredHlsOutputSettingsTypeDef",
     {
-        "HlsSettings": HlsSettingsOutputTypeDef,
+        "HlsSettings": HlsSettingsTypeDef,
     },
 )
-_OptionalHlsOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalHlsOutputSettingsOutputTypeDef",
+_OptionalHlsOutputSettingsTypeDef = TypedDict(
+    "_OptionalHlsOutputSettingsTypeDef",
     {
         "H265PackagingType": HlsH265PackagingTypeType,
         "NameModifier": str,
         "SegmentModifier": str,
     },
     total=False,
 )
 
-
-class HlsOutputSettingsOutputTypeDef(
-    _RequiredHlsOutputSettingsOutputTypeDef, _OptionalHlsOutputSettingsOutputTypeDef
+class HlsOutputSettingsTypeDef(
+    _RequiredHlsOutputSettingsTypeDef, _OptionalHlsOutputSettingsTypeDef
 ):
     pass
 
-
 CreateMultiplexResponseTypeDef = TypedDict(
     "CreateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMultiplexResponseTypeDef = TypedDict(
     "UpdateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
+    "CreateMultiplexProgramRequestRequestTypeDef",
+    {
+        "MultiplexId": str,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "ProgramName": str,
+        "RequestId": str,
     },
 )
 
 DeleteMultiplexProgramResponseTypeDef = TypedDict(
     "DeleteMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMultiplexProgramResponseTypeDef = TypedDict(
     "DescribeMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MultiplexProgramTypeDef = TypedDict(
     "MultiplexProgramTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
     },
     total=False,
 )
 
-CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
-    "CreateMultiplexProgramRequestRequestTypeDef",
-    {
-        "MultiplexId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
-        "ProgramName": str,
-        "RequestId": str,
-    },
-)
-
 _RequiredUpdateMultiplexProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
 )
@@ -6940,52 +5303,48 @@
     "_OptionalUpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMultiplexProgramRequestRequestTypeDef(
     _RequiredUpdateMultiplexProgramRequestRequestTypeDef,
     _OptionalUpdateMultiplexProgramRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredAudioDescriptionOutputTypeDef = TypedDict(
     "_RequiredAudioDescriptionOutputTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
 _OptionalAudioDescriptionOutputTypeDef = TypedDict(
     "_OptionalAudioDescriptionOutputTypeDef",
     {
-        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioType": AudioTypeType,
         "AudioTypeControl": AudioDescriptionAudioTypeControlType,
-        "AudioWatermarkingSettings": AudioWatermarkSettingsOutputTypeDef,
+        "AudioWatermarkingSettings": AudioWatermarkSettingsTypeDef,
         "CodecSettings": AudioCodecSettingsOutputTypeDef,
         "LanguageCode": str,
         "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "StreamName": str,
     },
     total=False,
 )
 
-
 class AudioDescriptionOutputTypeDef(
     _RequiredAudioDescriptionOutputTypeDef, _OptionalAudioDescriptionOutputTypeDef
 ):
     pass
 
-
 _RequiredAudioDescriptionTypeDef = TypedDict(
     "_RequiredAudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
@@ -7001,44 +5360,35 @@
         "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
         "RemixSettings": RemixSettingsTypeDef,
         "StreamName": str,
     },
     total=False,
 )
 
-
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
-
-Scte35DescriptorOutputTypeDef = TypedDict(
-    "Scte35DescriptorOutputTypeDef",
-    {
-        "Scte35DescriptorSettings": Scte35DescriptorSettingsOutputTypeDef,
-    },
-)
-
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
 OutputGroupSettingsOutputTypeDef = TypedDict(
     "OutputGroupSettingsOutputTypeDef",
     {
-        "ArchiveGroupSettings": ArchiveGroupSettingsOutputTypeDef,
-        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsOutputTypeDef,
+        "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
+        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
-        "MediaPackageGroupSettings": MediaPackageGroupSettingsOutputTypeDef,
-        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "MultiplexGroupSettings": Dict[str, Any],
         "RtmpGroupSettings": RtmpGroupSettingsOutputTypeDef,
-        "UdpGroupSettings": UdpGroupSettingsOutputTypeDef,
+        "UdpGroupSettings": UdpGroupSettingsTypeDef,
     },
     total=False,
 )
 
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
@@ -7059,19 +5409,19 @@
     {
         "AudioSelectors": List[AudioSelectorOutputTypeDef],
         "CaptionSelectors": List[CaptionSelectorOutputTypeDef],
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
         "FilterStrength": int,
         "InputFilter": InputFilterType,
-        "NetworkInputSettings": NetworkInputSettingsOutputTypeDef,
+        "NetworkInputSettings": NetworkInputSettingsTypeDef,
         "Scte35Pid": int,
         "Smpte2038DataPreference": Smpte2038DataPreferenceType,
         "SourceEndBehavior": InputSourceEndBehaviorType,
-        "VideoSelector": VideoSelectorOutputTypeDef,
+        "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
 InputSettingsTypeDef = TypedDict(
     "InputSettingsTypeDef",
     {
@@ -7105,21 +5455,19 @@
         "ScalingBehavior": VideoDescriptionScalingBehaviorType,
         "Sharpness": int,
         "Width": int,
     },
     total=False,
 )
 
-
 class VideoDescriptionOutputTypeDef(
     _RequiredVideoDescriptionOutputTypeDef, _OptionalVideoDescriptionOutputTypeDef
 ):
     pass
 
-
 _RequiredVideoDescriptionTypeDef = TypedDict(
     "_RequiredVideoDescriptionTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVideoDescriptionTypeDef = TypedDict(
@@ -7131,54 +5479,52 @@
         "ScalingBehavior": VideoDescriptionScalingBehaviorType,
         "Sharpness": int,
         "Width": int,
     },
     total=False,
 )
 
-
 class VideoDescriptionTypeDef(_RequiredVideoDescriptionTypeDef, _OptionalVideoDescriptionTypeDef):
     pass
 
-
-OutputSettingsOutputTypeDef = TypedDict(
-    "OutputSettingsOutputTypeDef",
+OutputSettingsTypeDef = TypedDict(
+    "OutputSettingsTypeDef",
     {
-        "ArchiveOutputSettings": ArchiveOutputSettingsOutputTypeDef,
-        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsOutputTypeDef,
-        "HlsOutputSettings": HlsOutputSettingsOutputTypeDef,
-        "MediaPackageOutputSettings": Dict[str, Any],
-        "MsSmoothOutputSettings": MsSmoothOutputSettingsOutputTypeDef,
-        "MultiplexOutputSettings": MultiplexOutputSettingsOutputTypeDef,
-        "RtmpOutputSettings": RtmpOutputSettingsOutputTypeDef,
-        "UdpOutputSettings": UdpOutputSettingsOutputTypeDef,
+        "ArchiveOutputSettings": ArchiveOutputSettingsTypeDef,
+        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsTypeDef,
+        "HlsOutputSettings": HlsOutputSettingsTypeDef,
+        "MediaPackageOutputSettings": Mapping[str, Any],
+        "MsSmoothOutputSettings": MsSmoothOutputSettingsTypeDef,
+        "MultiplexOutputSettings": MultiplexOutputSettingsTypeDef,
+        "RtmpOutputSettings": RtmpOutputSettingsTypeDef,
+        "UdpOutputSettings": UdpOutputSettingsTypeDef,
     },
     total=False,
 )
 
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     {
-        "Scte35Descriptors": List[Scte35DescriptorOutputTypeDef],
+        "Scte35Descriptors": List[Scte35DescriptorTypeDef],
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
@@ -7206,51 +5552,47 @@
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
-        "OutputSettings": OutputSettingsOutputTypeDef,
+        "OutputSettings": OutputSettingsTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
-        "AudioDescriptionNames": List[str],
-        "CaptionDescriptionNames": List[str],
+        "AudioDescriptionNames": Sequence[str],
+        "CaptionDescriptionNames": Sequence[str],
         "OutputName": str,
         "VideoDescriptionName": str,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-
 ScheduleActionSettingsOutputTypeDef = TypedDict(
     "ScheduleActionSettingsOutputTypeDef",
     {
-        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
-        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
+        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
+        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
         "InputPrepareSettings": InputPrepareScheduleActionSettingsOutputTypeDef,
         "InputSwitchSettings": InputSwitchScheduleActionSettingsOutputTypeDef,
-        "MotionGraphicsImageActivateSettings": (
-            MotionGraphicsActivateScheduleActionSettingsOutputTypeDef
-        ),
+        "MotionGraphicsImageActivateSettings": MotionGraphicsActivateScheduleActionSettingsTypeDef,
         "MotionGraphicsImageDeactivateSettings": Dict[str, Any],
         "PauseStateSettings": PauseStateScheduleActionSettingsOutputTypeDef,
-        "Scte35InputSettings": Scte35InputScheduleActionSettingsOutputTypeDef,
-        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
-        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+        "Scte35InputSettings": Scte35InputScheduleActionSettingsTypeDef,
+        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
+        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsTypeDef,
         "Scte35TimeSignalSettings": Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
-        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsOutputTypeDef,
-        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
+        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsTypeDef,
+        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsTypeDef,
     },
     total=False,
 )
 
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
@@ -7271,21 +5613,21 @@
     total=False,
 )
 
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
@@ -7305,21 +5647,19 @@
     "_OptionalOutputGroupOutputTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class OutputGroupOutputTypeDef(
     _RequiredOutputGroupOutputTypeDef, _OptionalOutputGroupOutputTypeDef
 ):
     pass
 
-
 _RequiredOutputGroupTypeDef = TypedDict(
     "_RequiredOutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
 )
@@ -7327,19 +5667,17 @@
     "_OptionalOutputGroupTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class OutputGroupTypeDef(_RequiredOutputGroupTypeDef, _OptionalOutputGroupTypeDef):
     pass
 
-
 ScheduleActionOutputTypeDef = TypedDict(
     "ScheduleActionOutputTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
     },
@@ -7355,50 +5693,48 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEncoderSettingsOutputTypeDef = TypedDict(
     "_RequiredEncoderSettingsOutputTypeDef",
     {
         "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
         "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
     },
 )
 _OptionalEncoderSettingsOutputTypeDef = TypedDict(
     "_OptionalEncoderSettingsOutputTypeDef",
     {
-        "AvailBlanking": AvailBlankingOutputTypeDef,
-        "AvailConfiguration": AvailConfigurationOutputTypeDef,
-        "BlackoutSlate": BlackoutSlateOutputTypeDef,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "AvailConfiguration": AvailConfigurationTypeDef,
+        "BlackoutSlate": BlackoutSlateTypeDef,
         "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
-        "FeatureActivations": FeatureActivationsOutputTypeDef,
-        "GlobalConfiguration": GlobalConfigurationOutputTypeDef,
+        "FeatureActivations": FeatureActivationsTypeDef,
+        "GlobalConfiguration": GlobalConfigurationTypeDef,
         "MotionGraphicsConfiguration": MotionGraphicsConfigurationOutputTypeDef,
-        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
-        "ThumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "ThumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class EncoderSettingsOutputTypeDef(
     _RequiredEncoderSettingsOutputTypeDef, _OptionalEncoderSettingsOutputTypeDef
 ):
     pass
 
-
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": Sequence[VideoDescriptionTypeDef],
@@ -7416,19 +5752,17 @@
         "MotionGraphicsConfiguration": MotionGraphicsConfigurationTypeDef,
         "NielsenConfiguration": NielsenConfigurationTypeDef,
         "ThumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class EncoderSettingsTypeDef(_RequiredEncoderSettingsTypeDef, _OptionalEncoderSettingsTypeDef):
     pass
 
-
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
         "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 
@@ -7440,37 +5774,37 @@
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
         "ScheduleActions": List[ScheduleActionOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchScheduleActionCreateRequestTypeDef = TypedDict(
     "BatchScheduleActionCreateRequestTypeDef",
     {
         "ScheduleActions": Sequence[ScheduleActionTypeDef],
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
@@ -7480,107 +5814,107 @@
     total=False,
 )
 
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
@@ -7619,27 +5953,25 @@
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 BatchUpdateScheduleResponseTypeDef = TypedDict(
     "BatchUpdateScheduleResponseTypeDef",
     {
         "Creates": BatchScheduleActionCreateResultTypeDef,
         "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -7650,38 +5982,36 @@
     {
         "Creates": BatchScheduleActionCreateRequestTypeDef,
         "Deletes": BatchScheduleActionDeleteRequestTypeDef,
     },
     total=False,
 )
 
-
 class BatchUpdateScheduleRequestRequestTypeDef(
     _RequiredBatchUpdateScheduleRequestRequestTypeDef,
     _OptionalBatchUpdateScheduleRequestRequestTypeDef,
 ):
     pass
 
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelClassResponseTypeDef = TypedDict(
     "UpdateChannelClassResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for medialive service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_medialive.type_defs import AacSettingsOutputTypeDef
+    from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
 
-    data: AacSettingsOutputTypeDef = {...}
+    data: AacSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from botocore.response import StreamingBody
@@ -285,94 +285,63 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
-    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
-    "AccountConfigurationOutputTypeDef",
     "AccountConfigurationTypeDef",
-    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
-    "ArchiveS3SettingsOutputTypeDef",
     "ArchiveS3SettingsTypeDef",
-    "OutputLocationRefOutputTypeDef",
     "OutputLocationRefTypeDef",
-    "InputChannelLevelOutputTypeDef",
     "InputChannelLevelTypeDef",
-    "Eac3AtmosSettingsOutputTypeDef",
-    "Eac3SettingsOutputTypeDef",
-    "Mp2SettingsOutputTypeDef",
-    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "WavSettingsTypeDef",
-    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
-    "AudioDolbyEDecodeOutputTypeDef",
     "AudioDolbyEDecodeTypeDef",
-    "AudioHlsRenditionSelectionOutputTypeDef",
     "AudioHlsRenditionSelectionTypeDef",
-    "AudioLanguageSelectionOutputTypeDef",
     "AudioLanguageSelectionTypeDef",
-    "InputLocationOutputTypeDef",
-    "AudioPidSelectionOutputTypeDef",
+    "InputLocationTypeDef",
     "AudioPidSelectionTypeDef",
-    "AudioSilenceFailoverSettingsOutputTypeDef",
     "AudioSilenceFailoverSettingsTypeDef",
-    "AudioTrackOutputTypeDef",
     "AudioTrackTypeDef",
-    "InputLocationTypeDef",
-    "EsamOutputTypeDef",
-    "Scte35SpliceInsertOutputTypeDef",
-    "Scte35TimeSignalAposOutputTypeDef",
     "EsamTypeDef",
     "Scte35SpliceInsertTypeDef",
     "Scte35TimeSignalAposTypeDef",
     "BatchDeleteRequestRequestTypeDef",
     "BatchFailedResultModelTypeDef",
     "BatchSuccessfulResultModelTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchScheduleActionDeleteRequestTypeDef",
     "BatchStartRequestRequestTypeDef",
     "BatchStopRequestRequestTypeDef",
     "CancelInputDeviceTransferRequestRequestTypeDef",
-    "EbuTtDDestinationSettingsOutputTypeDef",
-    "TtmlDestinationSettingsOutputTypeDef",
-    "WebvttDestinationSettingsOutputTypeDef",
     "EbuTtDDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
-    "CaptionLanguageMappingOutputTypeDef",
     "CaptionLanguageMappingTypeDef",
-    "CaptionRectangleOutputTypeDef",
     "CaptionRectangleTypeDef",
-    "DvbSubSourceSettingsOutputTypeDef",
-    "EmbeddedSourceSettingsOutputTypeDef",
-    "Scte20SourceSettingsOutputTypeDef",
-    "Scte27SourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "Scte20SourceSettingsTypeDef",
     "Scte27SourceSettingsTypeDef",
-    "CdiInputSpecificationOutputTypeDef",
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
-    "InputSpecificationOutputTypeDef",
+    "InputSpecificationTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
-    "InputSpecificationTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
     "MediaConnectFlowRequestTypeDef",
@@ -383,218 +352,155 @@
     "DeleteChannelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DeleteInputSecurityGroupRequestRequestTypeDef",
     "DeleteMultiplexProgramRequestRequestTypeDef",
     "MultiplexProgramPacketIdentifiersMapTypeDef",
     "MultiplexProgramPipelineDetailTypeDef",
     "DeleteMultiplexRequestRequestTypeDef",
-    "MultiplexSettingsOutputTypeDef",
     "DeleteReservationRequestRequestTypeDef",
-    "RenewalSettingsOutputTypeDef",
+    "RenewalSettingsTypeDef",
     "ReservationResourceSpecificationTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
-    "DescribeInputDeviceThumbnailResponseTypeDef",
     "DescribeInputRequestRequestTypeDef",
-    "InputDeviceSettingsOutputTypeDef",
     "InputSourceTypeDef",
     "MediaConnectFlowTypeDef",
     "DescribeInputSecurityGroupRequestRequestTypeDef",
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
-    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DescribeThumbnailsRequestRequestTypeDef",
-    "DvbNitSettingsOutputTypeDef",
-    "DvbSdtSettingsOutputTypeDef",
-    "DvbTdtSettingsOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FeatureActivationsOutputTypeDef",
-    "NielsenConfigurationOutputTypeDef",
-    "ThumbnailConfigurationOutputTypeDef",
-    "TimecodeConfigOutputTypeDef",
+    "DvbNitSettingsTypeDef",
+    "DvbSdtSettingsTypeDef",
+    "DvbTdtSettingsTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
-    "InputLossFailoverSettingsOutputTypeDef",
-    "VideoBlackFailoverSettingsOutputTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
-    "FecOutputSettingsOutputTypeDef",
-    "FixedModeScheduleActionStartSettingsOutputTypeDef",
+    "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
-    "Fmp4HlsSettingsOutputTypeDef",
-    "FollowModeScheduleActionStartSettingsOutputTypeDef",
+    "Fmp4HlsSettingsTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
-    "FrameCaptureS3SettingsOutputTypeDef",
     "FrameCaptureS3SettingsTypeDef",
-    "FrameCaptureOutputSettingsOutputTypeDef",
-    "TimecodeBurninSettingsOutputTypeDef",
+    "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
     "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
-    "TemporalFilterSettingsOutputTypeDef",
     "TemporalFilterSettingsTypeDef",
-    "Hdr10SettingsOutputTypeDef",
     "Hdr10SettingsTypeDef",
-    "HlsAkamaiSettingsOutputTypeDef",
     "HlsAkamaiSettingsTypeDef",
-    "HlsBasicPutSettingsOutputTypeDef",
     "HlsBasicPutSettingsTypeDef",
-    "HlsMediaStoreSettingsOutputTypeDef",
-    "HlsS3SettingsOutputTypeDef",
-    "HlsWebdavSettingsOutputTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
     "HlsWebdavSettingsTypeDef",
-    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
-    "HlsInputSettingsOutputTypeDef",
     "HlsInputSettingsTypeDef",
-    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
-    "StartTimecodeOutputTypeDef",
-    "StopTimecodeOutputTypeDef",
     "StartTimecodeTypeDef",
     "StopTimecodeTypeDef",
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "InputDeviceRequestTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
-    "ListInputsRequestListInputsPaginateTypeDef",
     "ListInputsRequestRequestTypeDef",
-    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "M3u8SettingsOutputTypeDef",
+    "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
-    "MediaPackageOutputDestinationSettingsOutputTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
-    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
-    "MsSmoothOutputSettingsOutputTypeDef",
+    "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
-    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
-    "MultiplexProgramServiceDescriptorOutputTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
-    "MultiplexStatmuxVideoSettingsOutputTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
-    "NielsenCBETOutputTypeDef",
     "NielsenCBETTypeDef",
-    "NielsenNaesIiNwOutputTypeDef",
     "NielsenNaesIiNwTypeDef",
-    "OutputDestinationSettingsOutputTypeDef",
     "OutputDestinationSettingsTypeDef",
     "RtmpGroupSettingsOutputTypeDef",
-    "UdpGroupSettingsOutputTypeDef",
-    "RtmpGroupSettingsTypeDef",
     "UdpGroupSettingsTypeDef",
-    "PaginatorConfigTypeDef",
-    "PipelinePauseStateSettingsOutputTypeDef",
+    "RtmpGroupSettingsTypeDef",
     "PipelinePauseStateSettingsTypeDef",
-    "RenewalSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "Scte35InputScheduleActionSettingsOutputTypeDef",
-    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
-    "Scte35SpliceInsertScheduleActionSettingsOutputTypeDef",
-    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
-    "Scte35DeliveryRestrictionsOutputTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
-    "VideoSelectorPidOutputTypeDef",
     "VideoSelectorPidTypeDef",
-    "VideoSelectorProgramIdOutputTypeDef",
     "VideoSelectorProgramIdTypeDef",
-    "DescribeAccountConfigurationResponseTypeDef",
-    "UpdateAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
-    "ArchiveCdnSettingsOutputTypeDef",
     "ArchiveCdnSettingsTypeDef",
-    "MediaPackageGroupSettingsOutputTypeDef",
-    "MsSmoothGroupSettingsOutputTypeDef",
-    "MultiplexOutputSettingsOutputTypeDef",
-    "RtmpOutputSettingsOutputTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
+    "MultiplexOutputSettingsTypeDef",
+    "RtmpOutputSettingsTypeDef",
     "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
     "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
-    "AudioOnlyHlsSettingsOutputTypeDef",
-    "AvailBlankingOutputTypeDef",
-    "BlackoutSlateOutputTypeDef",
-    "BurnInDestinationSettingsOutputTypeDef",
-    "DvbSubDestinationSettingsOutputTypeDef",
-    "InputLossBehaviorOutputTypeDef",
-    "StaticImageActivateScheduleActionSettingsOutputTypeDef",
-    "StaticKeySettingsOutputTypeDef",
-    "AudioTrackSelectionOutputTypeDef",
-    "AudioTrackSelectionTypeDef",
+    "AudioOnlyHlsSettingsTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AvailSettingsOutputTypeDef",
+    "AudioTrackSelectionOutputTypeDef",
+    "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
-    "TeletextSourceSettingsOutputTypeDef",
+    "DescribeAccountConfigurationResponseTypeDef",
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateAccountConfigurationResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
+    "PurchaseOfferingRequestRequestTypeDef",
+    "UpdateReservationRequestRequestTypeDef",
     "DeleteReservationResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "DescribeChannelRequestChannelCreatedWaitTypeDef",
     "DescribeChannelRequestChannelDeletedWaitTypeDef",
@@ -608,160 +514,142 @@
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
-    "M2tsSettingsOutputTypeDef",
-    "FailoverConditionSettingsOutputTypeDef",
+    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    "ListInputsRequestListInputsPaginateTypeDef",
+    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    "M2tsSettingsTypeDef",
     "FailoverConditionSettingsTypeDef",
     "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
-    "FrameCaptureCdnSettingsOutputTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
-    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
-    "H264FilterSettingsOutputTypeDef",
-    "H265FilterSettingsOutputTypeDef",
-    "Mpeg2FilterSettingsOutputTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
     "H265ColorSpaceSettingsOutputTypeDef",
-    "VideoSelectorColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
-    "HlsCdnSettingsOutputTypeDef",
     "HlsCdnSettingsTypeDef",
-    "NetworkInputSettingsOutputTypeDef",
     "NetworkInputSettingsTypeDef",
-    "InputClippingSettingsOutputTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
-    "StandardHlsSettingsOutputTypeDef",
+    "StandardHlsSettingsTypeDef",
     "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
-    "MultiplexVideoSettingsOutputTypeDef",
     "MultiplexVideoSettingsTypeDef",
-    "NielsenWatermarksSettingsOutputTypeDef",
     "NielsenWatermarksSettingsTypeDef",
     "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
     "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
-    "PurchaseOfferingRequestRequestTypeDef",
-    "UpdateReservationRequestRequestTypeDef",
-    "Scte35SegmentationDescriptorOutputTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
     "ThumbnailDetailTypeDef",
-    "VideoSelectorSettingsOutputTypeDef",
     "VideoSelectorSettingsTypeDef",
-    "ArchiveGroupSettingsOutputTypeDef",
     "ArchiveGroupSettingsTypeDef",
     "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
     "CaptionDestinationSettingsOutputTypeDef",
-    "GlobalConfigurationOutputTypeDef",
-    "KeyProviderSettingsOutputTypeDef",
-    "AudioSelectorSettingsOutputTypeDef",
-    "AudioSelectorSettingsTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "GlobalConfigurationTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AvailConfigurationOutputTypeDef",
+    "AudioSelectorSettingsOutputTypeDef",
+    "AudioSelectorSettingsTypeDef",
     "AvailConfigurationTypeDef",
     "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
-    "ArchiveContainerSettingsOutputTypeDef",
-    "UdpContainerSettingsOutputTypeDef",
-    "FailoverConditionOutputTypeDef",
+    "ArchiveContainerSettingsTypeDef",
+    "UdpContainerSettingsTypeDef",
     "FailoverConditionTypeDef",
-    "FrameCaptureGroupSettingsOutputTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
     "H264SettingsOutputTypeDef",
-    "Mpeg2SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
     "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
     "InputPrepareScheduleActionSettingsOutputTypeDef",
-    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
-    "HlsSettingsOutputTypeDef",
+    "HlsSettingsTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
-    "MultiplexProgramSettingsOutputTypeDef",
     "MultiplexProgramSettingsTypeDef",
-    "AudioWatermarkSettingsOutputTypeDef",
     "AudioWatermarkSettingsTypeDef",
     "UpdateChannelClassRequestRequestTypeDef",
-    "Scte35DescriptorSettingsOutputTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
-    "VideoSelectorOutputTypeDef",
     "VideoSelectorTypeDef",
     "CaptionDescriptionOutputTypeDef",
+    "CaptionDescriptionTypeDef",
     "HlsGroupSettingsOutputTypeDef",
+    "HlsGroupSettingsTypeDef",
     "AudioSelectorOutputTypeDef",
     "AudioSelectorTypeDef",
-    "CaptionDescriptionTypeDef",
-    "HlsGroupSettingsTypeDef",
     "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
-    "ArchiveOutputSettingsOutputTypeDef",
-    "UdpOutputSettingsOutputTypeDef",
+    "ArchiveOutputSettingsTypeDef",
+    "UdpOutputSettingsTypeDef",
     "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
     "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
-    "HlsOutputSettingsOutputTypeDef",
+    "HlsOutputSettingsTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
+    "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
-    "CreateMultiplexProgramRequestRequestTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
     "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
-    "Scte35DescriptorOutputTypeDef",
     "Scte35DescriptorTypeDef",
     "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
     "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
     "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
-    "OutputSettingsOutputTypeDef",
+    "OutputSettingsTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
     "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
@@ -789,30 +677,14 @@
     "BatchUpdateScheduleResponseTypeDef",
     "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
-AacSettingsOutputTypeDef = TypedDict(
-    "AacSettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "CodingMode": AacCodingModeType,
-        "InputType": AacInputTypeType,
-        "Profile": AacProfileType,
-        "RateControlMode": AacRateControlModeType,
-        "RawFormat": AacRawFormatType,
-        "SampleRate": float,
-        "Spec": AacSpecType,
-        "VbrQuality": AacVbrQualityType,
-    },
-    total=False,
-)
-
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": AacCodingModeType,
         "InputType": AacInputTypeType,
         "Profile": AacProfileType,
@@ -821,28 +693,14 @@
         "SampleRate": float,
         "Spec": AacSpecType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
-Ac3SettingsOutputTypeDef = TypedDict(
-    "Ac3SettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "BitstreamMode": Ac3BitstreamModeType,
-        "CodingMode": Ac3CodingModeType,
-        "Dialnorm": int,
-        "DrcProfile": Ac3DrcProfileType,
-        "LfeFilter": Ac3LfeFilterType,
-        "MetadataControl": Ac3MetadataControlType,
-    },
-    total=False,
-)
-
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": float,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -856,155 +714,54 @@
 AcceptInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
-AccountConfigurationOutputTypeDef = TypedDict(
-    "AccountConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
 AccountConfigurationTypeDef = TypedDict(
     "AccountConfigurationTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-AncillarySourceSettingsOutputTypeDef = TypedDict(
-    "AncillarySourceSettingsOutputTypeDef",
-    {
-        "SourceAncillaryChannelNumber": int,
-    },
-    total=False,
-)
-
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "SourceAncillaryChannelNumber": int,
     },
     total=False,
 )
 
-ArchiveS3SettingsOutputTypeDef = TypedDict(
-    "ArchiveS3SettingsOutputTypeDef",
-    {
-        "CannedAcl": S3CannedAclType,
-    },
-    total=False,
-)
-
 ArchiveS3SettingsTypeDef = TypedDict(
     "ArchiveS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
-OutputLocationRefOutputTypeDef = TypedDict(
-    "OutputLocationRefOutputTypeDef",
-    {
-        "DestinationRefId": str,
-    },
-    total=False,
-)
-
 OutputLocationRefTypeDef = TypedDict(
     "OutputLocationRefTypeDef",
     {
         "DestinationRefId": str,
     },
     total=False,
 )
 
-InputChannelLevelOutputTypeDef = TypedDict(
-    "InputChannelLevelOutputTypeDef",
-    {
-        "Gain": int,
-        "InputChannel": int,
-    },
-)
-
 InputChannelLevelTypeDef = TypedDict(
     "InputChannelLevelTypeDef",
     {
         "Gain": int,
         "InputChannel": int,
     },
 )
 
-Eac3AtmosSettingsOutputTypeDef = TypedDict(
-    "Eac3AtmosSettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "CodingMode": Eac3AtmosCodingModeType,
-        "Dialnorm": int,
-        "DrcLine": Eac3AtmosDrcLineType,
-        "DrcRf": Eac3AtmosDrcRfType,
-        "HeightTrim": float,
-        "SurroundTrim": float,
-    },
-    total=False,
-)
-
-Eac3SettingsOutputTypeDef = TypedDict(
-    "Eac3SettingsOutputTypeDef",
-    {
-        "AttenuationControl": Eac3AttenuationControlType,
-        "Bitrate": float,
-        "BitstreamMode": Eac3BitstreamModeType,
-        "CodingMode": Eac3CodingModeType,
-        "DcFilter": Eac3DcFilterType,
-        "Dialnorm": int,
-        "DrcLine": Eac3DrcLineType,
-        "DrcRf": Eac3DrcRfType,
-        "LfeControl": Eac3LfeControlType,
-        "LfeFilter": Eac3LfeFilterType,
-        "LoRoCenterMixLevel": float,
-        "LoRoSurroundMixLevel": float,
-        "LtRtCenterMixLevel": float,
-        "LtRtSurroundMixLevel": float,
-        "MetadataControl": Eac3MetadataControlType,
-        "PassthroughControl": Eac3PassthroughControlType,
-        "PhaseControl": Eac3PhaseControlType,
-        "StereoDownmix": Eac3StereoDownmixType,
-        "SurroundExMode": Eac3SurroundExModeType,
-        "SurroundMode": Eac3SurroundModeType,
-    },
-    total=False,
-)
-
-Mp2SettingsOutputTypeDef = TypedDict(
-    "Mp2SettingsOutputTypeDef",
-    {
-        "Bitrate": float,
-        "CodingMode": Mp2CodingModeType,
-        "SampleRate": float,
-    },
-    total=False,
-)
-
-WavSettingsOutputTypeDef = TypedDict(
-    "WavSettingsOutputTypeDef",
-    {
-        "BitDepth": float,
-        "CodingMode": WavCodingModeType,
-        "SampleRate": float,
-    },
-    total=False,
-)
-
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": Eac3AtmosCodingModeType,
         "Dialnorm": int,
         "DrcLine": Eac3AtmosDrcLineType,
@@ -1058,248 +815,115 @@
         "BitDepth": float,
         "CodingMode": WavCodingModeType,
         "SampleRate": float,
     },
     total=False,
 )
 
-AudioNormalizationSettingsOutputTypeDef = TypedDict(
-    "AudioNormalizationSettingsOutputTypeDef",
-    {
-        "Algorithm": AudioNormalizationAlgorithmType,
-        "AlgorithmControl": Literal["CORRECT_AUDIO"],
-        "TargetLkfs": float,
-    },
-    total=False,
-)
-
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": Literal["CORRECT_AUDIO"],
         "TargetLkfs": float,
     },
     total=False,
 )
 
-AudioDolbyEDecodeOutputTypeDef = TypedDict(
-    "AudioDolbyEDecodeOutputTypeDef",
-    {
-        "ProgramSelection": DolbyEProgramSelectionType,
-    },
-)
-
 AudioDolbyEDecodeTypeDef = TypedDict(
     "AudioDolbyEDecodeTypeDef",
     {
         "ProgramSelection": DolbyEProgramSelectionType,
     },
 )
 
-AudioHlsRenditionSelectionOutputTypeDef = TypedDict(
-    "AudioHlsRenditionSelectionOutputTypeDef",
-    {
-        "GroupId": str,
-        "Name": str,
-    },
-)
-
 AudioHlsRenditionSelectionTypeDef = TypedDict(
     "AudioHlsRenditionSelectionTypeDef",
     {
         "GroupId": str,
         "Name": str,
     },
 )
 
-_RequiredAudioLanguageSelectionOutputTypeDef = TypedDict(
-    "_RequiredAudioLanguageSelectionOutputTypeDef",
-    {
-        "LanguageCode": str,
-    },
-)
-_OptionalAudioLanguageSelectionOutputTypeDef = TypedDict(
-    "_OptionalAudioLanguageSelectionOutputTypeDef",
-    {
-        "LanguageSelectionPolicy": AudioLanguageSelectionPolicyType,
-    },
-    total=False,
-)
-
-class AudioLanguageSelectionOutputTypeDef(
-    _RequiredAudioLanguageSelectionOutputTypeDef, _OptionalAudioLanguageSelectionOutputTypeDef
-):
-    pass
-
 _RequiredAudioLanguageSelectionTypeDef = TypedDict(
     "_RequiredAudioLanguageSelectionTypeDef",
     {
         "LanguageCode": str,
     },
 )
 _OptionalAudioLanguageSelectionTypeDef = TypedDict(
     "_OptionalAudioLanguageSelectionTypeDef",
     {
         "LanguageSelectionPolicy": AudioLanguageSelectionPolicyType,
     },
     total=False,
 )
 
+
 class AudioLanguageSelectionTypeDef(
     _RequiredAudioLanguageSelectionTypeDef, _OptionalAudioLanguageSelectionTypeDef
 ):
     pass
 
-_RequiredInputLocationOutputTypeDef = TypedDict(
-    "_RequiredInputLocationOutputTypeDef",
+
+_RequiredInputLocationTypeDef = TypedDict(
+    "_RequiredInputLocationTypeDef",
     {
         "Uri": str,
     },
 )
-_OptionalInputLocationOutputTypeDef = TypedDict(
-    "_OptionalInputLocationOutputTypeDef",
+_OptionalInputLocationTypeDef = TypedDict(
+    "_OptionalInputLocationTypeDef",
     {
         "PasswordParam": str,
         "Username": str,
     },
     total=False,
 )
 
-class InputLocationOutputTypeDef(
-    _RequiredInputLocationOutputTypeDef, _OptionalInputLocationOutputTypeDef
-):
+
+class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
     pass
 
-AudioPidSelectionOutputTypeDef = TypedDict(
-    "AudioPidSelectionOutputTypeDef",
-    {
-        "Pid": int,
-    },
-)
 
 AudioPidSelectionTypeDef = TypedDict(
     "AudioPidSelectionTypeDef",
     {
         "Pid": int,
     },
 )
 
-_RequiredAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
-    "_RequiredAudioSilenceFailoverSettingsOutputTypeDef",
-    {
-        "AudioSelectorName": str,
-    },
-)
-_OptionalAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
-    "_OptionalAudioSilenceFailoverSettingsOutputTypeDef",
-    {
-        "AudioSilenceThresholdMsec": int,
-    },
-    total=False,
-)
-
-class AudioSilenceFailoverSettingsOutputTypeDef(
-    _RequiredAudioSilenceFailoverSettingsOutputTypeDef,
-    _OptionalAudioSilenceFailoverSettingsOutputTypeDef,
-):
-    pass
-
 _RequiredAudioSilenceFailoverSettingsTypeDef = TypedDict(
     "_RequiredAudioSilenceFailoverSettingsTypeDef",
     {
         "AudioSelectorName": str,
     },
 )
 _OptionalAudioSilenceFailoverSettingsTypeDef = TypedDict(
     "_OptionalAudioSilenceFailoverSettingsTypeDef",
     {
         "AudioSilenceThresholdMsec": int,
     },
     total=False,
 )
 
+
 class AudioSilenceFailoverSettingsTypeDef(
     _RequiredAudioSilenceFailoverSettingsTypeDef, _OptionalAudioSilenceFailoverSettingsTypeDef
 ):
     pass
 
-AudioTrackOutputTypeDef = TypedDict(
-    "AudioTrackOutputTypeDef",
-    {
-        "Track": int,
-    },
-)
 
 AudioTrackTypeDef = TypedDict(
     "AudioTrackTypeDef",
     {
         "Track": int,
     },
 )
 
-_RequiredInputLocationTypeDef = TypedDict(
-    "_RequiredInputLocationTypeDef",
-    {
-        "Uri": str,
-    },
-)
-_OptionalInputLocationTypeDef = TypedDict(
-    "_OptionalInputLocationTypeDef",
-    {
-        "PasswordParam": str,
-        "Username": str,
-    },
-    total=False,
-)
-
-class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
-    pass
-
-_RequiredEsamOutputTypeDef = TypedDict(
-    "_RequiredEsamOutputTypeDef",
-    {
-        "AcquisitionPointId": str,
-        "PoisEndpoint": str,
-    },
-)
-_OptionalEsamOutputTypeDef = TypedDict(
-    "_OptionalEsamOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "PasswordParam": str,
-        "Username": str,
-        "ZoneIdentity": str,
-    },
-    total=False,
-)
-
-class EsamOutputTypeDef(_RequiredEsamOutputTypeDef, _OptionalEsamOutputTypeDef):
-    pass
-
-Scte35SpliceInsertOutputTypeDef = TypedDict(
-    "Scte35SpliceInsertOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "NoRegionalBlackoutFlag": Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
-        "WebDeliveryAllowedFlag": Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
-    },
-    total=False,
-)
-
-Scte35TimeSignalAposOutputTypeDef = TypedDict(
-    "Scte35TimeSignalAposOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "NoRegionalBlackoutFlag": Scte35AposNoRegionalBlackoutBehaviorType,
-        "WebDeliveryAllowedFlag": Scte35AposWebDeliveryAllowedBehaviorType,
-    },
-    total=False,
-)
-
 _RequiredEsamTypeDef = TypedDict(
     "_RequiredEsamTypeDef",
     {
         "AcquisitionPointId": str,
         "PoisEndpoint": str,
     },
 )
@@ -1310,17 +934,19 @@
         "PasswordParam": str,
         "Username": str,
         "ZoneIdentity": str,
     },
     total=False,
 )
 
+
 class EsamTypeDef(_RequiredEsamTypeDef, _OptionalEsamTypeDef):
     pass
 
+
 Scte35SpliceInsertTypeDef = TypedDict(
     "Scte35SpliceInsertTypeDef",
     {
         "AdAvailOffset": int,
         "NoRegionalBlackoutFlag": Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
         "WebDeliveryAllowedFlag": Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
     },
@@ -1365,14 +991,25 @@
         "Arn": str,
         "Id": str,
         "State": str,
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
 BatchScheduleActionDeleteRequestTypeDef = TypedDict(
     "BatchScheduleActionDeleteRequestTypeDef",
     {
         "ActionNames": Sequence[str],
     },
 )
 
@@ -1397,41 +1034,14 @@
 CancelInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "CancelInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
-EbuTtDDestinationSettingsOutputTypeDef = TypedDict(
-    "EbuTtDDestinationSettingsOutputTypeDef",
-    {
-        "CopyrightHolder": str,
-        "FillLineGap": EbuTtDFillLineGapControlType,
-        "FontFamily": str,
-        "StyleControl": EbuTtDDestinationStyleControlType,
-    },
-    total=False,
-)
-
-TtmlDestinationSettingsOutputTypeDef = TypedDict(
-    "TtmlDestinationSettingsOutputTypeDef",
-    {
-        "StyleControl": TtmlDestinationStyleControlType,
-    },
-    total=False,
-)
-
-WebvttDestinationSettingsOutputTypeDef = TypedDict(
-    "WebvttDestinationSettingsOutputTypeDef",
-    {
-        "StyleControl": WebvttDestinationStyleControlType,
-    },
-    total=False,
-)
-
 EbuTtDDestinationSettingsTypeDef = TypedDict(
     "EbuTtDDestinationSettingsTypeDef",
     {
         "CopyrightHolder": str,
         "FillLineGap": EbuTtDFillLineGapControlType,
         "FontFamily": str,
         "StyleControl": EbuTtDDestinationStyleControlType,
@@ -1451,90 +1061,33 @@
     "WebvttDestinationSettingsTypeDef",
     {
         "StyleControl": WebvttDestinationStyleControlType,
     },
     total=False,
 )
 
-CaptionLanguageMappingOutputTypeDef = TypedDict(
-    "CaptionLanguageMappingOutputTypeDef",
-    {
-        "CaptionChannel": int,
-        "LanguageCode": str,
-        "LanguageDescription": str,
-    },
-)
-
 CaptionLanguageMappingTypeDef = TypedDict(
     "CaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "LanguageCode": str,
         "LanguageDescription": str,
     },
 )
 
-CaptionRectangleOutputTypeDef = TypedDict(
-    "CaptionRectangleOutputTypeDef",
-    {
-        "Height": float,
-        "LeftOffset": float,
-        "TopOffset": float,
-        "Width": float,
-    },
-)
-
 CaptionRectangleTypeDef = TypedDict(
     "CaptionRectangleTypeDef",
     {
         "Height": float,
         "LeftOffset": float,
         "TopOffset": float,
         "Width": float,
     },
 )
 
-DvbSubSourceSettingsOutputTypeDef = TypedDict(
-    "DvbSubSourceSettingsOutputTypeDef",
-    {
-        "OcrLanguage": DvbSubOcrLanguageType,
-        "Pid": int,
-    },
-    total=False,
-)
-
-EmbeddedSourceSettingsOutputTypeDef = TypedDict(
-    "EmbeddedSourceSettingsOutputTypeDef",
-    {
-        "Convert608To708": EmbeddedConvert608To708Type,
-        "Scte20Detection": EmbeddedScte20DetectionType,
-        "Source608ChannelNumber": int,
-        "Source608TrackNumber": int,
-    },
-    total=False,
-)
-
-Scte20SourceSettingsOutputTypeDef = TypedDict(
-    "Scte20SourceSettingsOutputTypeDef",
-    {
-        "Convert608To708": Scte20Convert608To708Type,
-        "Source608ChannelNumber": int,
-    },
-    total=False,
-)
-
-Scte27SourceSettingsOutputTypeDef = TypedDict(
-    "Scte27SourceSettingsOutputTypeDef",
-    {
-        "OcrLanguage": Scte27OcrLanguageType,
-        "Pid": int,
-    },
-    total=False,
-)
-
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "OcrLanguage": DvbSubOcrLanguageType,
         "Pid": int,
     },
     total=False,
@@ -1565,22 +1118,14 @@
     {
         "OcrLanguage": Scte27OcrLanguageType,
         "Pid": int,
     },
     total=False,
 )
 
-CdiInputSpecificationOutputTypeDef = TypedDict(
-    "CdiInputSpecificationOutputTypeDef",
-    {
-        "Resolution": CdiInputResolutionType,
-    },
-    total=False,
-)
-
 CdiInputSpecificationTypeDef = TypedDict(
     "CdiInputSpecificationTypeDef",
     {
         "Resolution": CdiInputResolutionType,
     },
     total=False,
 )
@@ -1589,16 +1134,16 @@
     "ChannelEgressEndpointTypeDef",
     {
         "SourceIp": str,
     },
     total=False,
 )
 
-InputSpecificationOutputTypeDef = TypedDict(
-    "InputSpecificationOutputTypeDef",
+InputSpecificationTypeDef = TypedDict(
+    "InputSpecificationTypeDef",
     {
         "Codec": InputCodecType,
         "MaximumBitrate": InputMaximumBitrateType,
         "Resolution": InputResolutionType,
     },
     total=False,
 )
@@ -1641,24 +1186,14 @@
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-InputSpecificationTypeDef = TypedDict(
-    "InputSpecificationTypeDef",
-    {
-        "Codec": InputCodecType,
-        "MaximumBitrate": InputMaximumBitrateType,
-        "Resolution": InputResolutionType,
-    },
-    total=False,
-)
-
 MaintenanceCreateSettingsTypeDef = TypedDict(
     "MaintenanceCreateSettingsTypeDef",
     {
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceStartTime": str,
     },
     total=False,
@@ -1675,19 +1210,21 @@
     {
         "PublicAddressAllocationIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcOutputSettingsTypeDef(
     _RequiredVpcOutputSettingsTypeDef, _OptionalVpcOutputSettingsTypeDef
 ):
     pass
 
+
 InputDestinationRequestTypeDef = TypedDict(
     "InputDestinationRequestTypeDef",
     {
         "StreamName": str,
     },
     total=False,
 )
@@ -1720,17 +1257,19 @@
     "_OptionalInputVpcRequestTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class InputVpcRequestTypeDef(_RequiredInputVpcRequestTypeDef, _OptionalInputVpcRequestTypeDef):
     pass
 
+
 MediaConnectFlowRequestTypeDef = TypedDict(
     "MediaConnectFlowRequestTypeDef",
     {
         "FlowArn": str,
     },
     total=False,
 )
@@ -1755,19 +1294,21 @@
     {
         "MaximumVideoBufferDelayMilliseconds": int,
         "TransportStreamReservedBitrate": int,
     },
     total=False,
 )
 
+
 class MultiplexSettingsTypeDef(
     _RequiredMultiplexSettingsTypeDef, _OptionalMultiplexSettingsTypeDef
 ):
     pass
 
+
 _RequiredCreatePartnerInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartnerInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalCreatePartnerInputRequestRequestTypeDef = TypedDict(
@@ -1775,39 +1316,43 @@
     {
         "RequestId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePartnerInputRequestRequestTypeDef(
     _RequiredCreatePartnerInputRequestRequestTypeDef,
     _OptionalCreatePartnerInputRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateTagsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalCreateTagsRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTagsRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateTagsRequestRequestTypeDef(
     _RequiredCreateTagsRequestRequestTypeDef, _OptionalCreateTagsRequestRequestTypeDef
 ):
     pass
 
+
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 
@@ -1865,44 +1410,23 @@
 DeleteMultiplexRequestRequestTypeDef = TypedDict(
     "DeleteMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 
-_RequiredMultiplexSettingsOutputTypeDef = TypedDict(
-    "_RequiredMultiplexSettingsOutputTypeDef",
-    {
-        "TransportStreamBitrate": int,
-        "TransportStreamId": int,
-    },
-)
-_OptionalMultiplexSettingsOutputTypeDef = TypedDict(
-    "_OptionalMultiplexSettingsOutputTypeDef",
-    {
-        "MaximumVideoBufferDelayMilliseconds": int,
-        "TransportStreamReservedBitrate": int,
-    },
-    total=False,
-)
-
-class MultiplexSettingsOutputTypeDef(
-    _RequiredMultiplexSettingsOutputTypeDef, _OptionalMultiplexSettingsOutputTypeDef
-):
-    pass
-
 DeleteReservationRequestRequestTypeDef = TypedDict(
     "DeleteReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-RenewalSettingsOutputTypeDef = TypedDict(
-    "RenewalSettingsOutputTypeDef",
+RenewalSettingsTypeDef = TypedDict(
+    "RenewalSettingsTypeDef",
     {
         "AutomaticRenewal": ReservationAutomaticRenewalType,
         "RenewalCount": int,
     },
     total=False,
 )
 
@@ -2007,41 +1531,21 @@
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
     {
         "InputDeviceId": str,
         "Accept": Literal["image/jpeg"],
     },
 )
 
-DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ContentType": Literal["image/jpeg"],
-        "ContentLength": int,
-        "ETag": str,
-        "LastModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 
-InputDeviceSettingsOutputTypeDef = TypedDict(
-    "InputDeviceSettingsOutputTypeDef",
-    {
-        "Id": str,
-    },
-    total=False,
-)
-
 InputSourceTypeDef = TypedDict(
     "InputSourceTypeDef",
     {
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
@@ -2096,34 +1600,24 @@
 DescribeReservationRequestRequestTypeDef = TypedDict(
     "DescribeReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "ChannelId": str,
-    },
-)
-_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
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
 
-class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
-    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeScheduleRequestRequestTypeDef = TypedDict(
@@ -2131,117 +1625,69 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScheduleRequestRequestTypeDef(
     _RequiredDescribeScheduleRequestRequestTypeDef, _OptionalDescribeScheduleRequestRequestTypeDef
 ):
     pass
 
+
 DescribeThumbnailsRequestRequestTypeDef = TypedDict(
     "DescribeThumbnailsRequestRequestTypeDef",
     {
         "ChannelId": str,
         "PipelineId": str,
         "ThumbnailType": str,
     },
 )
 
-_RequiredDvbNitSettingsOutputTypeDef = TypedDict(
-    "_RequiredDvbNitSettingsOutputTypeDef",
+_RequiredDvbNitSettingsTypeDef = TypedDict(
+    "_RequiredDvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
     },
 )
-_OptionalDvbNitSettingsOutputTypeDef = TypedDict(
-    "_OptionalDvbNitSettingsOutputTypeDef",
+_OptionalDvbNitSettingsTypeDef = TypedDict(
+    "_OptionalDvbNitSettingsTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
-class DvbNitSettingsOutputTypeDef(
-    _RequiredDvbNitSettingsOutputTypeDef, _OptionalDvbNitSettingsOutputTypeDef
-):
+
+class DvbNitSettingsTypeDef(_RequiredDvbNitSettingsTypeDef, _OptionalDvbNitSettingsTypeDef):
     pass
 
-DvbSdtSettingsOutputTypeDef = TypedDict(
-    "DvbSdtSettingsOutputTypeDef",
+
+DvbSdtSettingsTypeDef = TypedDict(
+    "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": DvbSdtOutputSdtType,
         "RepInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
-DvbTdtSettingsOutputTypeDef = TypedDict(
-    "DvbTdtSettingsOutputTypeDef",
+DvbTdtSettingsTypeDef = TypedDict(
+    "DvbTdtSettingsTypeDef",
     {
         "RepInterval": int,
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
-FeatureActivationsOutputTypeDef = TypedDict(
-    "FeatureActivationsOutputTypeDef",
-    {
-        "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
-    },
-    total=False,
-)
-
-NielsenConfigurationOutputTypeDef = TypedDict(
-    "NielsenConfigurationOutputTypeDef",
-    {
-        "DistributorId": str,
-        "NielsenPcmToId3Tagging": NielsenPcmToId3TaggingStateType,
-    },
-    total=False,
-)
-
-ThumbnailConfigurationOutputTypeDef = TypedDict(
-    "ThumbnailConfigurationOutputTypeDef",
-    {
-        "State": ThumbnailStateType,
-    },
-)
-
-_RequiredTimecodeConfigOutputTypeDef = TypedDict(
-    "_RequiredTimecodeConfigOutputTypeDef",
-    {
-        "Source": TimecodeConfigSourceType,
-    },
-)
-_OptionalTimecodeConfigOutputTypeDef = TypedDict(
-    "_OptionalTimecodeConfigOutputTypeDef",
-    {
-        "SyncThreshold": int,
-    },
-    total=False,
-)
-
-class TimecodeConfigOutputTypeDef(
-    _RequiredTimecodeConfigOutputTypeDef, _OptionalTimecodeConfigOutputTypeDef
-):
-    pass
-
 FeatureActivationsTypeDef = TypedDict(
     "FeatureActivationsTypeDef",
     {
         "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
     },
     total=False,
 )
@@ -2272,33 +1718,18 @@
     "_OptionalTimecodeConfigTypeDef",
     {
         "SyncThreshold": int,
     },
     total=False,
 )
 
+
 class TimecodeConfigTypeDef(_RequiredTimecodeConfigTypeDef, _OptionalTimecodeConfigTypeDef):
     pass
 
-InputLossFailoverSettingsOutputTypeDef = TypedDict(
-    "InputLossFailoverSettingsOutputTypeDef",
-    {
-        "InputLossThresholdMsec": int,
-    },
-    total=False,
-)
-
-VideoBlackFailoverSettingsOutputTypeDef = TypedDict(
-    "VideoBlackFailoverSettingsOutputTypeDef",
-    {
-        "BlackDetectThreshold": float,
-        "VideoBlackThresholdMsec": int,
-    },
-    total=False,
-)
 
 InputLossFailoverSettingsTypeDef = TypedDict(
     "InputLossFailoverSettingsTypeDef",
     {
         "InputLossThresholdMsec": int,
     },
     total=False,
@@ -2309,108 +1740,65 @@
     {
         "BlackDetectThreshold": float,
         "VideoBlackThresholdMsec": int,
     },
     total=False,
 )
 
-FecOutputSettingsOutputTypeDef = TypedDict(
-    "FecOutputSettingsOutputTypeDef",
+FecOutputSettingsTypeDef = TypedDict(
+    "FecOutputSettingsTypeDef",
     {
         "ColumnDepth": int,
         "IncludeFec": FecOutputIncludeFecType,
         "RowLength": int,
     },
     total=False,
 )
 
-FixedModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
-    "FixedModeScheduleActionStartSettingsOutputTypeDef",
-    {
-        "Time": str,
-    },
-)
-
 FixedModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FixedModeScheduleActionStartSettingsTypeDef",
     {
         "Time": str,
     },
 )
 
-Fmp4HlsSettingsOutputTypeDef = TypedDict(
-    "Fmp4HlsSettingsOutputTypeDef",
+Fmp4HlsSettingsTypeDef = TypedDict(
+    "Fmp4HlsSettingsTypeDef",
     {
         "AudioRenditionSets": str,
         "NielsenId3Behavior": Fmp4NielsenId3BehaviorType,
         "TimedMetadataBehavior": Fmp4TimedMetadataBehaviorType,
     },
     total=False,
 )
 
-FollowModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
-    "FollowModeScheduleActionStartSettingsOutputTypeDef",
-    {
-        "FollowPoint": FollowPointType,
-        "ReferenceActionName": str,
-    },
-)
-
 FollowModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FollowModeScheduleActionStartSettingsTypeDef",
     {
         "FollowPoint": FollowPointType,
         "ReferenceActionName": str,
     },
 )
 
-FrameCaptureS3SettingsOutputTypeDef = TypedDict(
-    "FrameCaptureS3SettingsOutputTypeDef",
-    {
-        "CannedAcl": S3CannedAclType,
-    },
-    total=False,
-)
-
 FrameCaptureS3SettingsTypeDef = TypedDict(
     "FrameCaptureS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
-FrameCaptureOutputSettingsOutputTypeDef = TypedDict(
-    "FrameCaptureOutputSettingsOutputTypeDef",
+FrameCaptureOutputSettingsTypeDef = TypedDict(
+    "FrameCaptureOutputSettingsTypeDef",
     {
         "NameModifier": str,
     },
     total=False,
 )
 
-_RequiredTimecodeBurninSettingsOutputTypeDef = TypedDict(
-    "_RequiredTimecodeBurninSettingsOutputTypeDef",
-    {
-        "FontSize": TimecodeBurninFontSizeType,
-        "Position": TimecodeBurninPositionType,
-    },
-)
-_OptionalTimecodeBurninSettingsOutputTypeDef = TypedDict(
-    "_OptionalTimecodeBurninSettingsOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-class TimecodeBurninSettingsOutputTypeDef(
-    _RequiredTimecodeBurninSettingsOutputTypeDef, _OptionalTimecodeBurninSettingsOutputTypeDef
-):
-    pass
-
 _RequiredTimecodeBurninSettingsTypeDef = TypedDict(
     "_RequiredTimecodeBurninSettingsTypeDef",
     {
         "FontSize": TimecodeBurninFontSizeType,
         "Position": TimecodeBurninPositionType,
     },
 )
@@ -2418,19 +1806,21 @@
     "_OptionalTimecodeBurninSettingsTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
+
 class TimecodeBurninSettingsTypeDef(
     _RequiredTimecodeBurninSettingsTypeDef, _OptionalTimecodeBurninSettingsTypeDef
 ):
     pass
 
+
 H264ColorSpaceSettingsOutputTypeDef = TypedDict(
     "H264ColorSpaceSettingsOutputTypeDef",
     {
         "ColorSpacePassthroughSettings": Dict[str, Any],
         "Rec601Settings": Dict[str, Any],
         "Rec709Settings": Dict[str, Any],
     },
@@ -2443,132 +1833,57 @@
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "Rec601Settings": Mapping[str, Any],
         "Rec709Settings": Mapping[str, Any],
     },
     total=False,
 )
 
-TemporalFilterSettingsOutputTypeDef = TypedDict(
-    "TemporalFilterSettingsOutputTypeDef",
-    {
-        "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
-        "Strength": TemporalFilterStrengthType,
-    },
-    total=False,
-)
-
 TemporalFilterSettingsTypeDef = TypedDict(
     "TemporalFilterSettingsTypeDef",
     {
         "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
         "Strength": TemporalFilterStrengthType,
     },
     total=False,
 )
 
-Hdr10SettingsOutputTypeDef = TypedDict(
-    "Hdr10SettingsOutputTypeDef",
-    {
-        "MaxCll": int,
-        "MaxFall": int,
-    },
-    total=False,
-)
-
 Hdr10SettingsTypeDef = TypedDict(
     "Hdr10SettingsTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
-HlsAkamaiSettingsOutputTypeDef = TypedDict(
-    "HlsAkamaiSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "HttpTransferMode": HlsAkamaiHttpTransferModeType,
-        "NumRetries": int,
-        "RestartDelay": int,
-        "Salt": str,
-        "Token": str,
-    },
-    total=False,
-)
-
 HlsAkamaiSettingsTypeDef = TypedDict(
     "HlsAkamaiSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "HttpTransferMode": HlsAkamaiHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
         "Salt": str,
         "Token": str,
     },
     total=False,
 )
 
-HlsBasicPutSettingsOutputTypeDef = TypedDict(
-    "HlsBasicPutSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "NumRetries": int,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
 HlsBasicPutSettingsTypeDef = TypedDict(
     "HlsBasicPutSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
-HlsMediaStoreSettingsOutputTypeDef = TypedDict(
-    "HlsMediaStoreSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "MediaStoreStorageClass": Literal["TEMPORAL"],
-        "NumRetries": int,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
-HlsS3SettingsOutputTypeDef = TypedDict(
-    "HlsS3SettingsOutputTypeDef",
-    {
-        "CannedAcl": S3CannedAclType,
-    },
-    total=False,
-)
-
-HlsWebdavSettingsOutputTypeDef = TypedDict(
-    "HlsWebdavSettingsOutputTypeDef",
-    {
-        "ConnectionRetryInterval": int,
-        "FilecacheDuration": int,
-        "HttpTransferMode": HlsWebdavHttpTransferModeType,
-        "NumRetries": int,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
 HlsMediaStoreSettingsTypeDef = TypedDict(
     "HlsMediaStoreSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "MediaStoreStorageClass": Literal["TEMPORAL"],
         "NumRetries": int,
@@ -2593,87 +1908,42 @@
         "HttpTransferMode": HlsWebdavHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
-HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef = TypedDict(
-    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
-    {
-        "Tag": str,
-        "Id3": str,
-    },
-    total=False,
-)
-
 HlsId3SegmentTaggingScheduleActionSettingsTypeDef = TypedDict(
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
     {
         "Tag": str,
         "Id3": str,
     },
     total=False,
 )
 
-HlsInputSettingsOutputTypeDef = TypedDict(
-    "HlsInputSettingsOutputTypeDef",
-    {
-        "Bandwidth": int,
-        "BufferSegments": int,
-        "Retries": int,
-        "RetryInterval": int,
-        "Scte35Source": HlsScte35SourceTypeType,
-    },
-    total=False,
-)
-
 HlsInputSettingsTypeDef = TypedDict(
     "HlsInputSettingsTypeDef",
     {
         "Bandwidth": int,
         "BufferSegments": int,
         "Retries": int,
         "RetryInterval": int,
         "Scte35Source": HlsScte35SourceTypeType,
     },
     total=False,
 )
 
-HlsTimedMetadataScheduleActionSettingsOutputTypeDef = TypedDict(
-    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
-    {
-        "Id3": str,
-    },
-)
-
 HlsTimedMetadataScheduleActionSettingsTypeDef = TypedDict(
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
     {
         "Id3": str,
     },
 )
 
-StartTimecodeOutputTypeDef = TypedDict(
-    "StartTimecodeOutputTypeDef",
-    {
-        "Timecode": str,
-    },
-    total=False,
-)
-
-StopTimecodeOutputTypeDef = TypedDict(
-    "StopTimecodeOutputTypeDef",
-    {
-        "LastFrameClippingBehavior": LastFrameClippingBehaviorType,
-        "Timecode": str,
-    },
-    total=False,
-)
-
 StartTimecodeTypeDef = TypedDict(
     "StartTimecodeTypeDef",
     {
         "Timecode": str,
     },
     total=False,
 )
@@ -2710,51 +1980,23 @@
     "InputDeviceRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "TransferType": str,
-    },
-)
-_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
-    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-):
-    pass
-
 _RequiredListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "_RequiredListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
     },
 )
 _OptionalListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
@@ -2762,102 +2004,60 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListInputDeviceTransfersRequestRequestTypeDef(
     _RequiredListInputDeviceTransfersRequestRequestTypeDef,
     _OptionalListInputDeviceTransfersRequestRequestTypeDef,
 ):
     pass
 
+
 TransferringInputDeviceSummaryTypeDef = TypedDict(
     "TransferringInputDeviceSummaryTypeDef",
     {
         "Id": str,
         "Message": str,
         "TargetCustomerId": str,
         "TransferType": InputDeviceTransferTypeType,
     },
     total=False,
 )
 
-ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInputDevicesRequestRequestTypeDef = TypedDict(
     "ListInputDevicesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInputSecurityGroupsRequestRequestTypeDef = TypedDict(
     "ListInputSecurityGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListInputsRequestListInputsPaginateTypeDef = TypedDict(
-    "ListInputsRequestListInputsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInputsRequestRequestTypeDef = TypedDict(
     "ListInputsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "MultiplexId": str,
-    },
-)
-_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
-    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMultiplexProgramsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiplexProgramsRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalListMultiplexProgramsRequestRequestTypeDef = TypedDict(
@@ -2865,64 +2065,40 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListMultiplexProgramsRequestRequestTypeDef(
     _RequiredListMultiplexProgramsRequestRequestTypeDef,
     _OptionalListMultiplexProgramsRequestRequestTypeDef,
 ):
     pass
 
+
 MultiplexProgramSummaryTypeDef = TypedDict(
     "MultiplexProgramSummaryTypeDef",
     {
         "ChannelId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
-ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMultiplexesRequestRequestTypeDef = TypedDict(
     "ListMultiplexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "ChannelConfiguration": str,
-        "Codec": str,
-        "Duration": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "ChannelConfiguration": str,
         "Codec": str,
         "Duration": str,
@@ -2934,30 +2110,14 @@
         "ResourceType": str,
         "SpecialFeature": str,
         "VideoQuality": str,
     },
     total=False,
 )
 
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "Codec": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "Codec": str,
         "MaxResults": int,
         "MaximumBitrate": str,
@@ -2974,24 +2134,16 @@
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
-M3u8SettingsOutputTypeDef = TypedDict(
-    "M3u8SettingsOutputTypeDef",
+M3u8SettingsTypeDef = TypedDict(
+    "M3u8SettingsTypeDef",
     {
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "EcmPid": str,
         "NielsenId3Behavior": M3u8NielsenId3BehaviorType,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
@@ -3016,41 +2168,22 @@
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceScheduledDate": str,
         "MaintenanceStartTime": str,
     },
     total=False,
 )
 
-MediaPackageOutputDestinationSettingsOutputTypeDef = TypedDict(
-    "MediaPackageOutputDestinationSettingsOutputTypeDef",
-    {
-        "ChannelId": str,
-    },
-    total=False,
-)
-
 MediaPackageOutputDestinationSettingsTypeDef = TypedDict(
     "MediaPackageOutputDestinationSettingsTypeDef",
     {
         "ChannelId": str,
     },
     total=False,
 )
 
-MotionGraphicsActivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
-    {
-        "Duration": int,
-        "PasswordParam": str,
-        "Url": str,
-        "Username": str,
-    },
-    total=False,
-)
-
 MotionGraphicsActivateScheduleActionSettingsTypeDef = TypedDict(
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     {
         "Duration": int,
         "PasswordParam": str,
         "Url": str,
         "Username": str,
@@ -3070,16 +2203,16 @@
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-MsSmoothOutputSettingsOutputTypeDef = TypedDict(
-    "MsSmoothOutputSettingsOutputTypeDef",
+MsSmoothOutputSettingsTypeDef = TypedDict(
+    "MsSmoothOutputSettingsTypeDef",
     {
         "H265PackagingType": MsSmoothH265PackagingTypeType,
         "NameModifier": str,
     },
     total=False,
 )
 
@@ -3087,40 +2220,23 @@
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     {
         "EntitlementArn": str,
     },
     total=False,
 )
 
-MultiplexProgramChannelDestinationSettingsOutputTypeDef = TypedDict(
-    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
-    {
-        "MultiplexId": str,
-        "ProgramName": str,
-    },
-    total=False,
-)
-
 MultiplexProgramChannelDestinationSettingsTypeDef = TypedDict(
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
-MultiplexProgramServiceDescriptorOutputTypeDef = TypedDict(
-    "MultiplexProgramServiceDescriptorOutputTypeDef",
-    {
-        "ProviderName": str,
-        "ServiceName": str,
-    },
-)
-
 MultiplexProgramServiceDescriptorTypeDef = TypedDict(
     "MultiplexProgramServiceDescriptorTypeDef",
     {
         "ProviderName": str,
         "ServiceName": str,
     },
 )
@@ -3129,72 +2245,33 @@
     "MultiplexSettingsSummaryTypeDef",
     {
         "TransportStreamBitrate": int,
     },
     total=False,
 )
 
-MultiplexStatmuxVideoSettingsOutputTypeDef = TypedDict(
-    "MultiplexStatmuxVideoSettingsOutputTypeDef",
-    {
-        "MaximumBitrate": int,
-        "MinimumBitrate": int,
-        "Priority": int,
-    },
-    total=False,
-)
-
 MultiplexStatmuxVideoSettingsTypeDef = TypedDict(
     "MultiplexStatmuxVideoSettingsTypeDef",
     {
         "MaximumBitrate": int,
         "MinimumBitrate": int,
         "Priority": int,
     },
     total=False,
 )
 
-NielsenCBETOutputTypeDef = TypedDict(
-    "NielsenCBETOutputTypeDef",
-    {
-        "CbetCheckDigitString": str,
-        "CbetStepaside": NielsenWatermarksCbetStepasideType,
-        "Csid": str,
-    },
-)
-
 NielsenCBETTypeDef = TypedDict(
     "NielsenCBETTypeDef",
     {
         "CbetCheckDigitString": str,
         "CbetStepaside": NielsenWatermarksCbetStepasideType,
         "Csid": str,
     },
 )
 
-_RequiredNielsenNaesIiNwOutputTypeDef = TypedDict(
-    "_RequiredNielsenNaesIiNwOutputTypeDef",
-    {
-        "CheckDigitString": str,
-        "Sid": float,
-    },
-)
-_OptionalNielsenNaesIiNwOutputTypeDef = TypedDict(
-    "_OptionalNielsenNaesIiNwOutputTypeDef",
-    {
-        "Timezone": NielsenWatermarkTimezonesType,
-    },
-    total=False,
-)
-
-class NielsenNaesIiNwOutputTypeDef(
-    _RequiredNielsenNaesIiNwOutputTypeDef, _OptionalNielsenNaesIiNwOutputTypeDef
-):
-    pass
-
 _RequiredNielsenNaesIiNwTypeDef = TypedDict(
     "_RequiredNielsenNaesIiNwTypeDef",
     {
         "CheckDigitString": str,
         "Sid": float,
     },
 )
@@ -3202,27 +2279,18 @@
     "_OptionalNielsenNaesIiNwTypeDef",
     {
         "Timezone": NielsenWatermarkTimezonesType,
     },
     total=False,
 )
 
+
 class NielsenNaesIiNwTypeDef(_RequiredNielsenNaesIiNwTypeDef, _OptionalNielsenNaesIiNwTypeDef):
     pass
 
-OutputDestinationSettingsOutputTypeDef = TypedDict(
-    "OutputDestinationSettingsOutputTypeDef",
-    {
-        "PasswordParam": str,
-        "StreamName": str,
-        "Url": str,
-        "Username": str,
-    },
-    total=False,
-)
 
 OutputDestinationSettingsTypeDef = TypedDict(
     "OutputDestinationSettingsTypeDef",
     {
         "PasswordParam": str,
         "StreamName": str,
         "Url": str,
@@ -3241,16 +2309,16 @@
         "CaptionData": RtmpCaptionDataType,
         "InputLossAction": InputLossActionForRtmpOutType,
         "RestartDelay": int,
     },
     total=False,
 )
 
-UdpGroupSettingsOutputTypeDef = TypedDict(
-    "UdpGroupSettingsOutputTypeDef",
+UdpGroupSettingsTypeDef = TypedDict(
+    "UdpGroupSettingsTypeDef",
     {
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
     },
     total=False,
 )
@@ -3265,170 +2333,71 @@
         "CaptionData": RtmpCaptionDataType,
         "InputLossAction": InputLossActionForRtmpOutType,
         "RestartDelay": int,
     },
     total=False,
 )
 
-UdpGroupSettingsTypeDef = TypedDict(
-    "UdpGroupSettingsTypeDef",
-    {
-        "InputLossAction": InputLossActionForUdpOutType,
-        "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-    },
-    total=False,
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
-PipelinePauseStateSettingsOutputTypeDef = TypedDict(
-    "PipelinePauseStateSettingsOutputTypeDef",
-    {
-        "PipelineId": PipelineIdType,
-    },
-)
-
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
-RenewalSettingsTypeDef = TypedDict(
-    "RenewalSettingsTypeDef",
-    {
-        "AutomaticRenewal": ReservationAutomaticRenewalType,
-        "RenewalCount": int,
-    },
-    total=False,
-)
-
 _RequiredRebootInputDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredRebootInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 _OptionalRebootInputDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalRebootInputDeviceRequestRequestTypeDef",
     {
         "Force": RebootInputDeviceForceType,
     },
     total=False,
 )
 
+
 class RebootInputDeviceRequestRequestTypeDef(
     _RequiredRebootInputDeviceRequestRequestTypeDef, _OptionalRebootInputDeviceRequestRequestTypeDef
 ):
     pass
 
+
 RejectInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "RejectInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
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
-_RequiredScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredScte35InputScheduleActionSettingsOutputTypeDef",
-    {
-        "Mode": Scte35InputModeType,
-    },
-)
-_OptionalScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalScte35InputScheduleActionSettingsOutputTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-    },
-    total=False,
-)
-
-class Scte35InputScheduleActionSettingsOutputTypeDef(
-    _RequiredScte35InputScheduleActionSettingsOutputTypeDef,
-    _OptionalScte35InputScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
-Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef = TypedDict(
-    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
-    {
-        "SpliceEventId": int,
-    },
-)
-
-_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
-    {
-        "SpliceEventId": int,
-    },
-)
-_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
-    {
-        "Duration": int,
-    },
-    total=False,
-)
-
-class Scte35SpliceInsertScheduleActionSettingsOutputTypeDef(
-    _RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-    _OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
-StaticImageDeactivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
-    {
-        "FadeOut": int,
-        "Layer": int,
-    },
-    total=False,
-)
-
 _RequiredScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredScte35InputScheduleActionSettingsTypeDef",
     {
         "Mode": Scte35InputModeType,
     },
 )
 _OptionalScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_OptionalScte35InputScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
     total=False,
 )
 
+
 class Scte35InputScheduleActionSettingsTypeDef(
     _RequiredScte35InputScheduleActionSettingsTypeDef,
     _OptionalScte35InputScheduleActionSettingsTypeDef,
 ):
     pass
 
+
 Scte35ReturnToNetworkScheduleActionSettingsTypeDef = TypedDict(
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     {
         "SpliceEventId": int,
     },
 )
 
@@ -3442,39 +2411,31 @@
     "_OptionalScte35SpliceInsertScheduleActionSettingsTypeDef",
     {
         "Duration": int,
     },
     total=False,
 )
 
+
 class Scte35SpliceInsertScheduleActionSettingsTypeDef(
     _RequiredScte35SpliceInsertScheduleActionSettingsTypeDef,
     _OptionalScte35SpliceInsertScheduleActionSettingsTypeDef,
 ):
     pass
 
+
 StaticImageDeactivateScheduleActionSettingsTypeDef = TypedDict(
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     {
         "FadeOut": int,
         "Layer": int,
     },
     total=False,
 )
 
-Scte35DeliveryRestrictionsOutputTypeDef = TypedDict(
-    "Scte35DeliveryRestrictionsOutputTypeDef",
-    {
-        "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
-        "DeviceRestrictions": Scte35DeviceRestrictionsType,
-        "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
-        "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
-    },
-)
-
 Scte35DeliveryRestrictionsTypeDef = TypedDict(
     "Scte35DeliveryRestrictionsTypeDef",
     {
         "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
         "DeviceRestrictions": Scte35DeviceRestrictionsType,
         "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
         "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
@@ -3539,107 +2500,69 @@
         "TargetCustomerId": str,
         "TargetRegion": str,
         "TransferMessage": str,
     },
     total=False,
 )
 
+
 class TransferInputDeviceRequestRequestTypeDef(
     _RequiredTransferInputDeviceRequestRequestTypeDef,
     _OptionalTransferInputDeviceRequestRequestTypeDef,
 ):
     pass
 
-VideoSelectorPidOutputTypeDef = TypedDict(
-    "VideoSelectorPidOutputTypeDef",
-    {
-        "Pid": int,
-    },
-    total=False,
-)
 
 VideoSelectorPidTypeDef = TypedDict(
     "VideoSelectorPidTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
 
-VideoSelectorProgramIdOutputTypeDef = TypedDict(
-    "VideoSelectorProgramIdOutputTypeDef",
-    {
-        "ProgramId": int,
-    },
-    total=False,
-)
-
 VideoSelectorProgramIdTypeDef = TypedDict(
     "VideoSelectorProgramIdTypeDef",
     {
         "ProgramId": int,
     },
     total=False,
 )
 
-DescribeAccountConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccountConfigurationResponseTypeDef",
-    {
-        "AccountConfiguration": AccountConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
-    {
-        "AccountConfiguration": AccountConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
     },
     total=False,
 )
 
-ArchiveCdnSettingsOutputTypeDef = TypedDict(
-    "ArchiveCdnSettingsOutputTypeDef",
-    {
-        "ArchiveS3Settings": ArchiveS3SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": ArchiveS3SettingsTypeDef,
     },
     total=False,
 )
 
-MediaPackageGroupSettingsOutputTypeDef = TypedDict(
-    "MediaPackageGroupSettingsOutputTypeDef",
+MediaPackageGroupSettingsTypeDef = TypedDict(
+    "MediaPackageGroupSettingsTypeDef",
     {
-        "Destination": OutputLocationRefOutputTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
 
-_RequiredMsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredMsSmoothGroupSettingsOutputTypeDef",
+_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_RequiredMsSmoothGroupSettingsTypeDef",
     {
-        "Destination": OutputLocationRefOutputTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalMsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalMsSmoothGroupSettingsOutputTypeDef",
+_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_OptionalMsSmoothGroupSettingsTypeDef",
     {
         "AcquisitionPointId": str,
         "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
         "CertificateMode": SmoothGroupCertificateModeType,
         "ConnectionRetryInterval": int,
         "EventId": str,
         "EventIdMode": SmoothGroupEventIdModeType,
@@ -3655,94 +2578,55 @@
         "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
         "TimestampOffset": str,
         "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
-class MsSmoothGroupSettingsOutputTypeDef(
-    _RequiredMsSmoothGroupSettingsOutputTypeDef, _OptionalMsSmoothGroupSettingsOutputTypeDef
-):
-    pass
-
-MultiplexOutputSettingsOutputTypeDef = TypedDict(
-    "MultiplexOutputSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
 
-_RequiredRtmpOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredRtmpOutputSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-_OptionalRtmpOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalRtmpOutputSettingsOutputTypeDef",
-    {
-        "CertificateMode": RtmpOutputCertificateModeType,
-        "ConnectionRetryInterval": int,
-        "NumRetries": int,
-    },
-    total=False,
-)
-
-class RtmpOutputSettingsOutputTypeDef(
-    _RequiredRtmpOutputSettingsOutputTypeDef, _OptionalRtmpOutputSettingsOutputTypeDef
+class MsSmoothGroupSettingsTypeDef(
+    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
 ):
     pass
 
-MediaPackageGroupSettingsTypeDef = TypedDict(
-    "MediaPackageGroupSettingsTypeDef",
+
+MultiplexOutputSettingsTypeDef = TypedDict(
+    "MultiplexOutputSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 
-_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_RequiredMsSmoothGroupSettingsTypeDef",
+_RequiredRtmpOutputSettingsTypeDef = TypedDict(
+    "_RequiredRtmpOutputSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_OptionalMsSmoothGroupSettingsTypeDef",
+_OptionalRtmpOutputSettingsTypeDef = TypedDict(
+    "_OptionalRtmpOutputSettingsTypeDef",
     {
-        "AcquisitionPointId": str,
-        "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
-        "CertificateMode": SmoothGroupCertificateModeType,
+        "CertificateMode": RtmpOutputCertificateModeType,
         "ConnectionRetryInterval": int,
-        "EventId": str,
-        "EventIdMode": SmoothGroupEventIdModeType,
-        "EventStopBehavior": SmoothGroupEventStopBehaviorType,
-        "FilecacheDuration": int,
-        "FragmentLength": int,
-        "InputLossAction": InputLossActionForMsSmoothOutType,
         "NumRetries": int,
-        "RestartDelay": int,
-        "SegmentationMode": SmoothGroupSegmentationModeType,
-        "SendDelayMs": int,
-        "SparseTrackType": SmoothGroupSparseTrackTypeType,
-        "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
-        "TimestampOffset": str,
-        "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
-class MsSmoothGroupSettingsTypeDef(
-    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
+
+class RtmpOutputSettingsTypeDef(
+    _RequiredRtmpOutputSettingsTypeDef, _OptionalRtmpOutputSettingsTypeDef
 ):
     pass
 
+
 AudioChannelMappingOutputTypeDef = TypedDict(
     "AudioChannelMappingOutputTypeDef",
     {
-        "InputChannelLevels": List[InputChannelLevelOutputTypeDef],
+        "InputChannelLevels": List[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
 
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
@@ -3750,21 +2634,21 @@
         "OutputChannel": int,
     },
 )
 
 AudioCodecSettingsOutputTypeDef = TypedDict(
     "AudioCodecSettingsOutputTypeDef",
     {
-        "AacSettings": AacSettingsOutputTypeDef,
-        "Ac3Settings": Ac3SettingsOutputTypeDef,
-        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
-        "Eac3Settings": Eac3SettingsOutputTypeDef,
-        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "AacSettings": AacSettingsTypeDef,
+        "Ac3Settings": Ac3SettingsTypeDef,
+        "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
+        "Eac3Settings": Eac3SettingsTypeDef,
+        "Mp2Settings": Mp2SettingsTypeDef,
         "PassThroughSettings": Dict[str, Any],
-        "WavSettings": WavSettingsOutputTypeDef,
+        "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
@@ -3775,53 +2659,53 @@
         "Mp2Settings": Mp2SettingsTypeDef,
         "PassThroughSettings": Mapping[str, Any],
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
-AudioOnlyHlsSettingsOutputTypeDef = TypedDict(
-    "AudioOnlyHlsSettingsOutputTypeDef",
+AudioOnlyHlsSettingsTypeDef = TypedDict(
+    "AudioOnlyHlsSettingsTypeDef",
     {
         "AudioGroupId": str,
-        "AudioOnlyImage": InputLocationOutputTypeDef,
+        "AudioOnlyImage": InputLocationTypeDef,
         "AudioTrackType": AudioOnlyHlsTrackTypeType,
         "SegmentType": AudioOnlyHlsSegmentTypeType,
     },
     total=False,
 )
 
-AvailBlankingOutputTypeDef = TypedDict(
-    "AvailBlankingOutputTypeDef",
+AvailBlankingTypeDef = TypedDict(
+    "AvailBlankingTypeDef",
     {
-        "AvailBlankingImage": InputLocationOutputTypeDef,
+        "AvailBlankingImage": InputLocationTypeDef,
         "State": AvailBlankingStateType,
     },
     total=False,
 )
 
-BlackoutSlateOutputTypeDef = TypedDict(
-    "BlackoutSlateOutputTypeDef",
+BlackoutSlateTypeDef = TypedDict(
+    "BlackoutSlateTypeDef",
     {
-        "BlackoutSlateImage": InputLocationOutputTypeDef,
+        "BlackoutSlateImage": InputLocationTypeDef,
         "NetworkEndBlackout": BlackoutSlateNetworkEndBlackoutType,
-        "NetworkEndBlackoutImage": InputLocationOutputTypeDef,
+        "NetworkEndBlackoutImage": InputLocationTypeDef,
         "NetworkId": str,
         "State": BlackoutSlateStateType,
     },
     total=False,
 )
 
-BurnInDestinationSettingsOutputTypeDef = TypedDict(
-    "BurnInDestinationSettingsOutputTypeDef",
+BurnInDestinationSettingsTypeDef = TypedDict(
+    "BurnInDestinationSettingsTypeDef",
     {
         "Alignment": BurnInAlignmentType,
         "BackgroundColor": BurnInBackgroundColorType,
         "BackgroundOpacity": int,
-        "Font": InputLocationOutputTypeDef,
+        "Font": InputLocationTypeDef,
         "FontColor": BurnInFontColorType,
         "FontOpacity": int,
         "FontResolution": int,
         "FontSize": str,
         "OutlineColor": BurnInOutlineColorType,
         "OutlineSize": int,
         "ShadowColor": BurnInShadowColorType,
@@ -3831,21 +2715,21 @@
         "TeletextGridControl": BurnInTeletextGridControlType,
         "XPosition": int,
         "YPosition": int,
     },
     total=False,
 )
 
-DvbSubDestinationSettingsOutputTypeDef = TypedDict(
-    "DvbSubDestinationSettingsOutputTypeDef",
+DvbSubDestinationSettingsTypeDef = TypedDict(
+    "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubDestinationAlignmentType,
         "BackgroundColor": DvbSubDestinationBackgroundColorType,
         "BackgroundOpacity": int,
-        "Font": InputLocationOutputTypeDef,
+        "Font": InputLocationTypeDef,
         "FontColor": DvbSubDestinationFontColorType,
         "FontOpacity": int,
         "FontResolution": int,
         "FontSize": str,
         "OutlineColor": DvbSubDestinationOutlineColorType,
         "OutlineSize": int,
         "ShadowColor": DvbSubDestinationShadowColorType,
@@ -3855,248 +2739,118 @@
         "TeletextGridControl": DvbSubDestinationTeletextGridControlType,
         "XPosition": int,
         "YPosition": int,
     },
     total=False,
 )
 
-InputLossBehaviorOutputTypeDef = TypedDict(
-    "InputLossBehaviorOutputTypeDef",
+InputLossBehaviorTypeDef = TypedDict(
+    "InputLossBehaviorTypeDef",
     {
         "BlackFrameMsec": int,
         "InputLossImageColor": str,
-        "InputLossImageSlate": InputLocationOutputTypeDef,
+        "InputLossImageSlate": InputLocationTypeDef,
         "InputLossImageType": InputLossImageTypeType,
         "RepeatFrameMsec": int,
     },
     total=False,
 )
 
-_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef",
+_RequiredStaticImageActivateScheduleActionSettingsTypeDef = TypedDict(
+    "_RequiredStaticImageActivateScheduleActionSettingsTypeDef",
     {
-        "Image": InputLocationOutputTypeDef,
+        "Image": InputLocationTypeDef,
     },
 )
-_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef",
+_OptionalStaticImageActivateScheduleActionSettingsTypeDef = TypedDict(
+    "_OptionalStaticImageActivateScheduleActionSettingsTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
         "FadeOut": int,
         "Height": int,
         "ImageX": int,
         "ImageY": int,
         "Layer": int,
         "Opacity": int,
         "Width": int,
     },
     total=False,
 )
 
-class StaticImageActivateScheduleActionSettingsOutputTypeDef(
-    _RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef,
-    _OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef,
+
+class StaticImageActivateScheduleActionSettingsTypeDef(
+    _RequiredStaticImageActivateScheduleActionSettingsTypeDef,
+    _OptionalStaticImageActivateScheduleActionSettingsTypeDef,
 ):
     pass
 
-_RequiredStaticKeySettingsOutputTypeDef = TypedDict(
-    "_RequiredStaticKeySettingsOutputTypeDef",
+
+_RequiredStaticKeySettingsTypeDef = TypedDict(
+    "_RequiredStaticKeySettingsTypeDef",
     {
         "StaticKeyValue": str,
     },
 )
-_OptionalStaticKeySettingsOutputTypeDef = TypedDict(
-    "_OptionalStaticKeySettingsOutputTypeDef",
+_OptionalStaticKeySettingsTypeDef = TypedDict(
+    "_OptionalStaticKeySettingsTypeDef",
     {
-        "KeyProviderServer": InputLocationOutputTypeDef,
+        "KeyProviderServer": InputLocationTypeDef,
     },
     total=False,
 )
 
-class StaticKeySettingsOutputTypeDef(
-    _RequiredStaticKeySettingsOutputTypeDef, _OptionalStaticKeySettingsOutputTypeDef
+
+class StaticKeySettingsTypeDef(
+    _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
 ):
     pass
 
+
 _RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
     "_RequiredAudioTrackSelectionOutputTypeDef",
     {
-        "Tracks": List[AudioTrackOutputTypeDef],
+        "Tracks": List[AudioTrackTypeDef],
     },
 )
 _OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
     "_OptionalAudioTrackSelectionOutputTypeDef",
     {
-        "DolbyEDecode": AudioDolbyEDecodeOutputTypeDef,
+        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
     },
     total=False,
 )
 
+
 class AudioTrackSelectionOutputTypeDef(
     _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
 ):
     pass
 
+
 _RequiredAudioTrackSelectionTypeDef = TypedDict(
     "_RequiredAudioTrackSelectionTypeDef",
     {
         "Tracks": Sequence[AudioTrackTypeDef],
     },
 )
 _OptionalAudioTrackSelectionTypeDef = TypedDict(
     "_OptionalAudioTrackSelectionTypeDef",
     {
         "DolbyEDecode": AudioDolbyEDecodeTypeDef,
     },
     total=False,
 )
 
+
 class AudioTrackSelectionTypeDef(
     _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
 ):
     pass
 
-AvailBlankingTypeDef = TypedDict(
-    "AvailBlankingTypeDef",
-    {
-        "AvailBlankingImage": InputLocationTypeDef,
-        "State": AvailBlankingStateType,
-    },
-    total=False,
-)
-
-BlackoutSlateTypeDef = TypedDict(
-    "BlackoutSlateTypeDef",
-    {
-        "BlackoutSlateImage": InputLocationTypeDef,
-        "NetworkEndBlackout": BlackoutSlateNetworkEndBlackoutType,
-        "NetworkEndBlackoutImage": InputLocationTypeDef,
-        "NetworkId": str,
-        "State": BlackoutSlateStateType,
-    },
-    total=False,
-)
-
-BurnInDestinationSettingsTypeDef = TypedDict(
-    "BurnInDestinationSettingsTypeDef",
-    {
-        "Alignment": BurnInAlignmentType,
-        "BackgroundColor": BurnInBackgroundColorType,
-        "BackgroundOpacity": int,
-        "Font": InputLocationTypeDef,
-        "FontColor": BurnInFontColorType,
-        "FontOpacity": int,
-        "FontResolution": int,
-        "FontSize": str,
-        "OutlineColor": BurnInOutlineColorType,
-        "OutlineSize": int,
-        "ShadowColor": BurnInShadowColorType,
-        "ShadowOpacity": int,
-        "ShadowXOffset": int,
-        "ShadowYOffset": int,
-        "TeletextGridControl": BurnInTeletextGridControlType,
-        "XPosition": int,
-        "YPosition": int,
-    },
-    total=False,
-)
-
-DvbSubDestinationSettingsTypeDef = TypedDict(
-    "DvbSubDestinationSettingsTypeDef",
-    {
-        "Alignment": DvbSubDestinationAlignmentType,
-        "BackgroundColor": DvbSubDestinationBackgroundColorType,
-        "BackgroundOpacity": int,
-        "Font": InputLocationTypeDef,
-        "FontColor": DvbSubDestinationFontColorType,
-        "FontOpacity": int,
-        "FontResolution": int,
-        "FontSize": str,
-        "OutlineColor": DvbSubDestinationOutlineColorType,
-        "OutlineSize": int,
-        "ShadowColor": DvbSubDestinationShadowColorType,
-        "ShadowOpacity": int,
-        "ShadowXOffset": int,
-        "ShadowYOffset": int,
-        "TeletextGridControl": DvbSubDestinationTeletextGridControlType,
-        "XPosition": int,
-        "YPosition": int,
-    },
-    total=False,
-)
-
-InputLossBehaviorTypeDef = TypedDict(
-    "InputLossBehaviorTypeDef",
-    {
-        "BlackFrameMsec": int,
-        "InputLossImageColor": str,
-        "InputLossImageSlate": InputLocationTypeDef,
-        "InputLossImageType": InputLossImageTypeType,
-        "RepeatFrameMsec": int,
-    },
-    total=False,
-)
-
-_RequiredStaticImageActivateScheduleActionSettingsTypeDef = TypedDict(
-    "_RequiredStaticImageActivateScheduleActionSettingsTypeDef",
-    {
-        "Image": InputLocationTypeDef,
-    },
-)
-_OptionalStaticImageActivateScheduleActionSettingsTypeDef = TypedDict(
-    "_OptionalStaticImageActivateScheduleActionSettingsTypeDef",
-    {
-        "Duration": int,
-        "FadeIn": int,
-        "FadeOut": int,
-        "Height": int,
-        "ImageX": int,
-        "ImageY": int,
-        "Layer": int,
-        "Opacity": int,
-        "Width": int,
-    },
-    total=False,
-)
-
-class StaticImageActivateScheduleActionSettingsTypeDef(
-    _RequiredStaticImageActivateScheduleActionSettingsTypeDef,
-    _OptionalStaticImageActivateScheduleActionSettingsTypeDef,
-):
-    pass
-
-_RequiredStaticKeySettingsTypeDef = TypedDict(
-    "_RequiredStaticKeySettingsTypeDef",
-    {
-        "StaticKeyValue": str,
-    },
-)
-_OptionalStaticKeySettingsTypeDef = TypedDict(
-    "_OptionalStaticKeySettingsTypeDef",
-    {
-        "KeyProviderServer": InputLocationTypeDef,
-    },
-    total=False,
-)
-
-class StaticKeySettingsTypeDef(
-    _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
-):
-    pass
-
-AvailSettingsOutputTypeDef = TypedDict(
-    "AvailSettingsOutputTypeDef",
-    {
-        "Esam": EsamOutputTypeDef,
-        "Scte35SpliceInsert": Scte35SpliceInsertOutputTypeDef,
-        "Scte35TimeSignalApos": Scte35TimeSignalAposOutputTypeDef,
-    },
-    total=False,
-)
 
 AvailSettingsTypeDef = TypedDict(
     "AvailSettingsTypeDef",
     {
         "Esam": EsamTypeDef,
         "Scte35SpliceInsert": Scte35SpliceInsertTypeDef,
         "Scte35TimeSignalApos": Scte35TimeSignalAposTypeDef,
@@ -4105,43 +2859,77 @@
 )
 
 BatchDeleteResponseTypeDef = TypedDict(
     "BatchDeleteResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartResponseTypeDef = TypedDict(
     "BatchStartResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStopResponseTypeDef = TypedDict(
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TeletextSourceSettingsOutputTypeDef = TypedDict(
-    "TeletextSourceSettingsOutputTypeDef",
+DescribeAccountConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccountConfigurationResponseTypeDef",
     {
-        "OutputRectangle": CaptionRectangleOutputTypeDef,
-        "PageNumber": str,
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ContentType": Literal["image/jpeg"],
+        "ContentLength": int,
+        "ETag": str,
+        "LastModified": datetime,
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
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
         "PageNumber": str,
@@ -4187,20 +2975,22 @@
     {
         "Tags": Mapping[str, str],
         "WhitelistRules": Sequence[InputWhitelistRuleCidrTypeDef],
     },
     total=False,
 )
 
+
 class UpdateInputSecurityGroupRequestRequestTypeDef(
     _RequiredUpdateInputSecurityGroupRequestRequestTypeDef,
     _OptionalUpdateInputSecurityGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMultiplexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultiplexRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "RequestId": str,
@@ -4210,19 +3000,21 @@
     "_OptionalCreateMultiplexRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateMultiplexRequestRequestTypeDef(
     _RequiredCreateMultiplexRequestRequestTypeDef, _OptionalCreateMultiplexRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateMultiplexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalUpdateMultiplexRequestRequestTypeDef = TypedDict(
@@ -4230,19 +3022,69 @@
     {
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateMultiplexRequestRequestTypeDef(
     _RequiredUpdateMultiplexRequestRequestTypeDef, _OptionalUpdateMultiplexRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_RequiredPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Count": int,
+        "OfferingId": str,
+    },
+)
+_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_OptionalPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+        "RequestId": str,
+        "Start": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class PurchaseOfferingRequestRequestTypeDef(
+    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReservationRequestRequestTypeDef",
+    {
+        "ReservationId": str,
+    },
+)
+_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReservationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateReservationRequestRequestTypeDef(
+    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
+):
+    pass
+
+
 DeleteReservationResponseTypeDef = TypedDict(
     "DeleteReservationResponseTypeDef",
     {
         "Arn": str,
         "Count": int,
         "CurrencyCode": str,
         "Duration": int,
@@ -4250,22 +3092,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsOutputTypeDef,
+        "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Arn": str,
@@ -4275,15 +3117,15 @@
         "FixedPrice": float,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "UsagePrice": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Arn": str,
@@ -4294,22 +3136,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsOutputTypeDef,
+        "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "Arn": str,
@@ -4338,15 +3180,15 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsOutputTypeDef,
+        "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
     },
@@ -4363,220 +3205,242 @@
     "_OptionalDescribeChannelRequestChannelCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeChannelRequestChannelCreatedWaitTypeDef(
     _RequiredDescribeChannelRequestChannelCreatedWaitTypeDef,
     _OptionalDescribeChannelRequestChannelCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeChannelRequestChannelDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeChannelRequestChannelDeletedWaitTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeChannelRequestChannelDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeChannelRequestChannelDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeChannelRequestChannelDeletedWaitTypeDef(
     _RequiredDescribeChannelRequestChannelDeletedWaitTypeDef,
     _OptionalDescribeChannelRequestChannelDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeChannelRequestChannelRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeChannelRequestChannelRunningWaitTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeChannelRequestChannelRunningWaitTypeDef = TypedDict(
     "_OptionalDescribeChannelRequestChannelRunningWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeChannelRequestChannelRunningWaitTypeDef(
     _RequiredDescribeChannelRequestChannelRunningWaitTypeDef,
     _OptionalDescribeChannelRequestChannelRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeChannelRequestChannelStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeChannelRequestChannelStoppedWaitTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeChannelRequestChannelStoppedWaitTypeDef = TypedDict(
     "_OptionalDescribeChannelRequestChannelStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeChannelRequestChannelStoppedWaitTypeDef(
     _RequiredDescribeChannelRequestChannelStoppedWaitTypeDef,
     _OptionalDescribeChannelRequestChannelStoppedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInputRequestInputAttachedWaitTypeDef = TypedDict(
     "_RequiredDescribeInputRequestInputAttachedWaitTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalDescribeInputRequestInputAttachedWaitTypeDef = TypedDict(
     "_OptionalDescribeInputRequestInputAttachedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInputRequestInputAttachedWaitTypeDef(
     _RequiredDescribeInputRequestInputAttachedWaitTypeDef,
     _OptionalDescribeInputRequestInputAttachedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInputRequestInputDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeInputRequestInputDeletedWaitTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalDescribeInputRequestInputDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeInputRequestInputDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInputRequestInputDeletedWaitTypeDef(
     _RequiredDescribeInputRequestInputDeletedWaitTypeDef,
     _OptionalDescribeInputRequestInputDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInputRequestInputDetachedWaitTypeDef = TypedDict(
     "_RequiredDescribeInputRequestInputDetachedWaitTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalDescribeInputRequestInputDetachedWaitTypeDef = TypedDict(
     "_OptionalDescribeInputRequestInputDetachedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInputRequestInputDetachedWaitTypeDef(
     _RequiredDescribeInputRequestInputDetachedWaitTypeDef,
     _OptionalDescribeInputRequestInputDetachedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMultiplexRequestMultiplexCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexCreatedWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexCreatedWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMultiplexRequestMultiplexCreatedWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexCreatedWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMultiplexRequestMultiplexDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexDeletedWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMultiplexRequestMultiplexDeletedWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexDeletedWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMultiplexRequestMultiplexRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexRunningWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMultiplexRequestMultiplexRunningWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMultiplexRequestMultiplexStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalDescribeMultiplexRequestMultiplexStoppedWaitTypeDef = TypedDict(
     "_OptionalDescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMultiplexRequestMultiplexStoppedWaitTypeDef(
     _RequiredDescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     _OptionalDescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
 ):
     pass
 
+
 DescribeInputDeviceResponseTypeDef = TypedDict(
     "DescribeInputDeviceResponseTypeDef",
     {
         "Arn": str,
         "ConnectionState": InputDeviceConnectionStateType,
         "DeviceSettingsSyncState": DeviceSettingsSyncStateType,
         "DeviceUpdateStatus": DeviceUpdateStatusType,
@@ -4585,15 +3449,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
         "Arn": str,
@@ -4625,28 +3489,28 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputSecurityGroupTypeDef = TypedDict(
     "InputSecurityGroupTypeDef",
     {
         "Arn": str,
@@ -4655,32 +3519,172 @@
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
     },
     total=False,
 )
 
-M2tsSettingsOutputTypeDef = TypedDict(
-    "M2tsSettingsOutputTypeDef",
+_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "ChannelId": str,
+    },
+)
+_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
+    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+):
+    pass
+
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "TransferType": str,
+    },
+)
+_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
+    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+):
+    pass
+
+
+ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInputsRequestListInputsPaginateTypeDef = TypedDict(
+    "ListInputsRequestListInputsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "MultiplexId": str,
+    },
+)
+_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
+    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+):
+    pass
+
+
+ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "ChannelConfiguration": str,
+        "Codec": str,
+        "Duration": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "Codec": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+M2tsSettingsTypeDef = TypedDict(
+    "M2tsSettingsTypeDef",
     {
         "AbsentInputAudioBehavior": M2tsAbsentInputAudioBehaviorType,
         "Arib": M2tsAribType,
         "AribCaptionsPid": str,
         "AribCaptionsPidControl": M2tsAribCaptionsPidControlType,
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "AudioStreamType": M2tsAudioStreamTypeType,
         "Bitrate": int,
         "BufferModel": M2tsBufferModelType,
         "CcDescriptor": M2tsCcDescriptorType,
-        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
+        "DvbNitSettings": DvbNitSettingsTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsTypeDef,
         "DvbSubPids": str,
-        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
+        "DvbTdtSettings": DvbTdtSettingsTypeDef,
         "DvbTeletextPid": str,
         "Ebif": M2tsEbifControlType,
         "EbpAudioInterval": M2tsAudioIntervalType,
         "EbpLookaheadMs": int,
         "EbpPlacement": M2tsEbpPlacementType,
         "EcmPid": str,
         "EsRateInPes": M2tsEsRateInPesType,
@@ -4710,39 +3714,29 @@
         "TransportStreamId": int,
         "VideoPid": str,
         "Scte35PrerollPullupMilliseconds": float,
     },
     total=False,
 )
 
-FailoverConditionSettingsOutputTypeDef = TypedDict(
-    "FailoverConditionSettingsOutputTypeDef",
-    {
-        "AudioSilenceSettings": AudioSilenceFailoverSettingsOutputTypeDef,
-        "InputLossSettings": InputLossFailoverSettingsOutputTypeDef,
-        "VideoBlackSettings": VideoBlackFailoverSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": AudioSilenceFailoverSettingsTypeDef,
         "InputLossSettings": InputLossFailoverSettingsTypeDef,
         "VideoBlackSettings": VideoBlackFailoverSettingsTypeDef,
     },
     total=False,
 )
 
 ScheduleActionStartSettingsOutputTypeDef = TypedDict(
     "ScheduleActionStartSettingsOutputTypeDef",
     {
-        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsOutputTypeDef,
-        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsOutputTypeDef,
+        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
+        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Dict[str, Any],
     },
     total=False,
 )
 
 ScheduleActionStartSettingsTypeDef = TypedDict(
     "ScheduleActionStartSettingsTypeDef",
@@ -4750,74 +3744,32 @@
         "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
         "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-FrameCaptureCdnSettingsOutputTypeDef = TypedDict(
-    "FrameCaptureCdnSettingsOutputTypeDef",
-    {
-        "FrameCaptureS3Settings": FrameCaptureS3SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 FrameCaptureCdnSettingsTypeDef = TypedDict(
     "FrameCaptureCdnSettingsTypeDef",
     {
         "FrameCaptureS3Settings": FrameCaptureS3SettingsTypeDef,
     },
     total=False,
 )
 
-FrameCaptureSettingsOutputTypeDef = TypedDict(
-    "FrameCaptureSettingsOutputTypeDef",
-    {
-        "CaptureInterval": int,
-        "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "CaptureInterval": int,
         "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-H264FilterSettingsOutputTypeDef = TypedDict(
-    "H264FilterSettingsOutputTypeDef",
-    {
-        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-H265FilterSettingsOutputTypeDef = TypedDict(
-    "H265FilterSettingsOutputTypeDef",
-    {
-        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-Mpeg2FilterSettingsOutputTypeDef = TypedDict(
-    "Mpeg2FilterSettingsOutputTypeDef",
-    {
-        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 H264FilterSettingsTypeDef = TypedDict(
     "H264FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
@@ -4839,29 +3791,21 @@
 )
 
 H265ColorSpaceSettingsOutputTypeDef = TypedDict(
     "H265ColorSpaceSettingsOutputTypeDef",
     {
         "ColorSpacePassthroughSettings": Dict[str, Any],
         "DolbyVision81Settings": Dict[str, Any],
-        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
+        "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Dict[str, Any],
         "Rec709Settings": Dict[str, Any],
     },
     total=False,
 )
 
-VideoSelectorColorSpaceSettingsOutputTypeDef = TypedDict(
-    "VideoSelectorColorSpaceSettingsOutputTypeDef",
-    {
-        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "DolbyVision81Settings": Mapping[str, Any],
         "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Mapping[str, Any],
@@ -4874,76 +3818,35 @@
     "VideoSelectorColorSpaceSettingsTypeDef",
     {
         "Hdr10Settings": Hdr10SettingsTypeDef,
     },
     total=False,
 )
 
-HlsCdnSettingsOutputTypeDef = TypedDict(
-    "HlsCdnSettingsOutputTypeDef",
-    {
-        "HlsAkamaiSettings": HlsAkamaiSettingsOutputTypeDef,
-        "HlsBasicPutSettings": HlsBasicPutSettingsOutputTypeDef,
-        "HlsMediaStoreSettings": HlsMediaStoreSettingsOutputTypeDef,
-        "HlsS3Settings": HlsS3SettingsOutputTypeDef,
-        "HlsWebdavSettings": HlsWebdavSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 HlsCdnSettingsTypeDef = TypedDict(
     "HlsCdnSettingsTypeDef",
     {
         "HlsAkamaiSettings": HlsAkamaiSettingsTypeDef,
         "HlsBasicPutSettings": HlsBasicPutSettingsTypeDef,
         "HlsMediaStoreSettings": HlsMediaStoreSettingsTypeDef,
         "HlsS3Settings": HlsS3SettingsTypeDef,
         "HlsWebdavSettings": HlsWebdavSettingsTypeDef,
     },
     total=False,
 )
 
-NetworkInputSettingsOutputTypeDef = TypedDict(
-    "NetworkInputSettingsOutputTypeDef",
-    {
-        "HlsInputSettings": HlsInputSettingsOutputTypeDef,
-        "ServerValidation": NetworkInputServerValidationType,
-    },
-    total=False,
-)
-
 NetworkInputSettingsTypeDef = TypedDict(
     "NetworkInputSettingsTypeDef",
     {
         "HlsInputSettings": HlsInputSettingsTypeDef,
         "ServerValidation": NetworkInputServerValidationType,
     },
     total=False,
 )
 
-_RequiredInputClippingSettingsOutputTypeDef = TypedDict(
-    "_RequiredInputClippingSettingsOutputTypeDef",
-    {
-        "InputTimecodeSource": InputTimecodeSourceType,
-    },
-)
-_OptionalInputClippingSettingsOutputTypeDef = TypedDict(
-    "_OptionalInputClippingSettingsOutputTypeDef",
-    {
-        "StartTimecode": StartTimecodeOutputTypeDef,
-        "StopTimecode": StopTimecodeOutputTypeDef,
-    },
-    total=False,
-)
-
-class InputClippingSettingsOutputTypeDef(
-    _RequiredInputClippingSettingsOutputTypeDef, _OptionalInputClippingSettingsOutputTypeDef
-):
-    pass
-
 _RequiredInputClippingSettingsTypeDef = TypedDict(
     "_RequiredInputClippingSettingsTypeDef",
     {
         "InputTimecodeSource": InputTimecodeSourceType,
     },
 )
 _OptionalInputClippingSettingsTypeDef = TypedDict(
@@ -4951,19 +3854,21 @@
     {
         "StartTimecode": StartTimecodeTypeDef,
         "StopTimecode": StopTimecodeTypeDef,
     },
     total=False,
 )
 
+
 class InputClippingSettingsTypeDef(
     _RequiredInputClippingSettingsTypeDef, _OptionalInputClippingSettingsTypeDef
 ):
     pass
 
+
 InputDestinationTypeDef = TypedDict(
     "InputDestinationTypeDef",
     {
         "Ip": str,
         "Port": str,
         "Url": str,
         "Vpc": InputDestinationVpcTypeDef,
@@ -4983,19 +3888,21 @@
         "HdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
         "Name": str,
         "UhdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateInputDeviceRequestRequestTypeDef(
     _RequiredUpdateInputDeviceRequestRequestTypeDef, _OptionalUpdateInputDeviceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalUpdateInputRequestRequestTypeDef = TypedDict(
@@ -5008,95 +3915,103 @@
         "Name": str,
         "RoleArn": str,
         "Sources": Sequence[InputSourceRequestTypeDef],
     },
     total=False,
 )
 
+
 class UpdateInputRequestRequestTypeDef(
     _RequiredUpdateInputRequestRequestTypeDef, _OptionalUpdateInputRequestRequestTypeDef
 ):
     pass
 
+
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStandardHlsSettingsOutputTypeDef = TypedDict(
-    "_RequiredStandardHlsSettingsOutputTypeDef",
+_RequiredStandardHlsSettingsTypeDef = TypedDict(
+    "_RequiredStandardHlsSettingsTypeDef",
     {
-        "M3u8Settings": M3u8SettingsOutputTypeDef,
+        "M3u8Settings": M3u8SettingsTypeDef,
     },
 )
-_OptionalStandardHlsSettingsOutputTypeDef = TypedDict(
-    "_OptionalStandardHlsSettingsOutputTypeDef",
+_OptionalStandardHlsSettingsTypeDef = TypedDict(
+    "_OptionalStandardHlsSettingsTypeDef",
     {
         "AudioRenditionSets": str,
     },
     total=False,
 )
 
-class StandardHlsSettingsOutputTypeDef(
-    _RequiredStandardHlsSettingsOutputTypeDef, _OptionalStandardHlsSettingsOutputTypeDef
+
+class StandardHlsSettingsTypeDef(
+    _RequiredStandardHlsSettingsTypeDef, _OptionalStandardHlsSettingsTypeDef
 ):
     pass
 
+
 _RequiredMotionGraphicsConfigurationOutputTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationOutputTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
     },
 )
 _OptionalMotionGraphicsConfigurationOutputTypeDef = TypedDict(
     "_OptionalMotionGraphicsConfigurationOutputTypeDef",
     {
         "MotionGraphicsInsertion": MotionGraphicsInsertionType,
     },
     total=False,
 )
 
+
 class MotionGraphicsConfigurationOutputTypeDef(
     _RequiredMotionGraphicsConfigurationOutputTypeDef,
     _OptionalMotionGraphicsConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredMotionGraphicsConfigurationTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
     },
 )
 _OptionalMotionGraphicsConfigurationTypeDef = TypedDict(
     "_OptionalMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsInsertion": MotionGraphicsInsertionType,
     },
     total=False,
 )
 
+
 class MotionGraphicsConfigurationTypeDef(
     _RequiredMotionGraphicsConfigurationTypeDef, _OptionalMotionGraphicsConfigurationTypeDef
 ):
     pass
 
+
 MultiplexOutputDestinationTypeDef = TypedDict(
     "MultiplexOutputDestinationTypeDef",
     {
         "MediaConnectSettings": MultiplexMediaConnectOutputDestinationSettingsTypeDef,
     },
     total=False,
 )
@@ -5113,59 +4028,40 @@
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-MultiplexVideoSettingsOutputTypeDef = TypedDict(
-    "MultiplexVideoSettingsOutputTypeDef",
-    {
-        "ConstantBitrate": int,
-        "StatmuxSettings": MultiplexStatmuxVideoSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 MultiplexVideoSettingsTypeDef = TypedDict(
     "MultiplexVideoSettingsTypeDef",
     {
         "ConstantBitrate": int,
         "StatmuxSettings": MultiplexStatmuxVideoSettingsTypeDef,
     },
     total=False,
 )
 
-NielsenWatermarksSettingsOutputTypeDef = TypedDict(
-    "NielsenWatermarksSettingsOutputTypeDef",
-    {
-        "NielsenCbetSettings": NielsenCBETOutputTypeDef,
-        "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
-        "NielsenNaesIiNwSettings": NielsenNaesIiNwOutputTypeDef,
-    },
-    total=False,
-)
-
 NielsenWatermarksSettingsTypeDef = TypedDict(
     "NielsenWatermarksSettingsTypeDef",
     {
         "NielsenCbetSettings": NielsenCBETTypeDef,
         "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
         "NielsenNaesIiNwSettings": NielsenNaesIiNwTypeDef,
     },
     total=False,
 )
 
 OutputDestinationOutputTypeDef = TypedDict(
     "OutputDestinationOutputTypeDef",
     {
         "Id": str,
-        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsOutputTypeDef],
-        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsOutputTypeDef,
-        "Settings": List[OutputDestinationSettingsOutputTypeDef],
+        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsTypeDef],
+        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
+        "Settings": List[OutputDestinationSettingsTypeDef],
     },
     total=False,
 )
 
 OutputDestinationTypeDef = TypedDict(
     "OutputDestinationTypeDef",
     {
@@ -5176,100 +4072,27 @@
     },
     total=False,
 )
 
 PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsOutputTypeDef",
     {
-        "Pipelines": List[PipelinePauseStateSettingsOutputTypeDef],
+        "Pipelines": List[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
 
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
         "Pipelines": Sequence[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
 
-_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_RequiredPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Count": int,
-        "OfferingId": str,
-    },
-)
-_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_OptionalPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-        "RequestId": str,
-        "Start": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PurchaseOfferingRequestRequestTypeDef(
-    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReservationRequestRequestTypeDef",
-    {
-        "ReservationId": str,
-    },
-)
-_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReservationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-    },
-    total=False,
-)
-
-class UpdateReservationRequestRequestTypeDef(
-    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
-):
-    pass
-
-_RequiredScte35SegmentationDescriptorOutputTypeDef = TypedDict(
-    "_RequiredScte35SegmentationDescriptorOutputTypeDef",
-    {
-        "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
-        "SegmentationEventId": int,
-    },
-)
-_OptionalScte35SegmentationDescriptorOutputTypeDef = TypedDict(
-    "_OptionalScte35SegmentationDescriptorOutputTypeDef",
-    {
-        "DeliveryRestrictions": Scte35DeliveryRestrictionsOutputTypeDef,
-        "SegmentNum": int,
-        "SegmentationDuration": int,
-        "SegmentationTypeId": int,
-        "SegmentationUpid": str,
-        "SegmentationUpidType": int,
-        "SegmentsExpected": int,
-        "SubSegmentNum": int,
-        "SubSegmentsExpected": int,
-    },
-    total=False,
-)
-
-class Scte35SegmentationDescriptorOutputTypeDef(
-    _RequiredScte35SegmentationDescriptorOutputTypeDef,
-    _OptionalScte35SegmentationDescriptorOutputTypeDef,
-):
-    pass
-
 _RequiredScte35SegmentationDescriptorTypeDef = TypedDict(
     "_RequiredScte35SegmentationDescriptorTypeDef",
     {
         "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
         "SegmentationEventId": int,
     },
 )
@@ -5285,66 +4108,39 @@
         "SegmentsExpected": int,
         "SubSegmentNum": int,
         "SubSegmentsExpected": int,
     },
     total=False,
 )
 
+
 class Scte35SegmentationDescriptorTypeDef(
     _RequiredScte35SegmentationDescriptorTypeDef, _OptionalScte35SegmentationDescriptorTypeDef
 ):
     pass
 
+
 ThumbnailDetailTypeDef = TypedDict(
     "ThumbnailDetailTypeDef",
     {
         "PipelineId": str,
         "Thumbnails": List[ThumbnailTypeDef],
     },
     total=False,
 )
 
-VideoSelectorSettingsOutputTypeDef = TypedDict(
-    "VideoSelectorSettingsOutputTypeDef",
-    {
-        "VideoSelectorPid": VideoSelectorPidOutputTypeDef,
-        "VideoSelectorProgramId": VideoSelectorProgramIdOutputTypeDef,
-    },
-    total=False,
-)
-
 VideoSelectorSettingsTypeDef = TypedDict(
     "VideoSelectorSettingsTypeDef",
     {
         "VideoSelectorPid": VideoSelectorPidTypeDef,
         "VideoSelectorProgramId": VideoSelectorProgramIdTypeDef,
     },
     total=False,
 )
 
-_RequiredArchiveGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredArchiveGroupSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-_OptionalArchiveGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalArchiveGroupSettingsOutputTypeDef",
-    {
-        "ArchiveCdnSettings": ArchiveCdnSettingsOutputTypeDef,
-        "RolloverInterval": int,
-    },
-    total=False,
-)
-
-class ArchiveGroupSettingsOutputTypeDef(
-    _RequiredArchiveGroupSettingsOutputTypeDef, _OptionalArchiveGroupSettingsOutputTypeDef
-):
-    pass
-
 _RequiredArchiveGroupSettingsTypeDef = TypedDict(
     "_RequiredArchiveGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalArchiveGroupSettingsTypeDef = TypedDict(
@@ -5352,19 +4148,21 @@
     {
         "ArchiveCdnSettings": ArchiveCdnSettingsTypeDef,
         "RolloverInterval": int,
     },
     total=False,
 )
 
+
 class ArchiveGroupSettingsTypeDef(
     _RequiredArchiveGroupSettingsTypeDef, _OptionalArchiveGroupSettingsTypeDef
 ):
     pass
 
+
 _RequiredRemixSettingsOutputTypeDef = TypedDict(
     "_RequiredRemixSettingsOutputTypeDef",
     {
         "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
     },
 )
 _OptionalRemixSettingsOutputTypeDef = TypedDict(
@@ -5372,19 +4170,21 @@
     {
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
+
 class RemixSettingsOutputTypeDef(
     _RequiredRemixSettingsOutputTypeDef, _OptionalRemixSettingsOutputTypeDef
 ):
     pass
 
+
 _RequiredRemixSettingsTypeDef = TypedDict(
     "_RequiredRemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
     },
 )
 _OptionalRemixSettingsTypeDef = TypedDict(
@@ -5392,76 +4192,35 @@
     {
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
+
 class RemixSettingsTypeDef(_RequiredRemixSettingsTypeDef, _OptionalRemixSettingsTypeDef):
     pass
 
+
 CaptionDestinationSettingsOutputTypeDef = TypedDict(
     "CaptionDestinationSettingsOutputTypeDef",
     {
         "AribDestinationSettings": Dict[str, Any],
-        "BurnInDestinationSettings": BurnInDestinationSettingsOutputTypeDef,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
-        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsOutputTypeDef,
+        "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
+        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": Dict[str, Any],
         "EmbeddedPlusScte20DestinationSettings": Dict[str, Any],
         "RtmpCaptionInfoDestinationSettings": Dict[str, Any],
         "Scte20PlusEmbeddedDestinationSettings": Dict[str, Any],
         "Scte27DestinationSettings": Dict[str, Any],
         "SmpteTtDestinationSettings": Dict[str, Any],
         "TeletextDestinationSettings": Dict[str, Any],
-        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-GlobalConfigurationOutputTypeDef = TypedDict(
-    "GlobalConfigurationOutputTypeDef",
-    {
-        "InitialAudioGain": int,
-        "InputEndAction": GlobalConfigurationInputEndActionType,
-        "InputLossBehavior": InputLossBehaviorOutputTypeDef,
-        "OutputLockingMode": GlobalConfigurationOutputLockingModeType,
-        "OutputTimingSource": GlobalConfigurationOutputTimingSourceType,
-        "SupportLowFramerateInputs": GlobalConfigurationLowFramerateInputsType,
-    },
-    total=False,
-)
-
-KeyProviderSettingsOutputTypeDef = TypedDict(
-    "KeyProviderSettingsOutputTypeDef",
-    {
-        "StaticKeySettings": StaticKeySettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-AudioSelectorSettingsOutputTypeDef = TypedDict(
-    "AudioSelectorSettingsOutputTypeDef",
-    {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionOutputTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionOutputTypeDef,
-        "AudioPidSelection": AudioPidSelectionOutputTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
-AudioSelectorSettingsTypeDef = TypedDict(
-    "AudioSelectorSettingsTypeDef",
-    {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
-        "AudioPidSelection": AudioPidSelectionTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
     },
     total=False,
 )
 
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
@@ -5499,18 +4258,32 @@
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": StaticKeySettingsTypeDef,
     },
     total=False,
 )
 
-AvailConfigurationOutputTypeDef = TypedDict(
-    "AvailConfigurationOutputTypeDef",
+AudioSelectorSettingsOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsOutputTypeDef",
+    {
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
+        "AudioPidSelection": AudioPidSelectionTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+AudioSelectorSettingsTypeDef = TypedDict(
+    "AudioSelectorSettingsTypeDef",
     {
-        "AvailSettings": AvailSettingsOutputTypeDef,
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
+        "AudioPidSelection": AudioPidSelectionTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionTypeDef,
     },
     total=False,
 )
 
 AvailConfigurationTypeDef = TypedDict(
     "AvailConfigurationTypeDef",
     {
@@ -5518,21 +4291,21 @@
     },
     total=False,
 )
 
 CaptionSelectorSettingsOutputTypeDef = TypedDict(
     "CaptionSelectorSettingsOutputTypeDef",
     {
-        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "AribSourceSettings": Dict[str, Any],
-        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
-        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
-        "Scte20SourceSettings": Scte20SourceSettingsOutputTypeDef,
-        "Scte27SourceSettings": Scte27SourceSettingsOutputTypeDef,
-        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+        "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
+        "Scte20SourceSettings": Scte20SourceSettingsTypeDef,
+        "Scte27SourceSettings": Scte27SourceSettingsTypeDef,
+        "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
     },
     total=False,
 )
 
 CaptionSelectorSettingsTypeDef = TypedDict(
     "CaptionSelectorSettingsTypeDef",
     {
@@ -5548,160 +4321,135 @@
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReservationResponseTypeDef = TypedDict(
     "UpdateReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInputSecurityGroupResponseTypeDef = TypedDict(
     "CreateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArchiveContainerSettingsOutputTypeDef = TypedDict(
-    "ArchiveContainerSettingsOutputTypeDef",
+ArchiveContainerSettingsTypeDef = TypedDict(
+    "ArchiveContainerSettingsTypeDef",
     {
-        "M2tsSettings": M2tsSettingsOutputTypeDef,
-        "RawSettings": Dict[str, Any],
+        "M2tsSettings": M2tsSettingsTypeDef,
+        "RawSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-UdpContainerSettingsOutputTypeDef = TypedDict(
-    "UdpContainerSettingsOutputTypeDef",
+UdpContainerSettingsTypeDef = TypedDict(
+    "UdpContainerSettingsTypeDef",
     {
-        "M2tsSettings": M2tsSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-FailoverConditionOutputTypeDef = TypedDict(
-    "FailoverConditionOutputTypeDef",
-    {
-        "FailoverConditionSettings": FailoverConditionSettingsOutputTypeDef,
+        "M2tsSettings": M2tsSettingsTypeDef,
     },
     total=False,
 )
 
 FailoverConditionTypeDef = TypedDict(
     "FailoverConditionTypeDef",
     {
         "FailoverConditionSettings": FailoverConditionSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredFrameCaptureGroupSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefOutputTypeDef,
-    },
-)
-_OptionalFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalFrameCaptureGroupSettingsOutputTypeDef",
-    {
-        "FrameCaptureCdnSettings": FrameCaptureCdnSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class FrameCaptureGroupSettingsOutputTypeDef(
-    _RequiredFrameCaptureGroupSettingsOutputTypeDef, _OptionalFrameCaptureGroupSettingsOutputTypeDef
-):
-    pass
-
 _RequiredFrameCaptureGroupSettingsTypeDef = TypedDict(
     "_RequiredFrameCaptureGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalFrameCaptureGroupSettingsTypeDef = TypedDict(
     "_OptionalFrameCaptureGroupSettingsTypeDef",
     {
         "FrameCaptureCdnSettings": FrameCaptureCdnSettingsTypeDef,
     },
     total=False,
 )
 
+
 class FrameCaptureGroupSettingsTypeDef(
     _RequiredFrameCaptureGroupSettingsTypeDef, _OptionalFrameCaptureGroupSettingsTypeDef
 ):
     pass
 
+
 H264SettingsOutputTypeDef = TypedDict(
     "H264SettingsOutputTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
         "BufSize": int,
         "ColorMetadata": H264ColorMetadataType,
         "ColorSpaceSettings": H264ColorSpaceSettingsOutputTypeDef,
         "EntropyEncoding": H264EntropyEncodingType,
-        "FilterSettings": H264FilterSettingsOutputTypeDef,
+        "FilterSettings": H264FilterSettingsTypeDef,
         "FixedAfd": FixedAfdType,
         "FlickerAq": H264FlickerAqType,
         "ForceFieldPictures": H264ForceFieldPicturesType,
         "FramerateControl": H264FramerateControlType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "GopBReference": H264GopBReferenceType,
@@ -5726,53 +4474,19 @@
         "Slices": int,
         "Softness": int,
         "SpatialAq": H264SpatialAqType,
         "SubgopLength": H264SubGopLengthType,
         "Syntax": H264SyntaxType,
         "TemporalAq": H264TemporalAqType,
         "TimecodeInsertion": H264TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredMpeg2SettingsOutputTypeDef = TypedDict(
-    "_RequiredMpeg2SettingsOutputTypeDef",
-    {
-        "FramerateDenominator": int,
-        "FramerateNumerator": int,
-    },
-)
-_OptionalMpeg2SettingsOutputTypeDef = TypedDict(
-    "_OptionalMpeg2SettingsOutputTypeDef",
-    {
-        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
-        "AfdSignaling": AfdSignalingType,
-        "ColorMetadata": Mpeg2ColorMetadataType,
-        "ColorSpace": Mpeg2ColorSpaceType,
-        "DisplayAspectRatio": Mpeg2DisplayRatioType,
-        "FilterSettings": Mpeg2FilterSettingsOutputTypeDef,
-        "FixedAfd": FixedAfdType,
-        "GopClosedCadence": int,
-        "GopNumBFrames": int,
-        "GopSize": float,
-        "GopSizeUnits": Mpeg2GopSizeUnitsType,
-        "ScanType": Mpeg2ScanTypeType,
-        "SubgopLength": Mpeg2SubGopLengthType,
-        "TimecodeInsertion": Mpeg2TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
-class Mpeg2SettingsOutputTypeDef(
-    _RequiredMpeg2SettingsOutputTypeDef, _OptionalMpeg2SettingsOutputTypeDef
-):
-    pass
-
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
@@ -5843,17 +4557,19 @@
         "SubgopLength": Mpeg2SubGopLengthType,
         "TimecodeInsertion": Mpeg2TimecodeInsertionBehaviorType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
+
 class Mpeg2SettingsTypeDef(_RequiredMpeg2SettingsTypeDef, _OptionalMpeg2SettingsTypeDef):
     pass
 
+
 _RequiredH265SettingsOutputTypeDef = TypedDict(
     "_RequiredH265SettingsOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -5863,15 +4579,15 @@
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "AlternativeTransferFunction": H265AlternativeTransferFunctionType,
         "Bitrate": int,
         "BufSize": int,
         "ColorMetadata": H265ColorMetadataType,
         "ColorSpaceSettings": H265ColorSpaceSettingsOutputTypeDef,
-        "FilterSettings": H265FilterSettingsOutputTypeDef,
+        "FilterSettings": H265FilterSettingsTypeDef,
         "FixedAfd": FixedAfdType,
         "FlickerAq": H265FlickerAqType,
         "GopClosedCadence": int,
         "GopSize": float,
         "GopSizeUnits": H265GopSizeUnitsType,
         "Level": H265LevelType,
         "LookAheadRateControl": H265LookAheadRateControlType,
@@ -5883,24 +4599,26 @@
         "QvbrQualityLevel": int,
         "RateControlMode": H265RateControlModeType,
         "ScanType": H265ScanTypeType,
         "SceneChangeDetect": H265SceneChangeDetectType,
         "Slices": int,
         "Tier": H265TierType,
         "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
+
 class H265SettingsOutputTypeDef(
     _RequiredH265SettingsOutputTypeDef, _OptionalH265SettingsOutputTypeDef
 ):
     pass
 
+
 _RequiredH265SettingsTypeDef = TypedDict(
     "_RequiredH265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -5935,57 +4653,61 @@
         "Tier": H265TierType,
         "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
+
 class H265SettingsTypeDef(_RequiredH265SettingsTypeDef, _OptionalH265SettingsTypeDef):
     pass
 
+
 InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": str,
-        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": List[str],
     },
     total=False,
 )
 
+InputPrepareScheduleActionSettingsTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+        "InputClippingSettings": InputClippingSettingsTypeDef,
+        "UrlPath": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
     "_RequiredInputSwitchScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
 )
 _OptionalInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
     "_OptionalInputSwitchScheduleActionSettingsOutputTypeDef",
     {
-        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": List[str],
     },
     total=False,
 )
 
+
 class InputSwitchScheduleActionSettingsOutputTypeDef(
     _RequiredInputSwitchScheduleActionSettingsOutputTypeDef,
     _OptionalInputSwitchScheduleActionSettingsOutputTypeDef,
 ):
     pass
 
-InputPrepareScheduleActionSettingsTypeDef = TypedDict(
-    "InputPrepareScheduleActionSettingsTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-        "InputClippingSettings": InputClippingSettingsTypeDef,
-        "UrlPath": Sequence[str],
-    },
-    total=False,
-)
 
 _RequiredInputSwitchScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredInputSwitchScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
 )
@@ -5994,119 +4716,121 @@
     {
         "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": Sequence[str],
     },
     total=False,
 )
 
+
 class InputSwitchScheduleActionSettingsTypeDef(
     _RequiredInputSwitchScheduleActionSettingsTypeDef,
     _OptionalInputSwitchScheduleActionSettingsTypeDef,
 ):
     pass
 
+
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
+        "InputDevices": List[InputDeviceSettingsTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
+        "InputDevices": List[InputDeviceSettingsTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
     },
     total=False,
 )
 
-HlsSettingsOutputTypeDef = TypedDict(
-    "HlsSettingsOutputTypeDef",
+HlsSettingsTypeDef = TypedDict(
+    "HlsSettingsTypeDef",
     {
-        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsOutputTypeDef,
-        "Fmp4HlsSettings": Fmp4HlsSettingsOutputTypeDef,
-        "FrameCaptureHlsSettings": Dict[str, Any],
-        "StandardHlsSettings": StandardHlsSettingsOutputTypeDef,
+        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsTypeDef,
+        "Fmp4HlsSettings": Fmp4HlsSettingsTypeDef,
+        "FrameCaptureHlsSettings": Mapping[str, Any],
+        "StandardHlsSettings": StandardHlsSettingsTypeDef,
     },
     total=False,
 )
 
 DeleteMultiplexResponseTypeDef = TypedDict(
     "DeleteMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMultiplexResponseTypeDef = TypedDict(
     "DescribeMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MultiplexTypeDef = TypedDict(
     "MultiplexTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
@@ -6115,70 +4839,49 @@
 StartMultiplexResponseTypeDef = TypedDict(
     "StartMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopMultiplexResponseTypeDef = TypedDict(
     "StopMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
+        "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredMultiplexProgramSettingsOutputTypeDef = TypedDict(
-    "_RequiredMultiplexProgramSettingsOutputTypeDef",
-    {
-        "ProgramNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalMultiplexProgramSettingsOutputTypeDef = TypedDict(
-    "_OptionalMultiplexProgramSettingsOutputTypeDef",
-    {
-        "PreferredChannelPipeline": PreferredChannelPipelineType,
-        "ServiceDescriptor": MultiplexProgramServiceDescriptorOutputTypeDef,
-        "VideoSettings": MultiplexVideoSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class MultiplexProgramSettingsOutputTypeDef(
-    _RequiredMultiplexProgramSettingsOutputTypeDef, _OptionalMultiplexProgramSettingsOutputTypeDef
-):
-    pass
 
 _RequiredMultiplexProgramSettingsTypeDef = TypedDict(
     "_RequiredMultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
     },
 )
@@ -6188,26 +4891,20 @@
         "PreferredChannelPipeline": PreferredChannelPipelineType,
         "ServiceDescriptor": MultiplexProgramServiceDescriptorTypeDef,
         "VideoSettings": MultiplexVideoSettingsTypeDef,
     },
     total=False,
 )
 
+
 class MultiplexProgramSettingsTypeDef(
     _RequiredMultiplexProgramSettingsTypeDef, _OptionalMultiplexProgramSettingsTypeDef
 ):
     pass
 
-AudioWatermarkSettingsOutputTypeDef = TypedDict(
-    "AudioWatermarkSettingsOutputTypeDef",
-    {
-        "NielsenWatermarksSettings": NielsenWatermarksSettingsOutputTypeDef,
-    },
-    total=False,
-)
 
 AudioWatermarkSettingsTypeDef = TypedDict(
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
@@ -6224,51 +4921,35 @@
     "_OptionalUpdateChannelClassRequestRequestTypeDef",
     {
         "Destinations": Sequence[OutputDestinationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateChannelClassRequestRequestTypeDef(
     _RequiredUpdateChannelClassRequestRequestTypeDef,
     _OptionalUpdateChannelClassRequestRequestTypeDef,
 ):
     pass
 
-Scte35DescriptorSettingsOutputTypeDef = TypedDict(
-    "Scte35DescriptorSettingsOutputTypeDef",
-    {
-        "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorOutputTypeDef,
-    },
-)
 
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
 DescribeThumbnailsResponseTypeDef = TypedDict(
     "DescribeThumbnailsResponseTypeDef",
     {
         "ThumbnailDetails": List[ThumbnailDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VideoSelectorOutputTypeDef = TypedDict(
-    "VideoSelectorOutputTypeDef",
-    {
-        "ColorSpace": VideoSelectorColorSpaceType,
-        "ColorSpaceSettings": VideoSelectorColorSpaceSettingsOutputTypeDef,
-        "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
-        "SelectorSettings": VideoSelectorSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 VideoSelectorTypeDef = TypedDict(
     "VideoSelectorTypeDef",
     {
         "ColorSpace": VideoSelectorColorSpaceType,
         "ColorSpaceSettings": VideoSelectorColorSpaceSettingsTypeDef,
@@ -6292,53 +4973,80 @@
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": str,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+
 class CaptionDescriptionOutputTypeDef(
     _RequiredCaptionDescriptionOutputTypeDef, _OptionalCaptionDescriptionOutputTypeDef
 ):
     pass
 
+
+_RequiredCaptionDescriptionTypeDef = TypedDict(
+    "_RequiredCaptionDescriptionTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "Name": str,
+    },
+)
+_OptionalCaptionDescriptionTypeDef = TypedDict(
+    "_OptionalCaptionDescriptionTypeDef",
+    {
+        "Accessibility": AccessibilityTypeType,
+        "DestinationSettings": CaptionDestinationSettingsTypeDef,
+        "LanguageCode": str,
+        "LanguageDescription": str,
+    },
+    total=False,
+)
+
+
+class CaptionDescriptionTypeDef(
+    _RequiredCaptionDescriptionTypeDef, _OptionalCaptionDescriptionTypeDef
+):
+    pass
+
+
 _RequiredHlsGroupSettingsOutputTypeDef = TypedDict(
     "_RequiredHlsGroupSettingsOutputTypeDef",
     {
-        "Destination": OutputLocationRefOutputTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalHlsGroupSettingsOutputTypeDef = TypedDict(
     "_OptionalHlsGroupSettingsOutputTypeDef",
     {
         "AdMarkers": List[HlsAdMarkersType],
         "BaseUrlContent": str,
         "BaseUrlContent1": str,
         "BaseUrlManifest": str,
         "BaseUrlManifest1": str,
-        "CaptionLanguageMappings": List[CaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageMappings": List[CaptionLanguageMappingTypeDef],
         "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
         "ClientCache": HlsClientCacheType,
         "CodecSpecification": HlsCodecSpecificationType,
         "ConstantIv": str,
         "DirectoryStructure": HlsDirectoryStructureType,
         "DiscontinuityTags": HlsDiscontinuityTagsType,
         "EncryptionType": HlsEncryptionTypeType,
-        "HlsCdnSettings": HlsCdnSettingsOutputTypeDef,
+        "HlsCdnSettings": HlsCdnSettingsTypeDef,
         "HlsId3SegmentTagging": HlsId3SegmentTaggingStateType,
         "IFrameOnlyPlaylists": IFrameOnlyPlaylistTypeType,
         "IncompleteSegmentBehavior": HlsIncompleteSegmentBehaviorType,
         "IndexNSegments": int,
         "InputLossAction": InputLossActionForHlsOutType,
         "IvInManifest": HlsIvInManifestType,
         "IvSource": HlsIvSourceType,
         "KeepSegments": int,
         "KeyFormat": str,
         "KeyFormatVersions": str,
-        "KeyProviderSettings": KeyProviderSettingsOutputTypeDef,
+        "KeyProviderSettings": KeyProviderSettingsTypeDef,
         "ManifestCompression": HlsManifestCompressionType,
         "ManifestDurationFormat": HlsManifestDurationFormatType,
         "MinSegmentLength": int,
         "Mode": HlsModeType,
         "OutputSelection": HlsOutputSelectionType,
         "ProgramDateTime": HlsProgramDateTimeType,
         "ProgramDateTimeClock": HlsProgramDateTimeClockType,
@@ -6352,77 +5060,20 @@
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
         "TsFileMode": HlsTsFileModeType,
     },
     total=False,
 )
 
+
 class HlsGroupSettingsOutputTypeDef(
     _RequiredHlsGroupSettingsOutputTypeDef, _OptionalHlsGroupSettingsOutputTypeDef
 ):
     pass
 
-_RequiredAudioSelectorOutputTypeDef = TypedDict(
-    "_RequiredAudioSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAudioSelectorOutputTypeDef = TypedDict(
-    "_OptionalAudioSelectorOutputTypeDef",
-    {
-        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class AudioSelectorOutputTypeDef(
-    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
-):
-    pass
-
-_RequiredAudioSelectorTypeDef = TypedDict(
-    "_RequiredAudioSelectorTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAudioSelectorTypeDef = TypedDict(
-    "_OptionalAudioSelectorTypeDef",
-    {
-        "SelectorSettings": AudioSelectorSettingsTypeDef,
-    },
-    total=False,
-)
-
-class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
-    pass
-
-_RequiredCaptionDescriptionTypeDef = TypedDict(
-    "_RequiredCaptionDescriptionTypeDef",
-    {
-        "CaptionSelectorName": str,
-        "Name": str,
-    },
-)
-_OptionalCaptionDescriptionTypeDef = TypedDict(
-    "_OptionalCaptionDescriptionTypeDef",
-    {
-        "Accessibility": AccessibilityTypeType,
-        "DestinationSettings": CaptionDestinationSettingsTypeDef,
-        "LanguageCode": str,
-        "LanguageDescription": str,
-    },
-    total=False,
-)
-
-class CaptionDescriptionTypeDef(
-    _RequiredCaptionDescriptionTypeDef, _OptionalCaptionDescriptionTypeDef
-):
-    pass
 
 _RequiredHlsGroupSettingsTypeDef = TypedDict(
     "_RequiredHlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
@@ -6471,17 +5122,59 @@
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
         "TsFileMode": HlsTsFileModeType,
     },
     total=False,
 )
 
+
 class HlsGroupSettingsTypeDef(_RequiredHlsGroupSettingsTypeDef, _OptionalHlsGroupSettingsTypeDef):
     pass
 
+
+_RequiredAudioSelectorOutputTypeDef = TypedDict(
+    "_RequiredAudioSelectorOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorOutputTypeDef = TypedDict(
+    "_OptionalAudioSelectorOutputTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AudioSelectorOutputTypeDef(
+    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
+):
+    pass
+
+
+_RequiredAudioSelectorTypeDef = TypedDict(
+    "_RequiredAudioSelectorTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorTypeDef = TypedDict(
+    "_OptionalAudioSelectorTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
+    pass
+
+
 _RequiredCaptionSelectorOutputTypeDef = TypedDict(
     "_RequiredCaptionSelectorOutputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCaptionSelectorOutputTypeDef = TypedDict(
@@ -6489,19 +5182,21 @@
     {
         "LanguageCode": str,
         "SelectorSettings": CaptionSelectorSettingsOutputTypeDef,
     },
     total=False,
 )
 
+
 class CaptionSelectorOutputTypeDef(
     _RequiredCaptionSelectorOutputTypeDef, _OptionalCaptionSelectorOutputTypeDef
 ):
     pass
 
+
 _RequiredCaptionSelectorTypeDef = TypedDict(
     "_RequiredCaptionSelectorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCaptionSelectorTypeDef = TypedDict(
@@ -6509,80 +5204,88 @@
     {
         "LanguageCode": str,
         "SelectorSettings": CaptionSelectorSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CaptionSelectorTypeDef(_RequiredCaptionSelectorTypeDef, _OptionalCaptionSelectorTypeDef):
     pass
 
-_RequiredArchiveOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredArchiveOutputSettingsOutputTypeDef",
+
+_RequiredArchiveOutputSettingsTypeDef = TypedDict(
+    "_RequiredArchiveOutputSettingsTypeDef",
     {
-        "ContainerSettings": ArchiveContainerSettingsOutputTypeDef,
+        "ContainerSettings": ArchiveContainerSettingsTypeDef,
     },
 )
-_OptionalArchiveOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalArchiveOutputSettingsOutputTypeDef",
+_OptionalArchiveOutputSettingsTypeDef = TypedDict(
+    "_OptionalArchiveOutputSettingsTypeDef",
     {
         "Extension": str,
         "NameModifier": str,
     },
     total=False,
 )
 
-class ArchiveOutputSettingsOutputTypeDef(
-    _RequiredArchiveOutputSettingsOutputTypeDef, _OptionalArchiveOutputSettingsOutputTypeDef
+
+class ArchiveOutputSettingsTypeDef(
+    _RequiredArchiveOutputSettingsTypeDef, _OptionalArchiveOutputSettingsTypeDef
 ):
     pass
 
-_RequiredUdpOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredUdpOutputSettingsOutputTypeDef",
+
+_RequiredUdpOutputSettingsTypeDef = TypedDict(
+    "_RequiredUdpOutputSettingsTypeDef",
     {
-        "ContainerSettings": UdpContainerSettingsOutputTypeDef,
-        "Destination": OutputLocationRefOutputTypeDef,
+        "ContainerSettings": UdpContainerSettingsTypeDef,
+        "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalUdpOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalUdpOutputSettingsOutputTypeDef",
+_OptionalUdpOutputSettingsTypeDef = TypedDict(
+    "_OptionalUdpOutputSettingsTypeDef",
     {
         "BufferMsec": int,
-        "FecOutputSettings": FecOutputSettingsOutputTypeDef,
+        "FecOutputSettings": FecOutputSettingsTypeDef,
     },
     total=False,
 )
 
-class UdpOutputSettingsOutputTypeDef(
-    _RequiredUdpOutputSettingsOutputTypeDef, _OptionalUdpOutputSettingsOutputTypeDef
+
+class UdpOutputSettingsTypeDef(
+    _RequiredUdpOutputSettingsTypeDef, _OptionalUdpOutputSettingsTypeDef
 ):
     pass
 
+
 _RequiredAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsOutputTypeDef",
     {
         "SecondaryInputId": str,
     },
 )
 _OptionalAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
     "_OptionalAutomaticInputFailoverSettingsOutputTypeDef",
     {
         "ErrorClearTimeMsec": int,
-        "FailoverConditions": List[FailoverConditionOutputTypeDef],
+        "FailoverConditions": List[FailoverConditionTypeDef],
         "InputPreference": InputPreferenceType,
     },
     total=False,
 )
 
+
 class AutomaticInputFailoverSettingsOutputTypeDef(
     _RequiredAutomaticInputFailoverSettingsOutputTypeDef,
     _OptionalAutomaticInputFailoverSettingsOutputTypeDef,
 ):
     pass
 
+
 _RequiredAutomaticInputFailoverSettingsTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsTypeDef",
     {
         "SecondaryInputId": str,
     },
 )
 _OptionalAutomaticInputFailoverSettingsTypeDef = TypedDict(
@@ -6591,26 +5294,28 @@
         "ErrorClearTimeMsec": int,
         "FailoverConditions": Sequence[FailoverConditionTypeDef],
         "InputPreference": InputPreferenceType,
     },
     total=False,
 )
 
+
 class AutomaticInputFailoverSettingsTypeDef(
     _RequiredAutomaticInputFailoverSettingsTypeDef, _OptionalAutomaticInputFailoverSettingsTypeDef
 ):
     pass
 
+
 VideoCodecSettingsOutputTypeDef = TypedDict(
     "VideoCodecSettingsOutputTypeDef",
     {
-        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
         "H264Settings": H264SettingsOutputTypeDef,
         "H265Settings": H265SettingsOutputTypeDef,
-        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsTypeDef,
     },
     total=False,
 )
 
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
@@ -6622,126 +5327,128 @@
     total=False,
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePartnerInputResponseTypeDef = TypedDict(
     "CreatePartnerInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHlsOutputSettingsOutputTypeDef = TypedDict(
-    "_RequiredHlsOutputSettingsOutputTypeDef",
+_RequiredHlsOutputSettingsTypeDef = TypedDict(
+    "_RequiredHlsOutputSettingsTypeDef",
     {
-        "HlsSettings": HlsSettingsOutputTypeDef,
+        "HlsSettings": HlsSettingsTypeDef,
     },
 )
-_OptionalHlsOutputSettingsOutputTypeDef = TypedDict(
-    "_OptionalHlsOutputSettingsOutputTypeDef",
+_OptionalHlsOutputSettingsTypeDef = TypedDict(
+    "_OptionalHlsOutputSettingsTypeDef",
     {
         "H265PackagingType": HlsH265PackagingTypeType,
         "NameModifier": str,
         "SegmentModifier": str,
     },
     total=False,
 )
 
-class HlsOutputSettingsOutputTypeDef(
-    _RequiredHlsOutputSettingsOutputTypeDef, _OptionalHlsOutputSettingsOutputTypeDef
+
+class HlsOutputSettingsTypeDef(
+    _RequiredHlsOutputSettingsTypeDef, _OptionalHlsOutputSettingsTypeDef
 ):
     pass
 
+
 CreateMultiplexResponseTypeDef = TypedDict(
     "CreateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMultiplexResponseTypeDef = TypedDict(
     "UpdateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
+    "CreateMultiplexProgramRequestRequestTypeDef",
+    {
+        "MultiplexId": str,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "ProgramName": str,
+        "RequestId": str,
     },
 )
 
 DeleteMultiplexProgramResponseTypeDef = TypedDict(
     "DeleteMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMultiplexProgramResponseTypeDef = TypedDict(
     "DescribeMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MultiplexProgramTypeDef = TypedDict(
     "MultiplexProgramTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
     },
     total=False,
 )
 
-CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
-    "CreateMultiplexProgramRequestRequestTypeDef",
-    {
-        "MultiplexId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
-        "ProgramName": str,
-        "RequestId": str,
-    },
-)
-
 _RequiredUpdateMultiplexProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
 )
@@ -6749,48 +5456,52 @@
     "_OptionalUpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMultiplexProgramRequestRequestTypeDef(
     _RequiredUpdateMultiplexProgramRequestRequestTypeDef,
     _OptionalUpdateMultiplexProgramRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredAudioDescriptionOutputTypeDef = TypedDict(
     "_RequiredAudioDescriptionOutputTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
 _OptionalAudioDescriptionOutputTypeDef = TypedDict(
     "_OptionalAudioDescriptionOutputTypeDef",
     {
-        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioType": AudioTypeType,
         "AudioTypeControl": AudioDescriptionAudioTypeControlType,
-        "AudioWatermarkingSettings": AudioWatermarkSettingsOutputTypeDef,
+        "AudioWatermarkingSettings": AudioWatermarkSettingsTypeDef,
         "CodecSettings": AudioCodecSettingsOutputTypeDef,
         "LanguageCode": str,
         "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "StreamName": str,
     },
     total=False,
 )
 
+
 class AudioDescriptionOutputTypeDef(
     _RequiredAudioDescriptionOutputTypeDef, _OptionalAudioDescriptionOutputTypeDef
 ):
     pass
 
+
 _RequiredAudioDescriptionTypeDef = TypedDict(
     "_RequiredAudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
@@ -6806,42 +5517,37 @@
         "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
         "RemixSettings": RemixSettingsTypeDef,
         "StreamName": str,
     },
     total=False,
 )
 
+
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
-Scte35DescriptorOutputTypeDef = TypedDict(
-    "Scte35DescriptorOutputTypeDef",
-    {
-        "Scte35DescriptorSettings": Scte35DescriptorSettingsOutputTypeDef,
-    },
-)
 
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
 OutputGroupSettingsOutputTypeDef = TypedDict(
     "OutputGroupSettingsOutputTypeDef",
     {
-        "ArchiveGroupSettings": ArchiveGroupSettingsOutputTypeDef,
-        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsOutputTypeDef,
+        "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
+        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
-        "MediaPackageGroupSettings": MediaPackageGroupSettingsOutputTypeDef,
-        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "MultiplexGroupSettings": Dict[str, Any],
         "RtmpGroupSettings": RtmpGroupSettingsOutputTypeDef,
-        "UdpGroupSettings": UdpGroupSettingsOutputTypeDef,
+        "UdpGroupSettings": UdpGroupSettingsTypeDef,
     },
     total=False,
 )
 
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
@@ -6862,19 +5568,19 @@
     {
         "AudioSelectors": List[AudioSelectorOutputTypeDef],
         "CaptionSelectors": List[CaptionSelectorOutputTypeDef],
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
         "FilterStrength": int,
         "InputFilter": InputFilterType,
-        "NetworkInputSettings": NetworkInputSettingsOutputTypeDef,
+        "NetworkInputSettings": NetworkInputSettingsTypeDef,
         "Scte35Pid": int,
         "Smpte2038DataPreference": Smpte2038DataPreferenceType,
         "SourceEndBehavior": InputSourceEndBehaviorType,
-        "VideoSelector": VideoSelectorOutputTypeDef,
+        "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
 InputSettingsTypeDef = TypedDict(
     "InputSettingsTypeDef",
     {
@@ -6908,19 +5614,21 @@
         "ScalingBehavior": VideoDescriptionScalingBehaviorType,
         "Sharpness": int,
         "Width": int,
     },
     total=False,
 )
 
+
 class VideoDescriptionOutputTypeDef(
     _RequiredVideoDescriptionOutputTypeDef, _OptionalVideoDescriptionOutputTypeDef
 ):
     pass
 
+
 _RequiredVideoDescriptionTypeDef = TypedDict(
     "_RequiredVideoDescriptionTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVideoDescriptionTypeDef = TypedDict(
@@ -6932,52 +5640,54 @@
         "ScalingBehavior": VideoDescriptionScalingBehaviorType,
         "Sharpness": int,
         "Width": int,
     },
     total=False,
 )
 
+
 class VideoDescriptionTypeDef(_RequiredVideoDescriptionTypeDef, _OptionalVideoDescriptionTypeDef):
     pass
 
-OutputSettingsOutputTypeDef = TypedDict(
-    "OutputSettingsOutputTypeDef",
+
+OutputSettingsTypeDef = TypedDict(
+    "OutputSettingsTypeDef",
     {
-        "ArchiveOutputSettings": ArchiveOutputSettingsOutputTypeDef,
-        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsOutputTypeDef,
-        "HlsOutputSettings": HlsOutputSettingsOutputTypeDef,
-        "MediaPackageOutputSettings": Dict[str, Any],
-        "MsSmoothOutputSettings": MsSmoothOutputSettingsOutputTypeDef,
-        "MultiplexOutputSettings": MultiplexOutputSettingsOutputTypeDef,
-        "RtmpOutputSettings": RtmpOutputSettingsOutputTypeDef,
-        "UdpOutputSettings": UdpOutputSettingsOutputTypeDef,
+        "ArchiveOutputSettings": ArchiveOutputSettingsTypeDef,
+        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsTypeDef,
+        "HlsOutputSettings": HlsOutputSettingsTypeDef,
+        "MediaPackageOutputSettings": Mapping[str, Any],
+        "MsSmoothOutputSettings": MsSmoothOutputSettingsTypeDef,
+        "MultiplexOutputSettings": MultiplexOutputSettingsTypeDef,
+        "RtmpOutputSettings": RtmpOutputSettingsTypeDef,
+        "UdpOutputSettings": UdpOutputSettingsTypeDef,
     },
     total=False,
 )
 
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     {
-        "Scte35Descriptors": List[Scte35DescriptorOutputTypeDef],
+        "Scte35Descriptors": List[Scte35DescriptorTypeDef],
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
@@ -7005,49 +5715,49 @@
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
-        "OutputSettings": OutputSettingsOutputTypeDef,
+        "OutputSettings": OutputSettingsTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
-        "AudioDescriptionNames": List[str],
-        "CaptionDescriptionNames": List[str],
+        "AudioDescriptionNames": Sequence[str],
+        "CaptionDescriptionNames": Sequence[str],
         "OutputName": str,
         "VideoDescriptionName": str,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+
 ScheduleActionSettingsOutputTypeDef = TypedDict(
     "ScheduleActionSettingsOutputTypeDef",
     {
-        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
-        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
+        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
+        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
         "InputPrepareSettings": InputPrepareScheduleActionSettingsOutputTypeDef,
         "InputSwitchSettings": InputSwitchScheduleActionSettingsOutputTypeDef,
-        "MotionGraphicsImageActivateSettings": (
-            MotionGraphicsActivateScheduleActionSettingsOutputTypeDef
-        ),
+        "MotionGraphicsImageActivateSettings": MotionGraphicsActivateScheduleActionSettingsTypeDef,
         "MotionGraphicsImageDeactivateSettings": Dict[str, Any],
         "PauseStateSettings": PauseStateScheduleActionSettingsOutputTypeDef,
-        "Scte35InputSettings": Scte35InputScheduleActionSettingsOutputTypeDef,
-        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
-        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+        "Scte35InputSettings": Scte35InputScheduleActionSettingsTypeDef,
+        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
+        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsTypeDef,
         "Scte35TimeSignalSettings": Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
-        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsOutputTypeDef,
-        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
+        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsTypeDef,
+        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsTypeDef,
     },
     total=False,
 )
 
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
@@ -7068,21 +5778,21 @@
     total=False,
 )
 
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
@@ -7102,19 +5812,21 @@
     "_OptionalOutputGroupOutputTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class OutputGroupOutputTypeDef(
     _RequiredOutputGroupOutputTypeDef, _OptionalOutputGroupOutputTypeDef
 ):
     pass
 
+
 _RequiredOutputGroupTypeDef = TypedDict(
     "_RequiredOutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
 )
@@ -7122,17 +5834,19 @@
     "_OptionalOutputGroupTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class OutputGroupTypeDef(_RequiredOutputGroupTypeDef, _OptionalOutputGroupTypeDef):
     pass
 
+
 ScheduleActionOutputTypeDef = TypedDict(
     "ScheduleActionOutputTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
     },
@@ -7148,48 +5862,50 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEncoderSettingsOutputTypeDef = TypedDict(
     "_RequiredEncoderSettingsOutputTypeDef",
     {
         "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
         "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
     },
 )
 _OptionalEncoderSettingsOutputTypeDef = TypedDict(
     "_OptionalEncoderSettingsOutputTypeDef",
     {
-        "AvailBlanking": AvailBlankingOutputTypeDef,
-        "AvailConfiguration": AvailConfigurationOutputTypeDef,
-        "BlackoutSlate": BlackoutSlateOutputTypeDef,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "AvailConfiguration": AvailConfigurationTypeDef,
+        "BlackoutSlate": BlackoutSlateTypeDef,
         "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
-        "FeatureActivations": FeatureActivationsOutputTypeDef,
-        "GlobalConfiguration": GlobalConfigurationOutputTypeDef,
+        "FeatureActivations": FeatureActivationsTypeDef,
+        "GlobalConfiguration": GlobalConfigurationTypeDef,
         "MotionGraphicsConfiguration": MotionGraphicsConfigurationOutputTypeDef,
-        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
-        "ThumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "ThumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class EncoderSettingsOutputTypeDef(
     _RequiredEncoderSettingsOutputTypeDef, _OptionalEncoderSettingsOutputTypeDef
 ):
     pass
 
+
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": Sequence[VideoDescriptionTypeDef],
@@ -7207,17 +5923,19 @@
         "MotionGraphicsConfiguration": MotionGraphicsConfigurationTypeDef,
         "NielsenConfiguration": NielsenConfigurationTypeDef,
         "ThumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class EncoderSettingsTypeDef(_RequiredEncoderSettingsTypeDef, _OptionalEncoderSettingsTypeDef):
     pass
 
+
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
         "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 
@@ -7229,37 +5947,37 @@
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
         "ScheduleActions": List[ScheduleActionOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchScheduleActionCreateRequestTypeDef = TypedDict(
     "BatchScheduleActionCreateRequestTypeDef",
     {
         "ScheduleActions": Sequence[ScheduleActionTypeDef],
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
@@ -7269,107 +5987,107 @@
     total=False,
 )
 
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
         "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
         "InputAttachments": List[InputAttachmentOutputTypeDef],
-        "InputSpecification": InputSpecificationOutputTypeDef,
+        "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
@@ -7408,25 +6126,27 @@
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 BatchUpdateScheduleResponseTypeDef = TypedDict(
     "BatchUpdateScheduleResponseTypeDef",
     {
         "Creates": BatchScheduleActionCreateResultTypeDef,
         "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -7437,36 +6157,38 @@
     {
         "Creates": BatchScheduleActionCreateRequestTypeDef,
         "Deletes": BatchScheduleActionDeleteRequestTypeDef,
     },
     total=False,
 )
 
+
 class BatchUpdateScheduleRequestRequestTypeDef(
     _RequiredBatchUpdateScheduleRequestRequestTypeDef,
     _OptionalBatchUpdateScheduleRequestRequestTypeDef,
 ):
     pass
 
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelClassResponseTypeDef = TypedDict(
     "UpdateChannelClassResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.28.15/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-medialive
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaLive 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -674,93 +642,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
-    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
-    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
-    AccountConfigurationOutputTypeDef,
     AccountConfigurationTypeDef,
-    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
-    ArchiveS3SettingsOutputTypeDef,
     ArchiveS3SettingsTypeDef,
-    OutputLocationRefOutputTypeDef,
     OutputLocationRefTypeDef,
-    InputChannelLevelOutputTypeDef,
     InputChannelLevelTypeDef,
-    Eac3AtmosSettingsOutputTypeDef,
-    Eac3SettingsOutputTypeDef,
-    Mp2SettingsOutputTypeDef,
-    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     WavSettingsTypeDef,
-    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
-    AudioDolbyEDecodeOutputTypeDef,
     AudioDolbyEDecodeTypeDef,
-    AudioHlsRenditionSelectionOutputTypeDef,
     AudioHlsRenditionSelectionTypeDef,
-    AudioLanguageSelectionOutputTypeDef,
     AudioLanguageSelectionTypeDef,
-    InputLocationOutputTypeDef,
-    AudioPidSelectionOutputTypeDef,
+    InputLocationTypeDef,
     AudioPidSelectionTypeDef,
-    AudioSilenceFailoverSettingsOutputTypeDef,
     AudioSilenceFailoverSettingsTypeDef,
-    AudioTrackOutputTypeDef,
     AudioTrackTypeDef,
-    InputLocationTypeDef,
-    EsamOutputTypeDef,
-    Scte35SpliceInsertOutputTypeDef,
-    Scte35TimeSignalAposOutputTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
+    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
-    EbuTtDDestinationSettingsOutputTypeDef,
-    TtmlDestinationSettingsOutputTypeDef,
-    WebvttDestinationSettingsOutputTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
-    CaptionLanguageMappingOutputTypeDef,
     CaptionLanguageMappingTypeDef,
-    CaptionRectangleOutputTypeDef,
     CaptionRectangleTypeDef,
-    DvbSubSourceSettingsOutputTypeDef,
-    EmbeddedSourceSettingsOutputTypeDef,
-    Scte20SourceSettingsOutputTypeDef,
-    Scte27SourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     Scte20SourceSettingsTypeDef,
     Scte27SourceSettingsTypeDef,
-    CdiInputSpecificationOutputTypeDef,
     CdiInputSpecificationTypeDef,
     ChannelEgressEndpointTypeDef,
-    InputSpecificationOutputTypeDef,
+    InputSpecificationTypeDef,
     MaintenanceStatusTypeDef,
     VpcOutputSettingsDescriptionTypeDef,
     PipelineDetailTypeDef,
     ClaimDeviceRequestRequestTypeDef,
-    InputSpecificationTypeDef,
     MaintenanceCreateSettingsTypeDef,
     VpcOutputSettingsTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputVpcRequestTypeDef,
     MediaConnectFlowRequestTypeDef,
@@ -771,218 +707,155 @@
     DeleteChannelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DeleteInputSecurityGroupRequestRequestTypeDef,
     DeleteMultiplexProgramRequestRequestTypeDef,
     MultiplexProgramPacketIdentifiersMapTypeDef,
     MultiplexProgramPipelineDetailTypeDef,
     DeleteMultiplexRequestRequestTypeDef,
-    MultiplexSettingsOutputTypeDef,
     DeleteReservationRequestRequestTypeDef,
-    RenewalSettingsOutputTypeDef,
+    RenewalSettingsTypeDef,
     ReservationResourceSpecificationTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
-    InputDeviceSettingsOutputTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeThumbnailsRequestRequestTypeDef,
-    DvbNitSettingsOutputTypeDef,
-    DvbSdtSettingsOutputTypeDef,
-    DvbTdtSettingsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FeatureActivationsOutputTypeDef,
-    NielsenConfigurationOutputTypeDef,
-    ThumbnailConfigurationOutputTypeDef,
-    TimecodeConfigOutputTypeDef,
+    DvbNitSettingsTypeDef,
+    DvbSdtSettingsTypeDef,
+    DvbTdtSettingsTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     TimecodeConfigTypeDef,
-    InputLossFailoverSettingsOutputTypeDef,
-    VideoBlackFailoverSettingsOutputTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
-    FecOutputSettingsOutputTypeDef,
-    FixedModeScheduleActionStartSettingsOutputTypeDef,
+    FecOutputSettingsTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
-    Fmp4HlsSettingsOutputTypeDef,
-    FollowModeScheduleActionStartSettingsOutputTypeDef,
+    Fmp4HlsSettingsTypeDef,
     FollowModeScheduleActionStartSettingsTypeDef,
-    FrameCaptureS3SettingsOutputTypeDef,
     FrameCaptureS3SettingsTypeDef,
-    FrameCaptureOutputSettingsOutputTypeDef,
-    TimecodeBurninSettingsOutputTypeDef,
+    FrameCaptureOutputSettingsTypeDef,
     TimecodeBurninSettingsTypeDef,
     H264ColorSpaceSettingsOutputTypeDef,
     H264ColorSpaceSettingsTypeDef,
-    TemporalFilterSettingsOutputTypeDef,
     TemporalFilterSettingsTypeDef,
-    Hdr10SettingsOutputTypeDef,
     Hdr10SettingsTypeDef,
-    HlsAkamaiSettingsOutputTypeDef,
     HlsAkamaiSettingsTypeDef,
-    HlsBasicPutSettingsOutputTypeDef,
     HlsBasicPutSettingsTypeDef,
-    HlsMediaStoreSettingsOutputTypeDef,
-    HlsS3SettingsOutputTypeDef,
-    HlsWebdavSettingsOutputTypeDef,
     HlsMediaStoreSettingsTypeDef,
     HlsS3SettingsTypeDef,
     HlsWebdavSettingsTypeDef,
-    HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
     HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
-    HlsInputSettingsOutputTypeDef,
     HlsInputSettingsTypeDef,
-    HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
-    StartTimecodeOutputTypeDef,
-    StopTimecodeOutputTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    M3u8SettingsOutputTypeDef,
+    M3u8SettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
-    MediaPackageOutputDestinationSettingsOutputTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
-    MotionGraphicsActivateScheduleActionSettingsOutputTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
     MotionGraphicsSettingsOutputTypeDef,
     MotionGraphicsSettingsTypeDef,
-    MsSmoothOutputSettingsOutputTypeDef,
+    MsSmoothOutputSettingsTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
-    MultiplexProgramChannelDestinationSettingsOutputTypeDef,
     MultiplexProgramChannelDestinationSettingsTypeDef,
-    MultiplexProgramServiceDescriptorOutputTypeDef,
     MultiplexProgramServiceDescriptorTypeDef,
     MultiplexSettingsSummaryTypeDef,
-    MultiplexStatmuxVideoSettingsOutputTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
-    NielsenCBETOutputTypeDef,
     NielsenCBETTypeDef,
-    NielsenNaesIiNwOutputTypeDef,
     NielsenNaesIiNwTypeDef,
-    OutputDestinationSettingsOutputTypeDef,
     OutputDestinationSettingsTypeDef,
     RtmpGroupSettingsOutputTypeDef,
-    UdpGroupSettingsOutputTypeDef,
-    RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    PipelinePauseStateSettingsOutputTypeDef,
+    RtmpGroupSettingsTypeDef,
     PipelinePauseStateSettingsTypeDef,
-    RenewalSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    Scte35InputScheduleActionSettingsOutputTypeDef,
-    Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
-    Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
-    StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
-    Scte35DeliveryRestrictionsOutputTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
     StartMultiplexRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     StopMultiplexRequestRequestTypeDef,
     ThumbnailTypeDef,
     TransferInputDeviceRequestRequestTypeDef,
-    VideoSelectorPidOutputTypeDef,
     VideoSelectorPidTypeDef,
-    VideoSelectorProgramIdOutputTypeDef,
     VideoSelectorProgramIdTypeDef,
-    DescribeAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
-    ArchiveCdnSettingsOutputTypeDef,
     ArchiveCdnSettingsTypeDef,
-    MediaPackageGroupSettingsOutputTypeDef,
-    MsSmoothGroupSettingsOutputTypeDef,
-    MultiplexOutputSettingsOutputTypeDef,
-    RtmpOutputSettingsOutputTypeDef,
     MediaPackageGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    MultiplexOutputSettingsTypeDef,
+    RtmpOutputSettingsTypeDef,
     AudioChannelMappingOutputTypeDef,
     AudioChannelMappingTypeDef,
     AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
-    AudioOnlyHlsSettingsOutputTypeDef,
-    AvailBlankingOutputTypeDef,
-    BlackoutSlateOutputTypeDef,
-    BurnInDestinationSettingsOutputTypeDef,
-    DvbSubDestinationSettingsOutputTypeDef,
-    InputLossBehaviorOutputTypeDef,
-    StaticImageActivateScheduleActionSettingsOutputTypeDef,
-    StaticKeySettingsOutputTypeDef,
-    AudioTrackSelectionOutputTypeDef,
-    AudioTrackSelectionTypeDef,
+    AudioOnlyHlsSettingsTypeDef,
     AvailBlankingTypeDef,
     BlackoutSlateTypeDef,
     BurnInDestinationSettingsTypeDef,
     DvbSubDestinationSettingsTypeDef,
     InputLossBehaviorTypeDef,
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
-    AvailSettingsOutputTypeDef,
+    AudioTrackSelectionOutputTypeDef,
+    AudioTrackSelectionTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    TeletextSourceSettingsOutputTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
+    PurchaseOfferingRequestRequestTypeDef,
+    UpdateReservationRequestRequestTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     DescribeChannelRequestChannelCreatedWaitTypeDef,
     DescribeChannelRequestChannelDeletedWaitTypeDef,
@@ -996,160 +869,142 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    M2tsSettingsOutputTypeDef,
-    FailoverConditionSettingsOutputTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
+    M2tsSettingsTypeDef,
     FailoverConditionSettingsTypeDef,
     ScheduleActionStartSettingsOutputTypeDef,
     ScheduleActionStartSettingsTypeDef,
-    FrameCaptureCdnSettingsOutputTypeDef,
     FrameCaptureCdnSettingsTypeDef,
-    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
-    H264FilterSettingsOutputTypeDef,
-    H265FilterSettingsOutputTypeDef,
-    Mpeg2FilterSettingsOutputTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
     Mpeg2FilterSettingsTypeDef,
     H265ColorSpaceSettingsOutputTypeDef,
-    VideoSelectorColorSpaceSettingsOutputTypeDef,
     H265ColorSpaceSettingsTypeDef,
     VideoSelectorColorSpaceSettingsTypeDef,
-    HlsCdnSettingsOutputTypeDef,
     HlsCdnSettingsTypeDef,
-    NetworkInputSettingsOutputTypeDef,
     NetworkInputSettingsTypeDef,
-    InputClippingSettingsOutputTypeDef,
     InputClippingSettingsTypeDef,
     InputDestinationTypeDef,
     UpdateInputDeviceRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
-    StandardHlsSettingsOutputTypeDef,
+    StandardHlsSettingsTypeDef,
     MotionGraphicsConfigurationOutputTypeDef,
     MotionGraphicsConfigurationTypeDef,
     MultiplexOutputDestinationTypeDef,
     MultiplexSummaryTypeDef,
-    MultiplexVideoSettingsOutputTypeDef,
     MultiplexVideoSettingsTypeDef,
-    NielsenWatermarksSettingsOutputTypeDef,
     NielsenWatermarksSettingsTypeDef,
     OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
     PauseStateScheduleActionSettingsOutputTypeDef,
     PauseStateScheduleActionSettingsTypeDef,
-    PurchaseOfferingRequestRequestTypeDef,
-    UpdateReservationRequestRequestTypeDef,
-    Scte35SegmentationDescriptorOutputTypeDef,
     Scte35SegmentationDescriptorTypeDef,
     ThumbnailDetailTypeDef,
-    VideoSelectorSettingsOutputTypeDef,
     VideoSelectorSettingsTypeDef,
-    ArchiveGroupSettingsOutputTypeDef,
     ArchiveGroupSettingsTypeDef,
     RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
     CaptionDestinationSettingsOutputTypeDef,
-    GlobalConfigurationOutputTypeDef,
-    KeyProviderSettingsOutputTypeDef,
-    AudioSelectorSettingsOutputTypeDef,
-    AudioSelectorSettingsTypeDef,
     CaptionDestinationSettingsTypeDef,
     GlobalConfigurationTypeDef,
     KeyProviderSettingsTypeDef,
-    AvailConfigurationOutputTypeDef,
+    AudioSelectorSettingsOutputTypeDef,
+    AudioSelectorSettingsTypeDef,
     AvailConfigurationTypeDef,
     CaptionSelectorSettingsOutputTypeDef,
     CaptionSelectorSettingsTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     UpdateReservationResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
-    ArchiveContainerSettingsOutputTypeDef,
-    UdpContainerSettingsOutputTypeDef,
-    FailoverConditionOutputTypeDef,
+    ArchiveContainerSettingsTypeDef,
+    UdpContainerSettingsTypeDef,
     FailoverConditionTypeDef,
-    FrameCaptureGroupSettingsOutputTypeDef,
     FrameCaptureGroupSettingsTypeDef,
     H264SettingsOutputTypeDef,
-    Mpeg2SettingsOutputTypeDef,
     H264SettingsTypeDef,
     Mpeg2SettingsTypeDef,
     H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
     InputPrepareScheduleActionSettingsOutputTypeDef,
-    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputPrepareScheduleActionSettingsTypeDef,
+    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputSwitchScheduleActionSettingsTypeDef,
     DescribeInputResponseTypeDef,
     InputTypeDef,
-    HlsSettingsOutputTypeDef,
+    HlsSettingsTypeDef,
     DeleteMultiplexResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
-    MultiplexProgramSettingsOutputTypeDef,
     MultiplexProgramSettingsTypeDef,
-    AudioWatermarkSettingsOutputTypeDef,
     AudioWatermarkSettingsTypeDef,
     UpdateChannelClassRequestRequestTypeDef,
-    Scte35DescriptorSettingsOutputTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
-    VideoSelectorOutputTypeDef,
     VideoSelectorTypeDef,
     CaptionDescriptionOutputTypeDef,
+    CaptionDescriptionTypeDef,
     HlsGroupSettingsOutputTypeDef,
+    HlsGroupSettingsTypeDef,
     AudioSelectorOutputTypeDef,
     AudioSelectorTypeDef,
-    CaptionDescriptionTypeDef,
-    HlsGroupSettingsTypeDef,
     CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
-    ArchiveOutputSettingsOutputTypeDef,
-    UdpOutputSettingsOutputTypeDef,
+    ArchiveOutputSettingsTypeDef,
+    UdpOutputSettingsTypeDef,
     AutomaticInputFailoverSettingsOutputTypeDef,
     AutomaticInputFailoverSettingsTypeDef,
     VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     CreateInputResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     ListInputsResponseTypeDef,
     UpdateInputResponseTypeDef,
-    HlsOutputSettingsOutputTypeDef,
+    HlsOutputSettingsTypeDef,
     CreateMultiplexResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
+    CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
-    CreateMultiplexProgramRequestRequestTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
-    Scte35DescriptorOutputTypeDef,
     Scte35DescriptorTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
-    OutputSettingsOutputTypeDef,
+    OutputSettingsTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
     Scte35TimeSignalScheduleActionSettingsTypeDef,
     InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
@@ -1178,15 +1033,15 @@
     BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsOutputTypeDef:
+def get_structure() -> AacSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.12/setup.py` & `mypy-boto3-medialive-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaLive 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

