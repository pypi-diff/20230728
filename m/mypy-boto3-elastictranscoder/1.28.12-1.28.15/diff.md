# Comparing `tmp/mypy-boto3-elastictranscoder-1.28.12.tar.gz` & `tmp/mypy-boto3-elastictranscoder-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastictranscoder-1.28.12.tar", last modified: Thu Jul 27 05:34:39 2023, max compression
+gzip compressed data, was "mypy-boto3-elastictranscoder-1.28.15.tar", last modified: Fri Jul 28 20:42:44 2023, max compression
```

## Comparing `mypy-boto3-elastictranscoder-1.28.12.tar` & `mypy-boto3-elastictranscoder-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.104519 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29436 2023-07-27 05:21:52.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:44.133046 mypy-boto3-elastictranscoder-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-07-28 20:42:44.133046 mypy-boto3-elastictranscoder-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:44.133046 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-07-28 20:25:17.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25094 2023-07-28 20:25:17.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:44.133046 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-07-28 20:42:43.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 20:42:43.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:43.000000 mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:44.133046 mypy-boto3-elastictranscoder-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-28 20:25:16.000000 mypy-boto3-elastictranscoder-1.28.15/setup.py
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/LICENSE` & `mypy-boto3-elastictranscoder-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/PKG-INFO` & `mypy-boto3-elastictranscoder-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticTranscoder 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticTranscoder 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,90 +358,75 @@
 ### Typed dictionaries
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
-    EncryptionOutputTypeDef,
     EncryptionTypeDef,
-    AudioCodecOptionsOutputTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
-    TimeSpanOutputTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
-    DetectedPropertiesOutputTypeDef,
     DetectedPropertiesTypeDef,
-    HlsContentProtectionOutputTypeDef,
     TimingTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    NotificationsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PermissionOutputTypeDef,
     PermissionTypeDef,
-    PlayReadyDrmOutputTypeDef,
-    ThumbnailsOutputTypeDef,
-    PresetWatermarkOutputTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
-    ArtworkOutputTypeDef,
-    CaptionFormatOutputTypeDef,
-    CaptionSourceOutputTypeDef,
-    JobWatermarkOutputTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
-    AudioParametersOutputTypeDef,
     AudioParametersTypeDef,
-    ClipOutputTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
+    PlaylistTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
-    PlaylistTypeDef,
     VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
     JobAlbumArtOutputTypeDef,
-    CaptionsOutputTypeDef,
-    InputCaptionsOutputTypeDef,
     JobAlbumArtTypeDef,
+    CaptionsOutputTypeDef,
     CaptionsTypeDef,
+    InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
     JobOutputTypeDef,
-    JobInputOutputTypeDef,
     CreateJobOutputTypeDef,
+    JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
@@ -453,15 +438,15 @@
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
 )
 
 
-def get_structure() -> EncryptionOutputTypeDef:
+def get_structure() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/README.md` & `mypy-boto3-elastictranscoder-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,90 +326,75 @@
 ### Typed dictionaries
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
-    EncryptionOutputTypeDef,
     EncryptionTypeDef,
-    AudioCodecOptionsOutputTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
-    TimeSpanOutputTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
-    DetectedPropertiesOutputTypeDef,
     DetectedPropertiesTypeDef,
-    HlsContentProtectionOutputTypeDef,
     TimingTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    NotificationsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PermissionOutputTypeDef,
     PermissionTypeDef,
-    PlayReadyDrmOutputTypeDef,
-    ThumbnailsOutputTypeDef,
-    PresetWatermarkOutputTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
-    ArtworkOutputTypeDef,
-    CaptionFormatOutputTypeDef,
-    CaptionSourceOutputTypeDef,
-    JobWatermarkOutputTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
-    AudioParametersOutputTypeDef,
     AudioParametersTypeDef,
-    ClipOutputTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
+    PlaylistTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
-    PlaylistTypeDef,
     VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
     JobAlbumArtOutputTypeDef,
-    CaptionsOutputTypeDef,
-    InputCaptionsOutputTypeDef,
     JobAlbumArtTypeDef,
+    CaptionsOutputTypeDef,
     CaptionsTypeDef,
+    InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
     JobOutputTypeDef,
-    JobInputOutputTypeDef,
     CreateJobOutputTypeDef,
+    JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
@@ -421,15 +406,15 @@
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
 )
 
 
