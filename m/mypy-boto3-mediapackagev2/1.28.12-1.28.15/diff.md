# Comparing `tmp/mypy-boto3-mediapackagev2-1.28.12.tar.gz` & `tmp/mypy-boto3-mediapackagev2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackagev2-1.28.12.tar", last modified: Thu Jul 27 05:35:01 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackagev2-1.28.15.tar", last modified: Fri Jul 28 20:43:16 2023, max compression
```

## Comparing `mypy-boto3-mediapackagev2-1.28.12.tar` & `mypy-boto3-mediapackagev2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.748438 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29180 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:26:23.000000 mypy-boto3-mediapackagev2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:16.869496 mypy-boto3-mediapackagev2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-07-28 20:43:16.869496 mypy-boto3-mediapackagev2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:16.869496 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28402 2023-07-28 20:31:38.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28360 2023-07-28 20:31:38.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:16.869496 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-07-28 20:43:16.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:16.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:16.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:16.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:16.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:16.000000 mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:16.869496 mypy-boto3-mediapackagev2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:31:37.000000 mypy-boto3-mediapackagev2-1.28.15/setup.py
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/LICENSE` & `mypy-boto3-mediapackagev2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/PKG-INFO` & `mypy-boto3-mediapackagev2-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.28.12
-Summary: Type annotations for boto3.mediapackagev2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.mediapackagev2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,69 +343,66 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     IngestEndpointTypeDef,
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
-    EncryptionMethodOutputTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
-    GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
-    ScteHlsOutputTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHlsManifestConfigurationTypeDef,
     ListLowLatencyHlsManifestConfigurationTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ScteOutputTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
-    UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    CreateChannelGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChannelGroupResponseTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetOriginEndpointPolicyResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
+    SpekeKeyProviderOutputTypeDef,
+    SpekeKeyProviderTypeDef,
+    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     OriginEndpointListConfigurationTypeDef,
     EncryptionOutputTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
     SegmentOutputTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/README.md` & `mypy-boto3-mediapackagev2-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,69 +311,66 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     IngestEndpointTypeDef,
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
-    EncryptionMethodOutputTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
-    GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
-    ScteHlsOutputTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHlsManifestConfigurationTypeDef,
     ListLowLatencyHlsManifestConfigurationTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ScteOutputTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
-    UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    CreateChannelGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChannelGroupResponseTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetOriginEndpointPolicyResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
+    SpekeKeyProviderOutputTypeDef,
+    SpekeKeyProviderTypeDef,
+    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     OriginEndpointListConfigurationTypeDef,
     EncryptionOutputTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
     SegmentOutputTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.py` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.pyi` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__main__.py` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mediapackagev2 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.mediapackagev2 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\nOther"
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

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.py` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.pyi` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.py` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.pyi` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.py` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,65 +32,60 @@
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListChannelGroupsPaginator", "ListChannelsPaginator", "ListOriginEndpointsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListChannelGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
         """
 
-
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, ChannelGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ChannelGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
         """
 
-
 class ListOriginEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listoriginendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.pyi` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,60 +32,65 @@
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListChannelGroupsPaginator", "ListChannelsPaginator", "ListOriginEndpointsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListChannelGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
         """
 
+
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, ChannelGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ChannelGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
         """
 
+
 class ListOriginEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listoriginendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.py` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,74 +30,70 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
-    "CreateChannelGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
-    "EncryptionMethodOutputTypeDef",
     "EncryptionMethodTypeDef",
     "GetChannelGroupRequestRequestTypeDef",
-    "GetChannelGroupResponseTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "GetChannelPolicyResponseTypeDef",
     "GetChannelRequestRequestTypeDef",
-    "ScteHlsOutputTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
-    "GetOriginEndpointPolicyResponseTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ScteOutputTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
-    "UpdateChannelGroupResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "CreateChannelGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetChannelGroupResponseTypeDef",
+    "GetChannelPolicyResponseTypeDef",
+    "GetOriginEndpointPolicyResponseTypeDef",
     "ListChannelGroupsResponseTypeDef",
     "ListChannelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateChannelGroupResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
-    "SpekeKeyProviderTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
+    "SpekeKeyProviderTypeDef",
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
     "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
     "SegmentOutputTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointResponseTypeDef",
