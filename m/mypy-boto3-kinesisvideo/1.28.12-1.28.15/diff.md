# Comparing `tmp/mypy-boto3-kinesisvideo-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.12.tar", last modified: Thu Jul 27 05:34:54 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.15.tar", last modified: Fri Jul 28 20:43:06 2023, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.28.12.tar` & `mypy-boto3-kinesisvideo-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33223 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33176 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:06.025347 mypy-boto3-kinesisvideo-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-28 20:43:06.021347 mypy-boto3-kinesisvideo-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:06.013347 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:06.021347 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:06.025347 mypy-boto3-kinesisvideo-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/LICENSE` & `mypy-boto3-kinesisvideo-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideo 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,109 +353,97 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
-    SingleMasterConfigurationOutputTypeDef,
-    ChannelNameConditionTypeDef,
     SingleMasterConfigurationTypeDef,
+    ChannelNameConditionTypeDef,
     TagTypeDef,
-    CreateSignalingChannelOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
-    CreateStreamOutputTypeDef,
     DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
-    LocalSizeConfigOutputTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationOutputTypeDef,
+    MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     LastRecorderStatusTypeDef,
     LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
-    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
-    ImageGenerationDestinationConfigOutputTypeDef,
     ImageGenerationDestinationConfigTypeDef,
-    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
-    ListTagsForStreamOutputTypeDef,
-    MediaSourceConfigOutputTypeDef,
     MediaSourceConfigTypeDef,
-    MediaStorageConfigurationTypeDef,
-    NotificationDestinationConfigOutputTypeDef,
     NotificationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ScheduleConfigOutputTypeDef,
     ScheduleConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
-    ListSignalingChannelsInputRequestTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
+    ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    DeletionConfigOutputTypeDef,
+    CreateSignalingChannelOutputTypeDef,
+    CreateStreamOutputTypeDef,
+    GetDataEndpointOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
-    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
-    RecorderConfigOutputTypeDef,
-    UploaderConfigOutputTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
-    EdgeConfigOutputTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
-    StartEdgeConfigurationUpdateOutputTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
+    StartEdgeConfigurationUpdateOutputTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationOutputTypeDef:
+def get_structure() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/README.md` & `mypy-boto3-kinesisvideo-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,109 +321,97 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
-    SingleMasterConfigurationOutputTypeDef,
-    ChannelNameConditionTypeDef,
     SingleMasterConfigurationTypeDef,
+    ChannelNameConditionTypeDef,
     TagTypeDef,
-    CreateSignalingChannelOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
-    CreateStreamOutputTypeDef,
     DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
-    LocalSizeConfigOutputTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationOutputTypeDef,
+    MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     LastRecorderStatusTypeDef,
     LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
-    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
-    ImageGenerationDestinationConfigOutputTypeDef,
     ImageGenerationDestinationConfigTypeDef,
-    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
-    ListTagsForStreamOutputTypeDef,
-    MediaSourceConfigOutputTypeDef,
     MediaSourceConfigTypeDef,
-    MediaStorageConfigurationTypeDef,
-    NotificationDestinationConfigOutputTypeDef,
     NotificationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ScheduleConfigOutputTypeDef,
     ScheduleConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
-    ListSignalingChannelsInputRequestTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
+    ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    DeletionConfigOutputTypeDef,
+    CreateSignalingChannelOutputTypeDef,
+    CreateStreamOutputTypeDef,
+    GetDataEndpointOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
-    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
-    RecorderConfigOutputTypeDef,
-    UploaderConfigOutputTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
-    EdgeConfigOutputTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
-    StartEdgeConfigurationUpdateOutputTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
+    StartEdgeConfigurationUpdateOutputTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationOutputTypeDef:
+def get_structure() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.py` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.pyi` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideo 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.py` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,30 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 
 class ListEdgeAgentConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
     """
 
     def paginate(
-        self, *, HubDeviceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HubDeviceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEdgeAgentConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
         """
 
 
@@ -97,15 +97,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 
@@ -115,13 +115,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.pyi` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,29 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 class ListEdgeAgentConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
     """
 
     def paginate(
-        self, *, HubDeviceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HubDeviceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEdgeAgentConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
         """
 
 class ListSignalingChannelsPaginator(Paginator):