-def get_structure() -> EncryptionOutputTypeDef:
+def get_structure() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.pyi` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__main__.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticTranscoder 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ElasticTranscoder 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.pyi` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.pyi` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -40,80 +40,74 @@
 __all__ = (
     "ListJobsByPipelinePaginator",
     "ListJobsByStatusPaginator",
     "ListPipelinesPaginator",
     "ListPresetsPaginator",
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
 class ListJobsByPipelinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsByPipelineResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
-
 class ListJobsByStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
     """
 
     def paginate(
-        self, *, Status: str, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: str, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsByStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
         """
 
-
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
         """
 
-
 class ListPresetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
         """
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.pyi` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,74 +40,80 @@
 __all__ = (
     "ListJobsByPipelinePaginator",
     "ListJobsByStatusPaginator",
     "ListPipelinesPaginator",
     "ListPresetsPaginator",
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
 class ListJobsByPipelinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsByPipelineResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
+
 class ListJobsByStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
     """
 
     def paginate(
-        self, *, Status: str, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: str, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsByStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
         """
 
+
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
         """
 
+
 class ListPresetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
         """
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,105 +2,90 @@
 Type annotations for elastictranscoder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elastictranscoder.type_defs import EncryptionOutputTypeDef
+    from mypy_boto3_elastictranscoder.type_defs import EncryptionTypeDef
 
-    data: EncryptionOutputTypeDef = {...}
+    data: EncryptionTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
-    "AudioCodecOptionsOutputTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "TimeSpanOutputTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
-    "DetectedPropertiesOutputTypeDef",
     "DetectedPropertiesTypeDef",
-    "HlsContentProtectionOutputTypeDef",
     "TimingTypeDef",
-    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
-    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "NotificationsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PermissionOutputTypeDef",
     "PermissionTypeDef",
-    "PlayReadyDrmOutputTypeDef",
-    "ThumbnailsOutputTypeDef",
-    "PresetWatermarkOutputTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
-    "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
-    "ArtworkOutputTypeDef",
-    "CaptionFormatOutputTypeDef",
-    "CaptionSourceOutputTypeDef",
-    "JobWatermarkOutputTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
-    "AudioParametersOutputTypeDef",
     "AudioParametersTypeDef",
-    "ClipOutputTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
+    "PlaylistTypeDef",
+    "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
+    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
     "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
-    "PlaylistTypeDef",
     "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
     "JobAlbumArtOutputTypeDef",
-    "CaptionsOutputTypeDef",
-    "InputCaptionsOutputTypeDef",
     "JobAlbumArtTypeDef",
+    "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
+    "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
     "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
     "JobOutputTypeDef",
-    "JobInputOutputTypeDef",
     "CreateJobOutputTypeDef",
+    "JobInputOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
@@ -111,47 +96,25 @@
     "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
 )
 
-EncryptionOutputTypeDef = TypedDict(
-    "EncryptionOutputTypeDef",
-    {
-        "Mode": str,
-        "Key": str,
-        "KeyMd5": str,
-        "InitializationVector": str,
-    },
-    total=False,
-)
-
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
         "KeyMd5": str,
         "InitializationVector": str,
     },
     total=False,
 )
 