@@ -120,21 +116,19 @@
     "_OptionalChannelGroupListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ChannelGroupListConfigurationTypeDef(
     _RequiredChannelGroupListConfigurationTypeDef, _OptionalChannelGroupListConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChannelListConfigurationTypeDef = TypedDict(
     "_RequiredChannelListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
@@ -145,21 +139,19 @@
     "_OptionalChannelListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ChannelListConfigurationTypeDef(
     _RequiredChannelListConfigurationTypeDef, _OptionalChannelListConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCreateChannelGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalCreateChannelGroupRequestRequestTypeDef = TypedDict(
@@ -168,33 +160,28 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateChannelGroupRequestRequestTypeDef(
     _RequiredCreateChannelGroupRequestRequestTypeDef,
     _OptionalCreateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
-
-CreateChannelGroupResponseTypeDef = TypedDict(
-    "CreateChannelGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -207,21 +194,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 IngestEndpointTypeDef = TypedDict(
     "IngestEndpointTypeDef",
     {
         "Id": str,
         "Url": str,
     },
     total=False,
@@ -272,46 +257,22 @@
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EncryptionContractConfigurationOutputTypeDef = TypedDict(
-    "EncryptionContractConfigurationOutputTypeDef",
-    {
-        "PresetSpeke20Audio": PresetSpeke20AudioType,
-        "PresetSpeke20Video": PresetSpeke20VideoType,
-    },
-)
-
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
 
-EncryptionMethodOutputTypeDef = TypedDict(
-    "EncryptionMethodOutputTypeDef",
-    {
-        "TsEncryptionMethod": TsEncryptionMethodType,
-        "CmafEncryptionMethod": CmafEncryptionMethodType,
-    },
-    total=False,
-)
-
 EncryptionMethodTypeDef = TypedDict(
     "EncryptionMethodTypeDef",
     {
         "TsEncryptionMethod": TsEncryptionMethodType,
         "CmafEncryptionMethod": CmafEncryptionMethodType,
     },
     total=False,
@@ -320,130 +281,67 @@
 GetChannelGroupRequestRequestTypeDef = TypedDict(
     "GetChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 
-GetChannelGroupResponseTypeDef = TypedDict(
-    "GetChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
-ScteHlsOutputTypeDef = TypedDict(
-    "ScteHlsOutputTypeDef",
-    {
-        "AdMarkerHls": Literal["DATERANGE"],
-    },
-    total=False,
-)
-
 GetOriginEndpointPolicyRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-GetOriginEndpointPolicyResponseTypeDef = TypedDict(
-    "GetOriginEndpointPolicyResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "OriginEndpointName": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOriginEndpointRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
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
 
 ListChannelGroupsRequestRequestTypeDef = TypedDict(
     "ListChannelGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-    },
-)
-_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListChannelsRequestListChannelsPaginateTypeDef(
-    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
-    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalListChannelsRequestRequestTypeDef = TypedDict(
@@ -451,21 +349,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelsRequestRequestTypeDef(
     _RequiredListChannelsRequestRequestTypeDef, _OptionalListChannelsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListHlsManifestConfigurationTypeDef = TypedDict(
@@ -473,21 +369,19 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
-
 class ListHlsManifestConfigurationTypeDef(
     _RequiredListHlsManifestConfigurationTypeDef, _OptionalListHlsManifestConfigurationTypeDef
 ):
     pass
 
-
 _RequiredListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -495,45 +389,20 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
-
 class ListLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredListLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalListLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-
-_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-    },
-)
-_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
-    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -542,47 +411,27 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListOriginEndpointsRequestRequestTypeDef(
     _RequiredListOriginEndpointsRequestRequestTypeDef,
     _OptionalListOriginEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
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
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "Policy": str,
     },
@@ -594,25 +443,14 @@
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "Policy": str,
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
 ScteOutputTypeDef = TypedDict(
     "ScteOutputTypeDef",
     {
         "ScteFilter": List[ScteFilterType],
     },
     total=False,
 )
@@ -651,118 +489,178 @@
     "_OptionalUpdateChannelGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateChannelGroupRequestRequestTypeDef(
     _RequiredUpdateChannelGroupRequestRequestTypeDef,
     _OptionalUpdateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateChannelRequestRequestTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+    },
+)
+_OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateChannelRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
 
-UpdateChannelGroupResponseTypeDef = TypedDict(
-    "UpdateChannelGroupResponseTypeDef",
+class UpdateChannelRequestRequestTypeDef(
+    _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
+):
+    pass
+
+CreateChannelGroupResponseTypeDef = TypedDict(
+    "CreateChannelGroupResponseTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
         "EgressDomain": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "ChannelGroupName": str,
-        "ChannelName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelRequestRequestTypeDef",
+
+GetChannelGroupResponseTypeDef = TypedDict(
+    "GetChannelGroupResponseTypeDef",
     {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
         "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateChannelRequestRequestTypeDef(
-    _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
-):
-    pass
-
+GetOriginEndpointPolicyResponseTypeDef = TypedDict(
+    "GetOriginEndpointPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "OriginEndpointName": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListChannelGroupsResponseTypeDef = TypedDict(
     "ListChannelGroupsResponseTypeDef",
     {
         "Items": List[ChannelGroupListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Items": List[ChannelListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+UpdateChannelGroupResponseTypeDef = TypedDict(
+    "UpdateChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
@@ -775,21 +673,19 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class CreateHlsManifestConfigurationTypeDef(
     _RequiredCreateHlsManifestConfigurationTypeDef, _OptionalCreateHlsManifestConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -799,94 +695,137 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class CreateLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-
-SpekeKeyProviderOutputTypeDef = TypedDict(
-    "SpekeKeyProviderOutputTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
-        "ResourceId": str,
-        "DrmSystems": List[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
-SpekeKeyProviderTypeDef = TypedDict(
-    "SpekeKeyProviderTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-        "ResourceId": str,
-        "DrmSystems": Sequence[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
 _RequiredGetHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
 _OptionalGetHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsOutputTypeDef,
+        "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
-
 class GetHlsManifestConfigurationTypeDef(
     _RequiredGetHlsManifestConfigurationTypeDef, _OptionalGetHlsManifestConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
 _OptionalGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsOutputTypeDef,
+        "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
-
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
+        "ResourceId": str,
+        "DrmSystems": List[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
+SpekeKeyProviderTypeDef = TypedDict(
+    "SpekeKeyProviderTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
+        "ResourceId": str,
+        "DrmSystems": Sequence[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
+ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+    },
+)
+_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListChannelsRequestListChannelsPaginateTypeDef(
+    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
+    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+    },
+)
+_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
+    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+):
+    pass
 
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
@@ -902,42 +841,38 @@
         "ModifiedAt": datetime,
         "HlsManifests": List[ListHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[ListLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
-
 _RequiredEncryptionOutputTypeDef = TypedDict(
     "_RequiredEncryptionOutputTypeDef",
     {
-        "EncryptionMethod": EncryptionMethodOutputTypeDef,
+        "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
 _OptionalEncryptionOutputTypeDef = TypedDict(
     "_OptionalEncryptionOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
     pass
 
-
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -946,25 +881,23 @@
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
-
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SegmentOutputTypeDef = TypedDict(
     "SegmentOutputTypeDef",
     {
         "SegmentDurationSeconds": int,
@@ -1004,15 +937,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginEndpointResponseTypeDef = TypedDict(
     "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -1024,15 +957,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOriginEndpointResponseTypeDef = TypedDict(
     "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -1044,15 +977,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -1071,22 +1004,20 @@
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateOriginEndpointRequestRequestTypeDef(
     _RequiredCreateOriginEndpointRequestRequestTypeDef,
     _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
@@ -1100,13 +1031,12 @@
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateOriginEndpointRequestRequestTypeDef(
     _RequiredUpdateOriginEndpointRequestRequestTypeDef,
     _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.pyi` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,73 +30,71 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
-    "CreateChannelGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
-    "EncryptionMethodOutputTypeDef",
     "EncryptionMethodTypeDef",
     "GetChannelGroupRequestRequestTypeDef",
-    "GetChannelGroupResponseTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "GetChannelPolicyResponseTypeDef",
     "GetChannelRequestRequestTypeDef",
-    "ScteHlsOutputTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
-    "GetOriginEndpointPolicyResponseTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ScteOutputTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
-    "UpdateChannelGroupResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "CreateChannelGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetChannelGroupResponseTypeDef",
+    "GetChannelPolicyResponseTypeDef",
+    "GetOriginEndpointPolicyResponseTypeDef",
     "ListChannelGroupsResponseTypeDef",
     "ListChannelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateChannelGroupResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
-    "SpekeKeyProviderTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
+    "SpekeKeyProviderTypeDef",
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
     "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
     "SegmentOutputTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointResponseTypeDef",
@@ -119,19 +117,21 @@
     "_OptionalChannelGroupListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ChannelGroupListConfigurationTypeDef(
     _RequiredChannelGroupListConfigurationTypeDef, _OptionalChannelGroupListConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChannelListConfigurationTypeDef = TypedDict(
     "_RequiredChannelListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
@@ -142,19 +142,21 @@
     "_OptionalChannelListConfigurationTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ChannelListConfigurationTypeDef(
     _RequiredChannelListConfigurationTypeDef, _OptionalChannelListConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCreateChannelGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalCreateChannelGroupRequestRequestTypeDef = TypedDict(
@@ -163,31 +165,30 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateChannelGroupRequestRequestTypeDef(
     _RequiredCreateChannelGroupRequestRequestTypeDef,
     _OptionalCreateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
-CreateChannelGroupResponseTypeDef = TypedDict(
-    "CreateChannelGroupResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -200,19 +201,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 IngestEndpointTypeDef = TypedDict(
     "IngestEndpointTypeDef",
     {
         "Id": str,
         "Url": str,
     },
     total=False,
@@ -263,46 +266,22 @@
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EncryptionContractConfigurationOutputTypeDef = TypedDict(
-    "EncryptionContractConfigurationOutputTypeDef",
-    {
-        "PresetSpeke20Audio": PresetSpeke20AudioType,
-        "PresetSpeke20Video": PresetSpeke20VideoType,
-    },
-)
-
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
 
-EncryptionMethodOutputTypeDef = TypedDict(
-    "EncryptionMethodOutputTypeDef",
-    {
-        "TsEncryptionMethod": TsEncryptionMethodType,
-        "CmafEncryptionMethod": CmafEncryptionMethodType,
-    },
-    total=False,
-)
-
 EncryptionMethodTypeDef = TypedDict(
     "EncryptionMethodTypeDef",
     {
         "TsEncryptionMethod": TsEncryptionMethodType,
         "CmafEncryptionMethod": CmafEncryptionMethodType,
     },
     total=False,
@@ -311,128 +290,67 @@
 GetChannelGroupRequestRequestTypeDef = TypedDict(
     "GetChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 
-GetChannelGroupResponseTypeDef = TypedDict(
-    "GetChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
-ScteHlsOutputTypeDef = TypedDict(
-    "ScteHlsOutputTypeDef",
-    {
-        "AdMarkerHls": Literal["DATERANGE"],
-    },
-    total=False,
-)
-
 GetOriginEndpointPolicyRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-GetOriginEndpointPolicyResponseTypeDef = TypedDict(
-    "GetOriginEndpointPolicyResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "OriginEndpointName": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOriginEndpointRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
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
 
 ListChannelGroupsRequestRequestTypeDef = TypedDict(
     "ListChannelGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-    },
-)
-_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListChannelsRequestListChannelsPaginateTypeDef(
-    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
-    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
-):
-    pass
-
 _RequiredListChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalListChannelsRequestRequestTypeDef = TypedDict(
@@ -440,19 +358,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelsRequestRequestTypeDef(
     _RequiredListChannelsRequestRequestTypeDef, _OptionalListChannelsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListHlsManifestConfigurationTypeDef = TypedDict(
@@ -460,19 +380,21 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
+
 class ListHlsManifestConfigurationTypeDef(
     _RequiredListHlsManifestConfigurationTypeDef, _OptionalListHlsManifestConfigurationTypeDef
 ):
     pass
 
+
 _RequiredListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredListLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalListLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -480,40 +402,21 @@
     {
         "ChildManifestName": str,
         "Url": str,
     },
     total=False,
 )
 
+
 class ListLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredListLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalListLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-    },
-)
-_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
-    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-):
-    pass
 
 _RequiredListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
@@ -523,45 +426,29 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListOriginEndpointsRequestRequestTypeDef(
     _RequiredListOriginEndpointsRequestRequestTypeDef,
     _OptionalListOriginEndpointsRequestRequestTypeDef,
 ):
     pass
 
+
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
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "Policy": str,
     },
@@ -573,25 +460,14 @@
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "Policy": str,
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
 ScteOutputTypeDef = TypedDict(
     "ScteOutputTypeDef",
     {
         "ScteFilter": List[ScteFilterType],
     },
     total=False,
 )
@@ -630,33 +506,21 @@
     "_OptionalUpdateChannelGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateChannelGroupRequestRequestTypeDef(
     _RequiredUpdateChannelGroupRequestRequestTypeDef,
     _OptionalUpdateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
-UpdateChannelGroupResponseTypeDef = TypedDict(
-    "UpdateChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
@@ -665,79 +529,159 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
+CreateChannelGroupResponseTypeDef = TypedDict(
+    "CreateChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
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
+GetChannelGroupResponseTypeDef = TypedDict(
+    "GetChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOriginEndpointPolicyResponseTypeDef = TypedDict(
+    "GetOriginEndpointPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "OriginEndpointName": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListChannelGroupsResponseTypeDef = TypedDict(
     "ListChannelGroupsResponseTypeDef",
     {
         "Items": List[ChannelGroupListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Items": List[ChannelListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+UpdateChannelGroupResponseTypeDef = TypedDict(
+    "UpdateChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
@@ -750,19 +694,21 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class CreateHlsManifestConfigurationTypeDef(
     _RequiredCreateHlsManifestConfigurationTypeDef, _OptionalCreateHlsManifestConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
     },
 )
 _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
@@ -772,89 +718,148 @@
         "ScteHls": ScteHlsTypeDef,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class CreateLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-SpekeKeyProviderOutputTypeDef = TypedDict(
-    "SpekeKeyProviderOutputTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
-        "ResourceId": str,
-        "DrmSystems": List[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
-SpekeKeyProviderTypeDef = TypedDict(
-    "SpekeKeyProviderTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-        "ResourceId": str,
-        "DrmSystems": Sequence[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
 
 _RequiredGetHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
 _OptionalGetHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsOutputTypeDef,
+        "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
+
 class GetHlsManifestConfigurationTypeDef(
     _RequiredGetHlsManifestConfigurationTypeDef, _OptionalGetHlsManifestConfigurationTypeDef
 ):
     pass
 
+
 _RequiredGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
 _OptionalGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsOutputTypeDef,
+        "ScteHls": ScteHlsTypeDef,
     },
     total=False,
 )
 
+
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
+        "ResourceId": str,
+        "DrmSystems": List[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
+SpekeKeyProviderTypeDef = TypedDict(
+    "SpekeKeyProviderTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
+        "ResourceId": str,
+        "DrmSystems": Sequence[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
+ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+    },
+)
+_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListChannelsRequestListChannelsPaginateTypeDef(
+    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
+    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+    },
+)
+_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
+    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -869,38 +874,42 @@
         "ModifiedAt": datetime,
         "HlsManifests": List[ListHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[ListLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
+
 _RequiredEncryptionOutputTypeDef = TypedDict(
     "_RequiredEncryptionOutputTypeDef",
     {
-        "EncryptionMethod": EncryptionMethodOutputTypeDef,
+        "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
 _OptionalEncryptionOutputTypeDef = TypedDict(
     "_OptionalEncryptionOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
     pass
 
+
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -909,23 +918,25 @@
     {
         "ConstantInitializationVector": str,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
+
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SegmentOutputTypeDef = TypedDict(
     "SegmentOutputTypeDef",
     {
         "SegmentDurationSeconds": int,
@@ -965,15 +976,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginEndpointResponseTypeDef = TypedDict(
     "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -985,15 +996,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOriginEndpointResponseTypeDef = TypedDict(
     "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -1005,15 +1016,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -1032,20 +1043,22 @@
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateOriginEndpointRequestRequestTypeDef(
     _RequiredCreateOriginEndpointRequestRequestTypeDef,
     _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
@@ -1059,12 +1072,13 @@
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateOriginEndpointRequestRequestTypeDef(
     _RequiredUpdateOriginEndpointRequestRequestTypeDef,
     _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/PKG-INFO` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.28.12
-Summary: Type annotations for boto3.mediapackagev2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.mediapackagev2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,69 +343,66 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     IngestEndpointTypeDef,
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
-    EncryptionMethodOutputTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
-    GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
-    ScteHlsOutputTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHlsManifestConfigurationTypeDef,
     ListLowLatencyHlsManifestConfigurationTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ScteOutputTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
-    UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    CreateChannelGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChannelGroupResponseTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetOriginEndpointPolicyResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
+    SpekeKeyProviderOutputTypeDef,
+    SpekeKeyProviderTypeDef,
+    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     OriginEndpointListConfigurationTypeDef,
     EncryptionOutputTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
     SegmentOutputTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt` & `mypy-boto3-mediapackagev2-1.28.15/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.12/setup.py` & `mypy-boto3-mediapackagev2-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackagev2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mediapackagev2 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.mediapackagev2 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