@@ -92,15 +92,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 class ListStreamsPaginator(Paginator):
@@ -109,13 +109,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesisvideo service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationOutputTypeDef
+    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
-    data: SingleMasterConfigurationOutputTypeDef = {...}
+    data: SingleMasterConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -40,109 +40,97 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "SingleMasterConfigurationOutputTypeDef",
-    "ChannelNameConditionTypeDef",
     "SingleMasterConfigurationTypeDef",
+    "ChannelNameConditionTypeDef",
     "TagTypeDef",
-    "CreateSignalingChannelOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
-    "CreateStreamOutputTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
-    "LocalSizeConfigOutputTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
-    "MediaStorageConfigurationOutputTypeDef",
+    "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "LastRecorderStatusTypeDef",
     "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
-    "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
-    "ImageGenerationDestinationConfigOutputTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
-    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
-    "ListTagsForStreamOutputTypeDef",
-    "MediaSourceConfigOutputTypeDef",
     "MediaSourceConfigTypeDef",
-    "MediaStorageConfigurationTypeDef",
-    "NotificationDestinationConfigOutputTypeDef",
     "NotificationDestinationConfigTypeDef",
-    "PaginatorConfigTypeDef",
-    "ScheduleConfigOutputTypeDef",
     "ScheduleConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    "ListSignalingChannelsInputRequestTypeDef",
     "UpdateSignalingChannelInputRequestTypeDef",
+    "ListSignalingChannelsInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "DeletionConfigOutputTypeDef",
+    "CreateSignalingChannelOutputTypeDef",
+    "CreateStreamOutputTypeDef",
+    "GetDataEndpointOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
     "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
-    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
-    "RecorderConfigOutputTypeDef",
-    "UploaderConfigOutputTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
-    "EdgeConfigOutputTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
-    "StartEdgeConfigurationUpdateOutputTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
+    "StartEdgeConfigurationUpdateOutputTypeDef",
     "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