-AudioCodecOptionsOutputTypeDef = TypedDict(
-    "AudioCodecOptionsOutputTypeDef",
-    {
-        "Profile": str,
-        "BitDepth": str,
-        "BitOrder": str,
-        "Signed": str,
-    },
-    total=False,
-)
-
 AudioCodecOptionsTypeDef = TypedDict(
     "AudioCodecOptionsTypeDef",
     {
         "Profile": str,
         "BitDepth": str,
         "BitOrder": str,
         "Signed": str,
@@ -162,23 +125,14 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-TimeSpanOutputTypeDef = TypedDict(
-    "TimeSpanOutputTypeDef",
-    {
-        "StartTime": str,
-        "Duration": str,
-    },
-    total=False,
-)
-
 TimeSpanTypeDef = TypedDict(
     "TimeSpanTypeDef",
     {
         "StartTime": str,
         "Duration": str,
     },
     total=False,
@@ -206,14 +160,25 @@
         "KeyId": str,
         "InitializationVector": str,
         "LicenseAcquisitionUrl": str,
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
 NotificationsTypeDef = TypedDict(
     "NotificationsTypeDef",
     {
         "Progressing": str,
         "Completed": str,
         "Warning": str,
         "Error": str,
@@ -255,84 +220,46 @@
 DeletePresetRequestRequestTypeDef = TypedDict(
     "DeletePresetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DetectedPropertiesOutputTypeDef = TypedDict(
-    "DetectedPropertiesOutputTypeDef",
-    {
-        "Width": int,
-        "Height": int,
-        "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-    },
-    total=False,
-)
-
 DetectedPropertiesTypeDef = TypedDict(
     "DetectedPropertiesTypeDef",
     {
         "Width": int,
         "Height": int,
         "FrameRate": str,
         "FileSize": int,
         "DurationMillis": int,
     },
     total=False,
 )
 
-HlsContentProtectionOutputTypeDef = TypedDict(
-    "HlsContentProtectionOutputTypeDef",
-    {
-        "Method": str,
-        "Key": str,
-        "KeyMd5": str,
-        "InitializationVector": str,
-        "LicenseAcquisitionUrl": str,
-        "KeyStoragePolicy": str,
-    },
-    total=False,
-)
-
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
     total=False,
 )
 
-_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
-    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobsByPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByPipelineRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalListJobsByPipelineRequestRequestTypeDef = TypedDict(
@@ -348,37 +275,14 @@
 class ListJobsByPipelineRequestRequestTypeDef(
     _RequiredListJobsByPipelineRequestRequestTypeDef,
     _OptionalListJobsByPipelineRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Status": str,
-    },
-)
-_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
-    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobsByStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByStatusRequestRequestTypeDef",
     {
         "Status": str,
     },
 )
 _OptionalListJobsByStatusRequestRequestTypeDef = TypedDict(
@@ -393,71 +297,32 @@
 
 class ListJobsByStatusRequestRequestTypeDef(
     _RequiredListJobsByStatusRequestRequestTypeDef, _OptionalListJobsByStatusRequestRequestTypeDef
 ):
     pass
 
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-NotificationsOutputTypeDef = TypedDict(
-    "NotificationsOutputTypeDef",
-    {
-        "Progressing": str,
-        "Completed": str,
-        "Warning": str,
-        "Error": str,
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
 PermissionOutputTypeDef = TypedDict(
     "PermissionOutputTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": List[str],
     },
@@ -470,59 +335,14 @@
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
     total=False,
 )
 
-PlayReadyDrmOutputTypeDef = TypedDict(
-    "PlayReadyDrmOutputTypeDef",
-    {
-        "Format": str,
-        "Key": str,
-        "KeyMd5": str,
-        "KeyId": str,
-        "InitializationVector": str,
-        "LicenseAcquisitionUrl": str,
-    },
-    total=False,
-)
-
-ThumbnailsOutputTypeDef = TypedDict(
-    "ThumbnailsOutputTypeDef",
-    {
-        "Format": str,
-        "Interval": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "SizingPolicy": str,
-        "PaddingPolicy": str,
-    },
-    total=False,
-)
-
-PresetWatermarkOutputTypeDef = TypedDict(
-    "PresetWatermarkOutputTypeDef",
-    {
-        "Id": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "SizingPolicy": str,
-        "HorizontalAlign": str,
-        "HorizontalOffset": str,
-        "VerticalAlign": str,
-        "VerticalOffset": str,
-        "Opacity": str,
-        "Target": str,
-    },
-    total=False,
-)
-
 PresetWatermarkTypeDef = TypedDict(
     "PresetWatermarkTypeDef",
     {
         "Id": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -562,98 +382,32 @@
 ReadPresetRequestRequestTypeDef = TypedDict(
     "ReadPresetRequestRequestTypeDef",
     {
         "Id": str,
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
 TestRoleRequestRequestTypeDef = TypedDict(
     "TestRoleRequestRequestTypeDef",
     {
         "Role": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Topics": Sequence[str],
     },
 )
 
-TestRoleResponseTypeDef = TypedDict(
-    "TestRoleResponseTypeDef",
-    {
-        "Success": str,
-        "Messages": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePipelineStatusRequestRequestTypeDef = TypedDict(
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
 
-ArtworkOutputTypeDef = TypedDict(
-    "ArtworkOutputTypeDef",
-    {
-        "InputKey": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "SizingPolicy": str,
-        "PaddingPolicy": str,
-        "AlbumArtFormat": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-CaptionFormatOutputTypeDef = TypedDict(
-    "CaptionFormatOutputTypeDef",
-    {
-        "Format": str,
-        "Pattern": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-CaptionSourceOutputTypeDef = TypedDict(
-    "CaptionSourceOutputTypeDef",
-    {
-        "Key": str,
-        "Language": str,
-        "TimeOffset": str,
-        "Label": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-JobWatermarkOutputTypeDef = TypedDict(
-    "JobWatermarkOutputTypeDef",
-    {
-        "PresetWatermarkId": str,
-        "InputKey": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
 ArtworkTypeDef = TypedDict(
     "ArtworkTypeDef",
     {
         "InputKey": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -692,48 +446,27 @@
         "PresetWatermarkId": str,
         "InputKey": str,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-AudioParametersOutputTypeDef = TypedDict(
-    "AudioParametersOutputTypeDef",
-    {
-        "Codec": str,
-        "SampleRate": str,
-        "BitRate": str,
-        "Channels": str,
-        "AudioPackingMode": str,
-        "CodecOptions": AudioCodecOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 AudioParametersTypeDef = TypedDict(
     "AudioParametersTypeDef",
     {
         "Codec": str,
         "SampleRate": str,
         "BitRate": str,
         "Channels": str,
         "AudioPackingMode": str,
         "CodecOptions": AudioCodecOptionsTypeDef,
     },
     total=False,
 )
 
-ClipOutputTypeDef = TypedDict(
-    "ClipOutputTypeDef",
-    {
-        "TimeSpan": TimeSpanOutputTypeDef,
-    },
-    total=False,
-)
-
 ClipTypeDef = TypedDict(
     "ClipTypeDef",
     {
         "TimeSpan": TimeSpanTypeDef,
     },
     total=False,
 )
@@ -746,22 +479,109 @@
         "OutputKeys": Sequence[str],
         "HlsContentProtection": HlsContentProtectionTypeDef,
         "PlayReadyDrm": PlayReadyDrmTypeDef,
     },
     total=False,
 )
 
+PlaylistTypeDef = TypedDict(
+    "PlaylistTypeDef",
+    {
+        "Name": str,
+        "Format": str,
+        "OutputKeys": List[str],
+        "HlsContentProtection": HlsContentProtectionTypeDef,
+        "PlayReadyDrm": PlayReadyDrmTypeDef,
+        "Status": str,
+        "StatusDetail": str,
+    },
+    total=False,
+)
+
+TestRoleResponseTypeDef = TypedDict(
+    "TestRoleResponseTypeDef",
+    {
+        "Success": str,
+        "Messages": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
+_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
+    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Status": str,
+    },
+)
+_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
+    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+):
+    pass
+
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 PipelineOutputConfigOutputTypeDef = TypedDict(
     "PipelineOutputConfigOutputTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": List[PermissionOutputTypeDef],
     },
@@ -774,28 +594,14 @@
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
-PlaylistTypeDef = TypedDict(
-    "PlaylistTypeDef",
-    {
-        "Name": str,
-        "Format": str,
-        "OutputKeys": List[str],
-        "HlsContentProtection": HlsContentProtectionOutputTypeDef,
-        "PlayReadyDrm": PlayReadyDrmOutputTypeDef,
-        "Status": str,
-        "StatusDetail": str,
-    },
-    total=False,
-)
-
 VideoParametersOutputTypeDef = TypedDict(
     "VideoParametersOutputTypeDef",
     {
         "Codec": str,
         "CodecOptions": Dict[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -805,15 +611,15 @@
         "Resolution": str,
         "AspectRatio": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "DisplayAspectRatio": str,
         "SizingPolicy": str,
         "PaddingPolicy": str,
-        "Watermarks": List[PresetWatermarkOutputTypeDef],
+        "Watermarks": List[PresetWatermarkTypeDef],
     },
     total=False,
 )
 
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
@@ -857,53 +663,53 @@
     pass
 
 
 JobAlbumArtOutputTypeDef = TypedDict(
     "JobAlbumArtOutputTypeDef",
     {
         "MergePolicy": str,
-        "Artwork": List[ArtworkOutputTypeDef],
+        "Artwork": List[ArtworkTypeDef],
     },
     total=False,
 )
 
-CaptionsOutputTypeDef = TypedDict(
-    "CaptionsOutputTypeDef",
+JobAlbumArtTypeDef = TypedDict(
+    "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceOutputTypeDef],
-        "CaptionFormats": List[CaptionFormatOutputTypeDef],
+        "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
 )
 
-InputCaptionsOutputTypeDef = TypedDict(
-    "InputCaptionsOutputTypeDef",
+CaptionsOutputTypeDef = TypedDict(
+    "CaptionsOutputTypeDef",
     {
         "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceOutputTypeDef],
+        "CaptionSources": List[CaptionSourceTypeDef],
+        "CaptionFormats": List[CaptionFormatTypeDef],
     },
     total=False,
 )
 
-JobAlbumArtTypeDef = TypedDict(
-    "JobAlbumArtTypeDef",
+CaptionsTypeDef = TypedDict(
+    "CaptionsTypeDef",
     {
         "MergePolicy": str,
-        "Artwork": Sequence[ArtworkTypeDef],
+        "CaptionSources": Sequence[CaptionSourceTypeDef],
+        "CaptionFormats": Sequence[CaptionFormatTypeDef],
     },
     total=False,
 )
 
-CaptionsTypeDef = TypedDict(
-    "CaptionsTypeDef",
+InputCaptionsOutputTypeDef = TypedDict(
+    "InputCaptionsOutputTypeDef",
     {
         "MergePolicy": str,
-        "CaptionSources": Sequence[CaptionSourceTypeDef],
-        "CaptionFormats": Sequence[CaptionFormatTypeDef],
+        "CaptionSources": List[CaptionSourceTypeDef],
     },
     total=False,
 )
 
 InputCaptionsTypeDef = TypedDict(
     "InputCaptionsTypeDef",
     {
@@ -920,15 +726,15 @@
         "Arn": str,
         "Name": str,
         "Status": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Role": str,
         "AwsKmsKeyArn": str,
-        "Notifications": NotificationsOutputTypeDef,
+        "Notifications": NotificationsTypeDef,
         "ContentConfig": PipelineOutputConfigOutputTypeDef,
         "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
@@ -989,17 +795,17 @@
     "PresetTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "Container": str,
-        "Audio": AudioParametersOutputTypeDef,
+        "Audio": AudioParametersTypeDef,
         "Video": VideoParametersOutputTypeDef,
-        "Thumbnails": ThumbnailsOutputTypeDef,
+        "Thumbnails": ThumbnailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
@@ -1028,53 +834,36 @@
 
 JobOutputTypeDef = TypedDict(
     "JobOutputTypeDef",
     {
         "Id": str,
         "Key": str,
         "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionOutputTypeDef,
+        "ThumbnailEncryption": EncryptionTypeDef,
         "Rotate": str,
         "PresetId": str,
         "SegmentDuration": str,
         "Status": str,
         "StatusDetail": str,
         "Duration": int,
         "Width": int,
         "Height": int,
         "FrameRate": str,
         "FileSize": int,
         "DurationMillis": int,
-        "Watermarks": List[JobWatermarkOutputTypeDef],
+        "Watermarks": List[JobWatermarkTypeDef],
         "AlbumArt": JobAlbumArtOutputTypeDef,
-        "Composition": List[ClipOutputTypeDef],
+        "Composition": List[ClipTypeDef],
         "Captions": CaptionsOutputTypeDef,
-        "Encryption": EncryptionOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
         "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
-JobInputOutputTypeDef = TypedDict(
-    "JobInputOutputTypeDef",
-    {
-        "Key": str,
-        "FrameRate": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "Interlaced": str,
-        "Container": str,
-        "Encryption": EncryptionOutputTypeDef,
-        "TimeSpan": TimeSpanOutputTypeDef,
-        "InputCaptions": InputCaptionsOutputTypeDef,
-        "DetectedProperties": DetectedPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "Key": str,
         "ThumbnailPattern": str,
         "ThumbnailEncryption": EncryptionTypeDef,
         "Rotate": str,
@@ -1085,14 +874,31 @@
         "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
+JobInputOutputTypeDef = TypedDict(
+    "JobInputOutputTypeDef",
+    {
+        "Key": str,
+        "FrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "Interlaced": str,
+        "Container": str,
+        "Encryption": EncryptionTypeDef,
+        "TimeSpan": TimeSpanTypeDef,
+        "InputCaptions": InputCaptionsOutputTypeDef,
+        "DetectedProperties": DetectedPropertiesTypeDef,
+    },
+    total=False,
+)
+
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
         "Key": str,
         "FrameRate": str,
         "Resolution": str,
         "AspectRatio": str,
@@ -1107,84 +913,84 @@
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "Pipelines": List[PipelineTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPipelineResponseTypeDef = TypedDict(
     "ReadPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineNotificationsResponseTypeDef = TypedDict(
     "UpdatePipelineNotificationsResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineStatusResponseTypeDef = TypedDict(
     "UpdatePipelineStatusResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "Presets": List[PresetTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPresetResponseTypeDef = TypedDict(
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Id": str,
@@ -1230,36 +1036,36 @@
     pass
 
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByPipelineResponseTypeDef = TypedDict(
     "ListJobsByPipelineResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByStatusResponseTypeDef = TypedDict(
     "ListJobsByStatusResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.pyi` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,104 +2,89 @@
 Type annotations for elastictranscoder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elastictranscoder.type_defs import EncryptionOutputTypeDef
+    from mypy_boto3_elastictranscoder.type_defs import EncryptionTypeDef
 
-    data: EncryptionOutputTypeDef = {...}
+    data: EncryptionTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
-    "AudioCodecOptionsOutputTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "TimeSpanOutputTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
-    "DetectedPropertiesOutputTypeDef",
     "DetectedPropertiesTypeDef",
-    "HlsContentProtectionOutputTypeDef",
     "TimingTypeDef",
-    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
-    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "NotificationsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PermissionOutputTypeDef",
     "PermissionTypeDef",
-    "PlayReadyDrmOutputTypeDef",
-    "ThumbnailsOutputTypeDef",
-    "PresetWatermarkOutputTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
-    "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
-    "ArtworkOutputTypeDef",
-    "CaptionFormatOutputTypeDef",
-    "CaptionSourceOutputTypeDef",
-    "JobWatermarkOutputTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
-    "AudioParametersOutputTypeDef",
     "AudioParametersTypeDef",
-    "ClipOutputTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
+    "PlaylistTypeDef",
+    "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
+    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
     "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
-    "PlaylistTypeDef",
     "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
     "JobAlbumArtOutputTypeDef",
-    "CaptionsOutputTypeDef",
-    "InputCaptionsOutputTypeDef",
     "JobAlbumArtTypeDef",
+    "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
+    "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
     "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
     "JobOutputTypeDef",
-    "JobInputOutputTypeDef",
     "CreateJobOutputTypeDef",
+    "JobInputOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
@@ -110,47 +95,25 @@
     "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
 )
 
-EncryptionOutputTypeDef = TypedDict(
-    "EncryptionOutputTypeDef",
-    {
-        "Mode": str,
-        "Key": str,
-        "KeyMd5": str,
-        "InitializationVector": str,
-    },
-    total=False,
-)
-
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
         "KeyMd5": str,
         "InitializationVector": str,
     },
     total=False,
 )
 
-AudioCodecOptionsOutputTypeDef = TypedDict(
-    "AudioCodecOptionsOutputTypeDef",
-    {
-        "Profile": str,
-        "BitDepth": str,
-        "BitOrder": str,
-        "Signed": str,
-    },
-    total=False,
-)
-
 AudioCodecOptionsTypeDef = TypedDict(
     "AudioCodecOptionsTypeDef",
     {
         "Profile": str,
         "BitDepth": str,
         "BitOrder": str,
         "Signed": str,
@@ -161,23 +124,14 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-TimeSpanOutputTypeDef = TypedDict(
-    "TimeSpanOutputTypeDef",
-    {
-        "StartTime": str,
-        "Duration": str,
-    },
-    total=False,
-)
-
 TimeSpanTypeDef = TypedDict(
     "TimeSpanTypeDef",
     {
         "StartTime": str,
         "Duration": str,
     },
     total=False,
@@ -205,14 +159,25 @@
         "KeyId": str,
         "InitializationVector": str,
         "LicenseAcquisitionUrl": str,
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
 NotificationsTypeDef = TypedDict(
     "NotificationsTypeDef",
     {
         "Progressing": str,
         "Completed": str,
         "Warning": str,
         "Error": str,
@@ -254,82 +219,46 @@
 DeletePresetRequestRequestTypeDef = TypedDict(
     "DeletePresetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DetectedPropertiesOutputTypeDef = TypedDict(
-    "DetectedPropertiesOutputTypeDef",
-    {
-        "Width": int,
-        "Height": int,
-        "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-    },
-    total=False,
-)
-
 DetectedPropertiesTypeDef = TypedDict(
     "DetectedPropertiesTypeDef",
     {
         "Width": int,
         "Height": int,
         "FrameRate": str,
         "FileSize": int,
         "DurationMillis": int,
     },
     total=False,
 )
 
-HlsContentProtectionOutputTypeDef = TypedDict(
-    "HlsContentProtectionOutputTypeDef",
-    {
-        "Method": str,
-        "Key": str,
-        "KeyMd5": str,
-        "InitializationVector": str,
-        "LicenseAcquisitionUrl": str,
-        "KeyStoragePolicy": str,
-    },
-    total=False,
-)
-
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
     total=False,
 )
 
-_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
-    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-):
-    pass
-
 _RequiredListJobsByPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByPipelineRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalListJobsByPipelineRequestRequestTypeDef = TypedDict(
@@ -343,35 +272,14 @@
 
 class ListJobsByPipelineRequestRequestTypeDef(
     _RequiredListJobsByPipelineRequestRequestTypeDef,
     _OptionalListJobsByPipelineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Status": str,
-    },
-)
-_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
-    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobsByStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByStatusRequestRequestTypeDef",
     {
         "Status": str,
     },
 )
 _OptionalListJobsByStatusRequestRequestTypeDef = TypedDict(
@@ -384,71 +292,32 @@
 )
 
 class ListJobsByStatusRequestRequestTypeDef(
     _RequiredListJobsByStatusRequestRequestTypeDef, _OptionalListJobsByStatusRequestRequestTypeDef
 ):
     pass
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-NotificationsOutputTypeDef = TypedDict(
-    "NotificationsOutputTypeDef",
-    {
-        "Progressing": str,
-        "Completed": str,
-        "Warning": str,
-        "Error": str,
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
 PermissionOutputTypeDef = TypedDict(
     "PermissionOutputTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": List[str],
     },
@@ -461,59 +330,14 @@
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
     total=False,
 )
 
-PlayReadyDrmOutputTypeDef = TypedDict(
-    "PlayReadyDrmOutputTypeDef",
-    {
-        "Format": str,
-        "Key": str,
-        "KeyMd5": str,
-        "KeyId": str,
-        "InitializationVector": str,
-        "LicenseAcquisitionUrl": str,
-    },
-    total=False,
-)
-
-ThumbnailsOutputTypeDef = TypedDict(
-    "ThumbnailsOutputTypeDef",
-    {
-        "Format": str,
-        "Interval": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "SizingPolicy": str,
-        "PaddingPolicy": str,
-    },
-    total=False,
-)
-
-PresetWatermarkOutputTypeDef = TypedDict(
-    "PresetWatermarkOutputTypeDef",
-    {
-        "Id": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "SizingPolicy": str,
-        "HorizontalAlign": str,
-        "HorizontalOffset": str,
-        "VerticalAlign": str,
-        "VerticalOffset": str,
-        "Opacity": str,
-        "Target": str,
-    },
-    total=False,
-)
-
 PresetWatermarkTypeDef = TypedDict(
     "PresetWatermarkTypeDef",
     {
         "Id": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -553,98 +377,32 @@
 ReadPresetRequestRequestTypeDef = TypedDict(
     "ReadPresetRequestRequestTypeDef",
     {
         "Id": str,
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
 TestRoleRequestRequestTypeDef = TypedDict(
     "TestRoleRequestRequestTypeDef",
     {
         "Role": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Topics": Sequence[str],
     },
 )
 
-TestRoleResponseTypeDef = TypedDict(
-    "TestRoleResponseTypeDef",
-    {
-        "Success": str,
-        "Messages": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePipelineStatusRequestRequestTypeDef = TypedDict(
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
 
-ArtworkOutputTypeDef = TypedDict(
-    "ArtworkOutputTypeDef",
-    {
-        "InputKey": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "SizingPolicy": str,
-        "PaddingPolicy": str,
-        "AlbumArtFormat": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-CaptionFormatOutputTypeDef = TypedDict(
-    "CaptionFormatOutputTypeDef",
-    {
-        "Format": str,
-        "Pattern": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-CaptionSourceOutputTypeDef = TypedDict(
-    "CaptionSourceOutputTypeDef",
-    {
-        "Key": str,
-        "Language": str,
-        "TimeOffset": str,
-        "Label": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-JobWatermarkOutputTypeDef = TypedDict(
-    "JobWatermarkOutputTypeDef",
-    {
-        "PresetWatermarkId": str,
-        "InputKey": str,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
 ArtworkTypeDef = TypedDict(
     "ArtworkTypeDef",
     {
         "InputKey": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -683,48 +441,27 @@
         "PresetWatermarkId": str,
         "InputKey": str,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-AudioParametersOutputTypeDef = TypedDict(
-    "AudioParametersOutputTypeDef",
-    {
-        "Codec": str,
-        "SampleRate": str,
-        "BitRate": str,
-        "Channels": str,
-        "AudioPackingMode": str,
-        "CodecOptions": AudioCodecOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 AudioParametersTypeDef = TypedDict(
     "AudioParametersTypeDef",
     {
         "Codec": str,
         "SampleRate": str,
         "BitRate": str,
         "Channels": str,
         "AudioPackingMode": str,
         "CodecOptions": AudioCodecOptionsTypeDef,
     },
     total=False,
 )
 
-ClipOutputTypeDef = TypedDict(
-    "ClipOutputTypeDef",
-    {
-        "TimeSpan": TimeSpanOutputTypeDef,
-    },
-    total=False,
-)
-
 ClipTypeDef = TypedDict(
     "ClipTypeDef",
     {
         "TimeSpan": TimeSpanTypeDef,
     },
     total=False,
 )
@@ -737,22 +474,105 @@
         "OutputKeys": Sequence[str],
         "HlsContentProtection": HlsContentProtectionTypeDef,
         "PlayReadyDrm": PlayReadyDrmTypeDef,
     },
     total=False,
 )
 
+PlaylistTypeDef = TypedDict(
+    "PlaylistTypeDef",
+    {
+        "Name": str,
+        "Format": str,
+        "OutputKeys": List[str],
+        "HlsContentProtection": HlsContentProtectionTypeDef,
+        "PlayReadyDrm": PlayReadyDrmTypeDef,
+        "Status": str,
+        "StatusDetail": str,
+    },
+    total=False,
+)
+
+TestRoleResponseTypeDef = TypedDict(
+    "TestRoleResponseTypeDef",
+    {
+        "Success": str,
+        "Messages": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
+_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
+    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+):
+    pass
+
+_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Status": str,
+    },
+)
+_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
+    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+):
+    pass
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 PipelineOutputConfigOutputTypeDef = TypedDict(
     "PipelineOutputConfigOutputTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": List[PermissionOutputTypeDef],
     },
@@ -765,28 +585,14 @@
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
-PlaylistTypeDef = TypedDict(
-    "PlaylistTypeDef",
-    {
-        "Name": str,
-        "Format": str,
-        "OutputKeys": List[str],
-        "HlsContentProtection": HlsContentProtectionOutputTypeDef,
-        "PlayReadyDrm": PlayReadyDrmOutputTypeDef,
-        "Status": str,
-        "StatusDetail": str,
-    },
-    total=False,
-)
-
 VideoParametersOutputTypeDef = TypedDict(
     "VideoParametersOutputTypeDef",
     {
         "Codec": str,
         "CodecOptions": Dict[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -796,15 +602,15 @@
         "Resolution": str,
         "AspectRatio": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "DisplayAspectRatio": str,
         "SizingPolicy": str,
         "PaddingPolicy": str,
-        "Watermarks": List[PresetWatermarkOutputTypeDef],
+        "Watermarks": List[PresetWatermarkTypeDef],
     },
     total=False,
 )
 
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
@@ -846,53 +652,53 @@
 ):
     pass
 
 JobAlbumArtOutputTypeDef = TypedDict(
     "JobAlbumArtOutputTypeDef",
     {
         "MergePolicy": str,
-        "Artwork": List[ArtworkOutputTypeDef],
+        "Artwork": List[ArtworkTypeDef],
     },
     total=False,
 )
 
-CaptionsOutputTypeDef = TypedDict(
-    "CaptionsOutputTypeDef",
+JobAlbumArtTypeDef = TypedDict(
+    "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceOutputTypeDef],
-        "CaptionFormats": List[CaptionFormatOutputTypeDef],
+        "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
 )
 
-InputCaptionsOutputTypeDef = TypedDict(
-    "InputCaptionsOutputTypeDef",
+CaptionsOutputTypeDef = TypedDict(
+    "CaptionsOutputTypeDef",
     {
         "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceOutputTypeDef],
+        "CaptionSources": List[CaptionSourceTypeDef],
+        "CaptionFormats": List[CaptionFormatTypeDef],
     },
     total=False,
 )
 
-JobAlbumArtTypeDef = TypedDict(
-    "JobAlbumArtTypeDef",
+CaptionsTypeDef = TypedDict(
+    "CaptionsTypeDef",
     {
         "MergePolicy": str,
-        "Artwork": Sequence[ArtworkTypeDef],
+        "CaptionSources": Sequence[CaptionSourceTypeDef],
+        "CaptionFormats": Sequence[CaptionFormatTypeDef],
     },
     total=False,
 )
 
-CaptionsTypeDef = TypedDict(
-    "CaptionsTypeDef",
+InputCaptionsOutputTypeDef = TypedDict(
+    "InputCaptionsOutputTypeDef",
     {
         "MergePolicy": str,
-        "CaptionSources": Sequence[CaptionSourceTypeDef],
-        "CaptionFormats": Sequence[CaptionFormatTypeDef],
+        "CaptionSources": List[CaptionSourceTypeDef],
     },
     total=False,
 )
 
 InputCaptionsTypeDef = TypedDict(
     "InputCaptionsTypeDef",
     {
@@ -909,15 +715,15 @@
         "Arn": str,
         "Name": str,
         "Status": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Role": str,
         "AwsKmsKeyArn": str,
-        "Notifications": NotificationsOutputTypeDef,
+        "Notifications": NotificationsTypeDef,
         "ContentConfig": PipelineOutputConfigOutputTypeDef,
         "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
@@ -974,17 +780,17 @@
     "PresetTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "Container": str,
-        "Audio": AudioParametersOutputTypeDef,
+        "Audio": AudioParametersTypeDef,
         "Video": VideoParametersOutputTypeDef,
-        "Thumbnails": ThumbnailsOutputTypeDef,
+        "Thumbnails": ThumbnailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
@@ -1011,53 +817,36 @@
 
 JobOutputTypeDef = TypedDict(
     "JobOutputTypeDef",
     {
         "Id": str,
         "Key": str,
         "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionOutputTypeDef,
+        "ThumbnailEncryption": EncryptionTypeDef,
         "Rotate": str,
         "PresetId": str,
         "SegmentDuration": str,
         "Status": str,
         "StatusDetail": str,
         "Duration": int,
         "Width": int,
         "Height": int,
         "FrameRate": str,
         "FileSize": int,
         "DurationMillis": int,
-        "Watermarks": List[JobWatermarkOutputTypeDef],
+        "Watermarks": List[JobWatermarkTypeDef],
         "AlbumArt": JobAlbumArtOutputTypeDef,
-        "Composition": List[ClipOutputTypeDef],
+        "Composition": List[ClipTypeDef],
         "Captions": CaptionsOutputTypeDef,
-        "Encryption": EncryptionOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
         "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
-JobInputOutputTypeDef = TypedDict(
-    "JobInputOutputTypeDef",
-    {
-        "Key": str,
-        "FrameRate": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "Interlaced": str,
-        "Container": str,
-        "Encryption": EncryptionOutputTypeDef,
-        "TimeSpan": TimeSpanOutputTypeDef,
-        "InputCaptions": InputCaptionsOutputTypeDef,
-        "DetectedProperties": DetectedPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "Key": str,
         "ThumbnailPattern": str,
         "ThumbnailEncryption": EncryptionTypeDef,
         "Rotate": str,
@@ -1068,14 +857,31 @@
         "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
+JobInputOutputTypeDef = TypedDict(
+    "JobInputOutputTypeDef",
+    {
+        "Key": str,
+        "FrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "Interlaced": str,
+        "Container": str,
+        "Encryption": EncryptionTypeDef,
+        "TimeSpan": TimeSpanTypeDef,
+        "InputCaptions": InputCaptionsOutputTypeDef,
+        "DetectedProperties": DetectedPropertiesTypeDef,
+    },
+    total=False,
+)
+
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
         "Key": str,
         "FrameRate": str,
         "Resolution": str,
         "AspectRatio": str,
@@ -1090,84 +896,84 @@
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "Pipelines": List[PipelineTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPipelineResponseTypeDef = TypedDict(
     "ReadPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineNotificationsResponseTypeDef = TypedDict(
     "UpdatePipelineNotificationsResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineStatusResponseTypeDef = TypedDict(
     "UpdatePipelineStatusResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "Presets": List[PresetTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPresetResponseTypeDef = TypedDict(
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Id": str,
@@ -1211,36 +1017,36 @@
 ):
     pass
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByPipelineResponseTypeDef = TypedDict(
     "ListJobsByPipelineResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByStatusResponseTypeDef = TypedDict(
     "ListJobsByStatusResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.py` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.pyi` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/PKG-INFO` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticTranscoder 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticTranscoder 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,90 +358,75 @@
 ### Typed dictionaries
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
-    EncryptionOutputTypeDef,
     EncryptionTypeDef,
-    AudioCodecOptionsOutputTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
-    TimeSpanOutputTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
-    DetectedPropertiesOutputTypeDef,
     DetectedPropertiesTypeDef,
-    HlsContentProtectionOutputTypeDef,
     TimingTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    NotificationsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PermissionOutputTypeDef,
     PermissionTypeDef,
-    PlayReadyDrmOutputTypeDef,
-    ThumbnailsOutputTypeDef,
-    PresetWatermarkOutputTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
-    ArtworkOutputTypeDef,
-    CaptionFormatOutputTypeDef,
-    CaptionSourceOutputTypeDef,
-    JobWatermarkOutputTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
-    AudioParametersOutputTypeDef,
     AudioParametersTypeDef,
-    ClipOutputTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
+    PlaylistTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
-    PlaylistTypeDef,
     VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
     JobAlbumArtOutputTypeDef,
-    CaptionsOutputTypeDef,
-    InputCaptionsOutputTypeDef,
     JobAlbumArtTypeDef,
+    CaptionsOutputTypeDef,
     CaptionsTypeDef,
+    InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
     JobOutputTypeDef,
-    JobInputOutputTypeDef,
     CreateJobOutputTypeDef,
+    JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
@@ -453,15 +438,15 @@
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
 )
 
 
-def get_structure() -> EncryptionOutputTypeDef:
+def get_structure() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt` & `mypy-boto3-elastictranscoder-1.28.15/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.12/setup.py` & `mypy-boto3-elastictranscoder-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastictranscoder",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticTranscoder 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ElasticTranscoder 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