-SingleMasterConfigurationOutputTypeDef = TypedDict(
-    "SingleMasterConfigurationOutputTypeDef",
+SingleMasterConfigurationTypeDef = TypedDict(
+    "SingleMasterConfigurationTypeDef",
     {
         "MessageTtlSeconds": int,
     },
     total=False,
 )
 
 ChannelNameConditionTypeDef = TypedDict(
@@ -150,35 +138,30 @@
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
 )
 
-SingleMasterConfigurationTypeDef = TypedDict(
-    "SingleMasterConfigurationTypeDef",
-    {
-        "MessageTtlSeconds": int,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateSignalingChannelOutputTypeDef = TypedDict(
-    "CreateSignalingChannelOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChannelARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
@@ -199,22 +182,14 @@
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
 
-CreateStreamOutputTypeDef = TypedDict(
-    "CreateStreamOutputTypeDef",
-    {
-        "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
     "DeleteEdgeConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -259,23 +234,14 @@
 
 class DeleteStreamInputRequestTypeDef(
     _RequiredDeleteStreamInputRequestTypeDef, _OptionalDeleteStreamInputRequestTypeDef
 ):
     pass
 
 
-LocalSizeConfigOutputTypeDef = TypedDict(
-    "LocalSizeConfigOutputTypeDef",
-    {
-        "MaxLocalMediaSizeInMB": int,
-        "StrategyOnFullSize": StrategyOnFullSizeType,
-    },
-    total=False,
-)
-
 LocalSizeConfigTypeDef = TypedDict(
     "LocalSizeConfigTypeDef",
     {
         "MaxLocalMediaSizeInMB": int,
         "StrategyOnFullSize": StrategyOnFullSizeType,
     },
     total=False,
@@ -295,20 +261,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     {
@@ -334,31 +300,31 @@
     {
         "ChannelName": str,
         "ChannelARN": str,
     },
     total=False,
 )
 
-_RequiredMediaStorageConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMediaStorageConfigurationOutputTypeDef",
+_RequiredMediaStorageConfigurationTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationTypeDef",
     {
         "Status": MediaStorageConfigurationStatusType,
     },
 )
-_OptionalMediaStorageConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMediaStorageConfigurationOutputTypeDef",
+_OptionalMediaStorageConfigurationTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationTypeDef",
     {
         "StreamARN": str,
     },
     total=False,
 )
 
 
-class MediaStorageConfigurationOutputTypeDef(
-    _RequiredMediaStorageConfigurationOutputTypeDef, _OptionalMediaStorageConfigurationOutputTypeDef
+class MediaStorageConfigurationTypeDef(
+    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
 ):
     pass
 
 
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
@@ -442,22 +408,14 @@
 
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
 
-GetDataEndpointOutputTypeDef = TypedDict(
-    "GetDataEndpointOutputTypeDef",
-    {
-        "DataEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -468,52 +426,22 @@
     {
         "Protocol": ChannelProtocolType,
         "ResourceEndpoint": str,
     },
     total=False,
 )
 
-ImageGenerationDestinationConfigOutputTypeDef = TypedDict(
-    "ImageGenerationDestinationConfigOutputTypeDef",
-    {
-        "Uri": str,
-        "DestinationRegion": str,
-    },
-)
-
 ImageGenerationDestinationConfigTypeDef = TypedDict(
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
-_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
-    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
-    {
-        "HubDeviceArn": str,
-    },
-)
-_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
-    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
-    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
-    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
     "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
     {
         "HubDeviceArn": str,
     },
 )
 _OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
@@ -559,130 +487,47 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MediaSourceConfigOutputTypeDef = TypedDict(
-    "MediaSourceConfigOutputTypeDef",
-    {
-        "MediaUriSecretArn": str,
-        "MediaUriType": MediaUriTypeType,
-    },
-)
-
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
 
-_RequiredMediaStorageConfigurationTypeDef = TypedDict(
-    "_RequiredMediaStorageConfigurationTypeDef",
-    {
-        "Status": MediaStorageConfigurationStatusType,
-    },
-)
-_OptionalMediaStorageConfigurationTypeDef = TypedDict(
-    "_OptionalMediaStorageConfigurationTypeDef",
-    {
-        "StreamARN": str,
-    },
-    total=False,
-)
-
-
-class MediaStorageConfigurationTypeDef(
-    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
-):
-    pass
-
-
-NotificationDestinationConfigOutputTypeDef = TypedDict(
-    "NotificationDestinationConfigOutputTypeDef",
-    {
-        "Uri": str,
-    },
-)
-
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
     },
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
-ScheduleConfigOutputTypeDef = TypedDict(
-    "ScheduleConfigOutputTypeDef",
-    {
-        "ScheduleExpression": str,
-        "DurationInSeconds": int,
-    },
-)
-
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
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
 _RequiredTagStreamInputRequestTypeDef = TypedDict(
     "_RequiredTagStreamInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
 )
 _OptionalTagStreamInputRequestTypeDef = TypedDict(
@@ -783,39 +628,20 @@
     "ChannelInfoTypeDef",
     {
         "ChannelName": str,
         "ChannelARN": str,
         "ChannelType": ChannelTypeType,
         "ChannelStatus": StatusType,
         "CreationTime": datetime,
-        "SingleMasterConfiguration": SingleMasterConfigurationOutputTypeDef,
+        "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
         "Version": str,
     },
     total=False,
 )
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSignalingChannelsInputRequestTypeDef = TypedDict(
-    "ListSignalingChannelsInputRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
         "CurrentVersion": str,
     },
 )
@@ -831,14 +657,24 @@
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
 
+ListSignalingChannelsInputRequestTypeDef = TypedDict(
+    "ListSignalingChannelsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredCreateSignalingChannelInputRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalCreateSignalingChannelInputRequestTypeDef = TypedDict(
@@ -863,65 +699,146 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DeletionConfigOutputTypeDef = TypedDict(
-    "DeletionConfigOutputTypeDef",
+CreateSignalingChannelOutputTypeDef = TypedDict(
+    "CreateSignalingChannelOutputTypeDef",
     {
-        "EdgeRetentionInHours": int,
-        "LocalSizeConfig": LocalSizeConfigOutputTypeDef,
-        "DeleteAfterUpload": bool,
+        "ChannelARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamOutputTypeDef = TypedDict(
+    "CreateStreamOutputTypeDef",
+    {
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataEndpointOutputTypeDef = TypedDict(
+    "GetDataEndpointOutputTypeDef",
+    {
+        "DataEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+):
+    pass
+
+
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationOutputTypeDef",
     {
         "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
-        "MediaStorageConfiguration": MediaStorageConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelARN": str,
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
     },
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EdgeAgentStatusTypeDef = TypedDict(
     "EdgeAgentStatusTypeDef",
     {
         "LastRecorderStatus": LastRecorderStatusTypeDef,
@@ -952,24 +869,24 @@
     pass
 
 
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationOutputTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
-        "DestinationConfig": ImageGenerationDestinationConfigOutputTypeDef,
+        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationOutputTypeDef",
     {
@@ -1015,81 +932,37 @@
     pass
 
 
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "StreamNameCondition": StreamNameConditionTypeDef,
     },
     total=False,
 )
 
-UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
-    {
-        "ChannelARN": str,
-        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-    },
-)
-
-NotificationConfigurationOutputTypeDef = TypedDict(
-    "NotificationConfigurationOutputTypeDef",
-    {
-        "Status": ConfigurationStatusType,
-        "DestinationConfig": NotificationDestinationConfigOutputTypeDef,
-    },
-)
-
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "DestinationConfig": NotificationDestinationConfigTypeDef,
     },
 )
 
-_RequiredRecorderConfigOutputTypeDef = TypedDict(
-    "_RequiredRecorderConfigOutputTypeDef",
-    {
-        "MediaSourceConfig": MediaSourceConfigOutputTypeDef,
-    },
-)
-_OptionalRecorderConfigOutputTypeDef = TypedDict(
-    "_OptionalRecorderConfigOutputTypeDef",
-    {
-        "ScheduleConfig": ScheduleConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RecorderConfigOutputTypeDef(
-    _RequiredRecorderConfigOutputTypeDef, _OptionalRecorderConfigOutputTypeDef
-):
-    pass
-
-
-UploaderConfigOutputTypeDef = TypedDict(
-    "UploaderConfigOutputTypeDef",
-    {
-        "ScheduleConfig": ScheduleConfigOutputTypeDef,
-    },
-)
-
 _RequiredRecorderConfigTypeDef = TypedDict(
     "_RequiredRecorderConfigTypeDef",
     {
         "MediaSourceConfig": MediaSourceConfigTypeDef,
     },
 )
 _OptionalRecorderConfigTypeDef = TypedDict(
@@ -1112,32 +985,32 @@
     },
 )
 
 DescribeSignalingChannelOutputTypeDef = TypedDict(
     "DescribeSignalingChannelOutputTypeDef",
     {
         "ChannelInfo": ChannelInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalingChannelsOutputTypeDef = TypedDict(
     "ListSignalingChannelsOutputTypeDef",
     {
         "ChannelInfoList": List[ChannelInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
         "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -1146,50 +1019,29 @@
     },
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredEdgeConfigOutputTypeDef = TypedDict(
-    "_RequiredEdgeConfigOutputTypeDef",
-    {
-        "HubDeviceArn": str,
-        "RecorderConfig": RecorderConfigOutputTypeDef,
-    },
-)
-_OptionalEdgeConfigOutputTypeDef = TypedDict(
-    "_OptionalEdgeConfigOutputTypeDef",
-    {
-        "UploaderConfig": UploaderConfigOutputTypeDef,
-        "DeletionConfig": DeletionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EdgeConfigOutputTypeDef(_RequiredEdgeConfigOutputTypeDef, _OptionalEdgeConfigOutputTypeDef):
-    pass
-
-
 _RequiredEdgeConfigTypeDef = TypedDict(
     "_RequiredEdgeConfigTypeDef",
     {
         "HubDeviceArn": str,
         "RecorderConfig": RecorderConfigTypeDef,
     },
 )
@@ -1212,48 +1064,34 @@
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigOutputTypeDef,
+        "EdgeConfig": EdgeConfigTypeDef,
         "EdgeAgentStatus": EdgeAgentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigOutputTypeDef,
+        "EdgeConfig": EdgeConfigTypeDef,
     },
     total=False,
 )
 
-StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
-    "StartEdgeConfigurationUpdateOutputTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "SyncStatus": SyncStatusType,
-        "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -1269,15 +1107,29 @@
 class StartEdgeConfigurationUpdateInputRequestTypeDef(
     _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef,
     _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef,
 ):
     pass
 
 
+StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
+    "StartEdgeConfigurationUpdateOutputTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsOutputTypeDef",
     {
         "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesisvideo service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationOutputTypeDef
+    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
-    data: SingleMasterConfigurationOutputTypeDef = {...}
+    data: SingleMasterConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -39,109 +39,97 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "SingleMasterConfigurationOutputTypeDef",
-    "ChannelNameConditionTypeDef",
     "SingleMasterConfigurationTypeDef",
+    "ChannelNameConditionTypeDef",
     "TagTypeDef",
-    "CreateSignalingChannelOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
-    "CreateStreamOutputTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
-    "LocalSizeConfigOutputTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
-    "MediaStorageConfigurationOutputTypeDef",
+    "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "LastRecorderStatusTypeDef",
     "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
-    "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
-    "ImageGenerationDestinationConfigOutputTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
-    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
-    "ListTagsForStreamOutputTypeDef",
-    "MediaSourceConfigOutputTypeDef",
     "MediaSourceConfigTypeDef",
-    "MediaStorageConfigurationTypeDef",
-    "NotificationDestinationConfigOutputTypeDef",
     "NotificationDestinationConfigTypeDef",
-    "PaginatorConfigTypeDef",
-    "ScheduleConfigOutputTypeDef",
     "ScheduleConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    "ListSignalingChannelsInputRequestTypeDef",
     "UpdateSignalingChannelInputRequestTypeDef",
+    "ListSignalingChannelsInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "DeletionConfigOutputTypeDef",
+    "CreateSignalingChannelOutputTypeDef",
+    "CreateStreamOutputTypeDef",
+    "GetDataEndpointOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
     "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
-    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
-    "RecorderConfigOutputTypeDef",
-    "UploaderConfigOutputTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
-    "EdgeConfigOutputTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
-    "StartEdgeConfigurationUpdateOutputTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
+    "StartEdgeConfigurationUpdateOutputTypeDef",
     "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
-SingleMasterConfigurationOutputTypeDef = TypedDict(
-    "SingleMasterConfigurationOutputTypeDef",
+SingleMasterConfigurationTypeDef = TypedDict(
+    "SingleMasterConfigurationTypeDef",
     {
         "MessageTtlSeconds": int,
     },
     total=False,
 )
 
 ChannelNameConditionTypeDef = TypedDict(
@@ -149,35 +137,30 @@
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
 )
 
-SingleMasterConfigurationTypeDef = TypedDict(
-    "SingleMasterConfigurationTypeDef",
-    {
-        "MessageTtlSeconds": int,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateSignalingChannelOutputTypeDef = TypedDict(
-    "CreateSignalingChannelOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChannelARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
@@ -196,22 +179,14 @@
 )
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
-CreateStreamOutputTypeDef = TypedDict(
-    "CreateStreamOutputTypeDef",
-    {
-        "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
     "DeleteEdgeConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -252,23 +227,14 @@
 )
 
 class DeleteStreamInputRequestTypeDef(
     _RequiredDeleteStreamInputRequestTypeDef, _OptionalDeleteStreamInputRequestTypeDef
 ):
     pass
 
-LocalSizeConfigOutputTypeDef = TypedDict(
-    "LocalSizeConfigOutputTypeDef",
-    {
-        "MaxLocalMediaSizeInMB": int,
-        "StrategyOnFullSize": StrategyOnFullSizeType,
-    },
-    total=False,
-)
-
 LocalSizeConfigTypeDef = TypedDict(
     "LocalSizeConfigTypeDef",
     {
         "MaxLocalMediaSizeInMB": int,
         "StrategyOnFullSize": StrategyOnFullSizeType,
     },
     total=False,
@@ -288,20 +254,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     {
@@ -327,30 +293,30 @@
     {
         "ChannelName": str,
         "ChannelARN": str,
     },
     total=False,
 )
 
-_RequiredMediaStorageConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMediaStorageConfigurationOutputTypeDef",
+_RequiredMediaStorageConfigurationTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationTypeDef",
     {
         "Status": MediaStorageConfigurationStatusType,
     },
 )
-_OptionalMediaStorageConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMediaStorageConfigurationOutputTypeDef",
+_OptionalMediaStorageConfigurationTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationTypeDef",
     {
         "StreamARN": str,
     },
     total=False,
 )
 
-class MediaStorageConfigurationOutputTypeDef(
-    _RequiredMediaStorageConfigurationOutputTypeDef, _OptionalMediaStorageConfigurationOutputTypeDef
+class MediaStorageConfigurationTypeDef(
+    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
 ):
     pass
 
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -431,22 +397,14 @@
 )
 
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
-GetDataEndpointOutputTypeDef = TypedDict(
-    "GetDataEndpointOutputTypeDef",
-    {
-        "DataEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -457,50 +415,22 @@
     {
         "Protocol": ChannelProtocolType,
         "ResourceEndpoint": str,
     },
     total=False,
 )
 
-ImageGenerationDestinationConfigOutputTypeDef = TypedDict(
-    "ImageGenerationDestinationConfigOutputTypeDef",
-    {
-        "Uri": str,
-        "DestinationRegion": str,
-    },
-)
-
 ImageGenerationDestinationConfigTypeDef = TypedDict(
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
-_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
-    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
-    {
-        "HubDeviceArn": str,
-    },
-)
-_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
-    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
-    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
-    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
     "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
     {
         "HubDeviceArn": str,
     },
 )
 _OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
@@ -542,128 +472,47 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MediaSourceConfigOutputTypeDef = TypedDict(
-    "MediaSourceConfigOutputTypeDef",
-    {
-        "MediaUriSecretArn": str,
-        "MediaUriType": MediaUriTypeType,
-    },
-)
-
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
 
-_RequiredMediaStorageConfigurationTypeDef = TypedDict(
-    "_RequiredMediaStorageConfigurationTypeDef",
-    {
-        "Status": MediaStorageConfigurationStatusType,
-    },
-)
-_OptionalMediaStorageConfigurationTypeDef = TypedDict(
-    "_OptionalMediaStorageConfigurationTypeDef",
-    {
-        "StreamARN": str,
-    },
-    total=False,
-)
-
-class MediaStorageConfigurationTypeDef(
-    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
-):
-    pass
-
-NotificationDestinationConfigOutputTypeDef = TypedDict(
-    "NotificationDestinationConfigOutputTypeDef",
-    {
-        "Uri": str,
-    },
-)
-
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
     },
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
-ScheduleConfigOutputTypeDef = TypedDict(
-    "ScheduleConfigOutputTypeDef",
-    {
-        "ScheduleExpression": str,
-        "DurationInSeconds": int,
-    },
-)
-
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
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
 _RequiredTagStreamInputRequestTypeDef = TypedDict(
     "_RequiredTagStreamInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
 )
 _OptionalTagStreamInputRequestTypeDef = TypedDict(
@@ -756,39 +605,20 @@
     "ChannelInfoTypeDef",
     {
         "ChannelName": str,
         "ChannelARN": str,
         "ChannelType": ChannelTypeType,
         "ChannelStatus": StatusType,
         "CreationTime": datetime,
-        "SingleMasterConfiguration": SingleMasterConfigurationOutputTypeDef,
+        "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
         "Version": str,
     },
     total=False,
 )
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSignalingChannelsInputRequestTypeDef = TypedDict(
-    "ListSignalingChannelsInputRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
         "CurrentVersion": str,
     },
 )
@@ -802,14 +632,24 @@
 
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+ListSignalingChannelsInputRequestTypeDef = TypedDict(
+    "ListSignalingChannelsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredCreateSignalingChannelInputRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalCreateSignalingChannelInputRequestTypeDef = TypedDict(
@@ -832,65 +672,144 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DeletionConfigOutputTypeDef = TypedDict(
-    "DeletionConfigOutputTypeDef",
+CreateSignalingChannelOutputTypeDef = TypedDict(
+    "CreateSignalingChannelOutputTypeDef",
     {
-        "EdgeRetentionInHours": int,
-        "LocalSizeConfig": LocalSizeConfigOutputTypeDef,
-        "DeleteAfterUpload": bool,
+        "ChannelARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamOutputTypeDef = TypedDict(
+    "CreateStreamOutputTypeDef",
+    {
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataEndpointOutputTypeDef = TypedDict(
+    "GetDataEndpointOutputTypeDef",
+    {
+        "DataEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+):
+    pass
+
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationOutputTypeDef",
     {
         "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
-        "MediaStorageConfiguration": MediaStorageConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelARN": str,
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
     },
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EdgeAgentStatusTypeDef = TypedDict(
     "EdgeAgentStatusTypeDef",
     {
         "LastRecorderStatus": LastRecorderStatusTypeDef,
@@ -919,24 +838,24 @@
 ):
     pass
 
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationOutputTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
-        "DestinationConfig": ImageGenerationDestinationConfigOutputTypeDef,
+        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationOutputTypeDef",
     {
@@ -978,79 +897,37 @@
 ):
     pass
 
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "StreamNameCondition": StreamNameConditionTypeDef,
     },
     total=False,
 )
 
-UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
-    {
-        "ChannelARN": str,
-        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-    },
-)
-
-NotificationConfigurationOutputTypeDef = TypedDict(
-    "NotificationConfigurationOutputTypeDef",
-    {
-        "Status": ConfigurationStatusType,
-        "DestinationConfig": NotificationDestinationConfigOutputTypeDef,
-    },
-)
-
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "DestinationConfig": NotificationDestinationConfigTypeDef,
     },
 )
 
-_RequiredRecorderConfigOutputTypeDef = TypedDict(
-    "_RequiredRecorderConfigOutputTypeDef",
-    {
-        "MediaSourceConfig": MediaSourceConfigOutputTypeDef,
-    },
-)
-_OptionalRecorderConfigOutputTypeDef = TypedDict(
-    "_OptionalRecorderConfigOutputTypeDef",
-    {
-        "ScheduleConfig": ScheduleConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class RecorderConfigOutputTypeDef(
-    _RequiredRecorderConfigOutputTypeDef, _OptionalRecorderConfigOutputTypeDef
-):
-    pass
-
-UploaderConfigOutputTypeDef = TypedDict(
-    "UploaderConfigOutputTypeDef",
-    {
-        "ScheduleConfig": ScheduleConfigOutputTypeDef,
-    },
-)
-
 _RequiredRecorderConfigTypeDef = TypedDict(
     "_RequiredRecorderConfigTypeDef",
     {
         "MediaSourceConfig": MediaSourceConfigTypeDef,
     },
 )
 _OptionalRecorderConfigTypeDef = TypedDict(
@@ -1071,32 +948,32 @@
     },
 )
 
 DescribeSignalingChannelOutputTypeDef = TypedDict(
     "DescribeSignalingChannelOutputTypeDef",
     {
         "ChannelInfo": ChannelInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalingChannelsOutputTypeDef = TypedDict(
     "ListSignalingChannelsOutputTypeDef",
     {
         "ChannelInfoList": List[ChannelInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
         "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -1105,48 +982,29 @@
     },
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredEdgeConfigOutputTypeDef = TypedDict(
-    "_RequiredEdgeConfigOutputTypeDef",
-    {
-        "HubDeviceArn": str,
-        "RecorderConfig": RecorderConfigOutputTypeDef,
-    },
-)
-_OptionalEdgeConfigOutputTypeDef = TypedDict(
-    "_OptionalEdgeConfigOutputTypeDef",
-    {
-        "UploaderConfig": UploaderConfigOutputTypeDef,
-        "DeletionConfig": DeletionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class EdgeConfigOutputTypeDef(_RequiredEdgeConfigOutputTypeDef, _OptionalEdgeConfigOutputTypeDef):
-    pass
-
 _RequiredEdgeConfigTypeDef = TypedDict(
     "_RequiredEdgeConfigTypeDef",
     {
         "HubDeviceArn": str,
         "RecorderConfig": RecorderConfigTypeDef,
     },
 )
@@ -1167,48 +1025,34 @@
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigOutputTypeDef,
+        "EdgeConfig": EdgeConfigTypeDef,
         "EdgeAgentStatus": EdgeAgentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigOutputTypeDef,
+        "EdgeConfig": EdgeConfigTypeDef,
     },
     total=False,
 )
 
-StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
-    "StartEdgeConfigurationUpdateOutputTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "SyncStatus": SyncStatusType,
-        "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -1222,15 +1066,29 @@
 
 class StartEdgeConfigurationUpdateInputRequestTypeDef(
     _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef,
     _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef,
 ):
     pass
 
+StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
+    "StartEdgeConfigurationUpdateOutputTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsOutputTypeDef",
     {
         "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideo 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,109 +353,97 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
-    SingleMasterConfigurationOutputTypeDef,
-    ChannelNameConditionTypeDef,
     SingleMasterConfigurationTypeDef,
+    ChannelNameConditionTypeDef,
     TagTypeDef,
-    CreateSignalingChannelOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
-    CreateStreamOutputTypeDef,
     DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
-    LocalSizeConfigOutputTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationOutputTypeDef,
+    MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     LastRecorderStatusTypeDef,
     LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
-    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
-    ImageGenerationDestinationConfigOutputTypeDef,
     ImageGenerationDestinationConfigTypeDef,
-    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
-    ListTagsForStreamOutputTypeDef,
-    MediaSourceConfigOutputTypeDef,
     MediaSourceConfigTypeDef,
-    MediaStorageConfigurationTypeDef,
-    NotificationDestinationConfigOutputTypeDef,
     NotificationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ScheduleConfigOutputTypeDef,
     ScheduleConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
-    ListSignalingChannelsInputRequestTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
+    ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    DeletionConfigOutputTypeDef,
+    CreateSignalingChannelOutputTypeDef,
+    CreateStreamOutputTypeDef,
+    GetDataEndpointOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
-    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
-    RecorderConfigOutputTypeDef,
-    UploaderConfigOutputTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
-    EdgeConfigOutputTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
-    StartEdgeConfigurationUpdateOutputTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
+    StartEdgeConfigurationUpdateOutputTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationOutputTypeDef:
+def get_structure() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.12/setup.py` & `mypy-boto3-kinesisvideo-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideo 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

