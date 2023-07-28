# Comparing `tmp/mypy-boto3-mediapackage-1.28.12.tar.gz` & `tmp/mypy-boto3-mediapackage-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-1.28.12.tar` & `mypy-boto3-mediapackage-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.856442 mypy-boto3-mediapackage-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-07-27 05:35:00.848442 mypy-boto3-mediapackage-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.840442 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31656 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.848442 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.856442 mypy-boto3-mediapackage-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.245473 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30177 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30146 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/setup.py
```

### Comparing `mypy-boto3-mediapackage-1.28.12/LICENSE` & `mypy-boto3-mediapackage-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/PKG-INFO` & `mypy-boto3-mediapackage-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaPackage 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,59 +345,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
-    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
-    EgressAccessLogsOutputTypeDef,
-    IngressAccessLogsOutputTypeDef,
+    EgressAccessLogsTypeDef,
+    IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
-    StreamSelectionOutputTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
+    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
-    S3DestinationOutputTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RotateChannelCredentialsRequestRequestTypeDef,
     RotateIngestEndpointCredentialsRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListHarvestJobsResponseTypeDef,
     CmafEncryptionOutputTypeDef,
     DashEncryptionOutputTypeDef,
     HlsEncryptionOutputTypeDef,
     MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
@@ -425,15 +419,15 @@
     UpdateOriginEndpointResponseTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationOutputTypeDef:
+def get_structure() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.12/README.md` & `mypy-boto3-mediapackage-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,59 +313,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
-    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
-    EgressAccessLogsOutputTypeDef,
-    IngressAccessLogsOutputTypeDef,
+    EgressAccessLogsTypeDef,
+    IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
-    StreamSelectionOutputTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
+    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
-    S3DestinationOutputTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RotateChannelCredentialsRequestRequestTypeDef,
     RotateIngestEndpointCredentialsRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListHarvestJobsResponseTypeDef,
     CmafEncryptionOutputTypeDef,
     DashEncryptionOutputTypeDef,
     HlsEncryptionOutputTypeDef,
     MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
@@ -393,15 +387,15 @@
     UpdateOriginEndpointResponseTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationOutputTypeDef:
+def get_structure() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.py` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.pyi` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__main__.py` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackage 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaPackage 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.py` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.pyi` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.py` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.pyi` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.py` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
         """
 
 
@@ -69,28 +69,28 @@
     """
 
     def paginate(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHarvestJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listharvestjobspaginator)
         """
 
 
 class ListOriginEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ChannelId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.pyi` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
         """
 
 class ListHarvestJobsPaginator(Paginator):
@@ -65,27 +65,27 @@
     """
 
     def paginate(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHarvestJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listharvestjobspaginator)
         """
 
 class ListOriginEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ChannelId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.py` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediapackage service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediapackage.type_defs import AuthorizationOutputTypeDef
+    from mypy_boto3_mediapackage.type_defs import AuthorizationTypeDef
 
-    data: AuthorizationOutputTypeDef = {...}
+    data: AuthorizationTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
@@ -39,59 +39,53 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
-    "EgressAccessLogsOutputTypeDef",
-    "IngressAccessLogsOutputTypeDef",
+    "EgressAccessLogsTypeDef",
+    "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
-    "StreamSelectionOutputTypeDef",
-    "EgressAccessLogsTypeDef",
-    "IngressAccessLogsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "S3DestinationTypeDef",
-    "S3DestinationOutputTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeHarvestJobRequestRequestTypeDef",
     "DescribeOriginEndpointRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "IngestEndpointTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListHarvestJobsRequestRequestTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RotateChannelCredentialsRequestRequestTypeDef",
     "RotateIngestEndpointCredentialsRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListHarvestJobsResponseTypeDef",
     "CmafEncryptionOutputTypeDef",
     "DashEncryptionOutputTypeDef",
     "HlsEncryptionOutputTypeDef",
     "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
@@ -118,40 +112,32 @@
     "OriginEndpointTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
-AuthorizationOutputTypeDef = TypedDict(
-    "AuthorizationOutputTypeDef",
-    {
-        "CdnIdentifierSecret": str,
-        "SecretsRoleArn": str,
-    },
-)
-
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
         "CdnIdentifierSecret": str,
         "SecretsRoleArn": str,
     },
 )
 
-EgressAccessLogsOutputTypeDef = TypedDict(
-    "EgressAccessLogsOutputTypeDef",
+EgressAccessLogsTypeDef = TypedDict(
+    "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
-IngressAccessLogsOutputTypeDef = TypedDict(
-    "IngressAccessLogsOutputTypeDef",
+IngressAccessLogsTypeDef = TypedDict(
+    "IngressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
 _RequiredHlsManifestCreateOrUpdateParametersTypeDef = TypedDict(
@@ -216,38 +202,23 @@
 )
 
 
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
     pass
 
 
-StreamSelectionOutputTypeDef = TypedDict(
-    "StreamSelectionOutputTypeDef",
-    {
-        "MaxVideoBitsPerSecond": int,
-        "MinVideoBitsPerSecond": int,
-        "StreamOrder": StreamOrderType,
-    },
-    total=False,
-)
-
-EgressAccessLogsTypeDef = TypedDict(
-    "EgressAccessLogsTypeDef",
-    {
-        "LogGroupName": str,
-    },
-    total=False,
-)
-
-IngressAccessLogsTypeDef = TypedDict(
-    "IngressAccessLogsTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "LogGroupName": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -273,23 +244,14 @@
     {
         "BucketName": str,
         "ManifestKey": str,
         "RoleArn": str,
     },
 )
 
-S3DestinationOutputTypeDef = TypedDict(
-    "S3DestinationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ManifestKey": str,
-        "RoleArn": str,
-    },
-)
-
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -317,29 +279,14 @@
 DescribeOriginEndpointRequestRequestTypeDef = TypedDict(
     "DescribeOriginEndpointRequestRequestTypeDef",
     {
         "Id": str,
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
@@ -351,61 +298,44 @@
         "Password": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
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
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
-    {
-        "IncludeChannelId": str,
-        "IncludeStatus": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHarvestJobsRequestRequestTypeDef = TypedDict(
     "ListHarvestJobsRequestRequestTypeDef",
     {
         "IncludeChannelId": str,
         "IncludeStatus": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "ListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -415,43 +345,14 @@
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
 RotateChannelCredentialsRequestRequestTypeDef = TypedDict(
     "RotateChannelCredentialsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -518,14 +419,29 @@
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
 
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
 CreateHarvestJobRequestRequestTypeDef = TypedDict(
     "CreateHarvestJobRequestRequestTypeDef",
     {
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
@@ -538,47 +454,47 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationOutputTypeDef,
+        "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHarvestJobResponseTypeDef = TypedDict(
     "DescribeHarvestJobResponseTypeDef",
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationOutputTypeDef,
+        "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HarvestJobTypeDef = TypedDict(
     "HarvestJobTypeDef",
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationOutputTypeDef,
+        "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
     },
     total=False,
 )
 
 _RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
@@ -590,15 +506,15 @@
         "Url": str,
     },
 )
 _OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
     "_OptionalSpekeKeyProviderOutputTypeDef",
     {
         "CertificateArn": str,
-        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class SpekeKeyProviderOutputTypeDef(
     _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
@@ -633,20 +549,47 @@
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
+    {
+        "IncludeChannelId": str,
+        "IncludeStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListHarvestJobsResponseTypeDef = TypedDict(
     "ListHarvestJobsResponseTypeDef",
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCmafEncryptionOutputTypeDef = TypedDict(
     "_RequiredCmafEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
@@ -792,121 +735,121 @@
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ConfigureLogsResponseTypeDef = TypedDict(
     "ConfigureLogsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateChannelCredentialsResponseTypeDef = TypedDict(
     "RotateChannelCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateIngestEndpointCredentialsResponseTypeDef = TypedDict(
     "RotateIngestEndpointCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CmafPackageTypeDef = TypedDict(
     "CmafPackageTypeDef",
     {
         "Encryption": CmafEncryptionOutputTypeDef,
         "HlsManifests": List[HlsManifestTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
 DashPackageOutputTypeDef = TypedDict(
     "DashPackageOutputTypeDef",
     {
@@ -918,15 +861,15 @@
         "ManifestWindowSeconds": int,
         "MinBufferTimeSeconds": int,
         "MinUpdatePeriodSeconds": int,
         "PeriodTriggers": List[Literal["ADS"]],
         "Profile": ProfileType,
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
         "SuggestedPresentationDelaySeconds": int,
         "UtcTiming": UtcTimingType,
         "UtcTimingUri": str,
     },
     total=False,
 )
 
@@ -939,27 +882,27 @@
         "Encryption": HlsEncryptionOutputTypeDef,
         "IncludeDvbSubtitles": bool,
         "IncludeIframeOnlyStream": bool,
         "PlaylistType": PlaylistTypeType,
         "PlaylistWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
         "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
 MssPackageOutputTypeDef = TypedDict(
     "MssPackageOutputTypeDef",
     {
         "Encryption": MssEncryptionOutputTypeDef,
         "ManifestWindowSeconds": int,
         "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
 CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
     "CmafPackageCreateOrUpdateParametersTypeDef",
     {
@@ -1026,23 +969,23 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateOriginEndpointResponseTypeDef = TypedDict(
     "CreateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1050,23 +993,23 @@
         "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOriginEndpointResponseTypeDef = TypedDict(
     "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1074,23 +1017,23 @@
         "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginEndpointTypeDef = TypedDict(
     "OriginEndpointTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1106,15 +1049,15 @@
     total=False,
 )
 
 UpdateOriginEndpointResponseTypeDef = TypedDict(
     "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1122,15 +1065,15 @@
         "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -1197,10 +1140,10 @@
 
 
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.pyi` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediapackage service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediapackage.type_defs import AuthorizationOutputTypeDef
+    from mypy_boto3_mediapackage.type_defs import AuthorizationTypeDef
 
-    data: AuthorizationOutputTypeDef = {...}
+    data: AuthorizationTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
@@ -38,59 +38,53 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
-    "EgressAccessLogsOutputTypeDef",
-    "IngressAccessLogsOutputTypeDef",
+    "EgressAccessLogsTypeDef",
+    "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
-    "StreamSelectionOutputTypeDef",
-    "EgressAccessLogsTypeDef",
-    "IngressAccessLogsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "S3DestinationTypeDef",
-    "S3DestinationOutputTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeHarvestJobRequestRequestTypeDef",
     "DescribeOriginEndpointRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "IngestEndpointTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListHarvestJobsRequestRequestTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RotateChannelCredentialsRequestRequestTypeDef",
     "RotateIngestEndpointCredentialsRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListHarvestJobsResponseTypeDef",
     "CmafEncryptionOutputTypeDef",
     "DashEncryptionOutputTypeDef",
     "HlsEncryptionOutputTypeDef",
     "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
@@ -117,40 +111,32 @@
     "OriginEndpointTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
-AuthorizationOutputTypeDef = TypedDict(
-    "AuthorizationOutputTypeDef",
-    {
-        "CdnIdentifierSecret": str,
-        "SecretsRoleArn": str,
-    },
-)
-
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
         "CdnIdentifierSecret": str,
         "SecretsRoleArn": str,
     },
 )
 
-EgressAccessLogsOutputTypeDef = TypedDict(
-    "EgressAccessLogsOutputTypeDef",
+EgressAccessLogsTypeDef = TypedDict(
+    "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
-IngressAccessLogsOutputTypeDef = TypedDict(
-    "IngressAccessLogsOutputTypeDef",
+IngressAccessLogsTypeDef = TypedDict(
+    "IngressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
 _RequiredHlsManifestCreateOrUpdateParametersTypeDef = TypedDict(
@@ -211,38 +197,23 @@
     },
     total=False,
 )
 
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
     pass
 
-StreamSelectionOutputTypeDef = TypedDict(
-    "StreamSelectionOutputTypeDef",
-    {
-        "MaxVideoBitsPerSecond": int,
-        "MinVideoBitsPerSecond": int,
-        "StreamOrder": StreamOrderType,
-    },
-    total=False,
-)
-
-EgressAccessLogsTypeDef = TypedDict(
-    "EgressAccessLogsTypeDef",
-    {
-        "LogGroupName": str,
-    },
-    total=False,
-)
-
-IngressAccessLogsTypeDef = TypedDict(
-    "IngressAccessLogsTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "LogGroupName": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -266,23 +237,14 @@
     {
         "BucketName": str,
         "ManifestKey": str,
         "RoleArn": str,
     },
 )
 
-S3DestinationOutputTypeDef = TypedDict(
-    "S3DestinationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ManifestKey": str,
-        "RoleArn": str,
-    },
-)
-
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -310,29 +272,14 @@
 DescribeOriginEndpointRequestRequestTypeDef = TypedDict(
     "DescribeOriginEndpointRequestRequestTypeDef",
     {
         "Id": str,
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
@@ -344,61 +291,44 @@
         "Password": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
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
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
-    {
-        "IncludeChannelId": str,
-        "IncludeStatus": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHarvestJobsRequestRequestTypeDef = TypedDict(
     "ListHarvestJobsRequestRequestTypeDef",
     {
         "IncludeChannelId": str,
         "IncludeStatus": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "ListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -408,43 +338,14 @@
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
 RotateChannelCredentialsRequestRequestTypeDef = TypedDict(
     "RotateChannelCredentialsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -507,14 +408,29 @@
 )
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
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
 CreateHarvestJobRequestRequestTypeDef = TypedDict(
     "CreateHarvestJobRequestRequestTypeDef",
     {
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
@@ -527,47 +443,47 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationOutputTypeDef,
+        "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHarvestJobResponseTypeDef = TypedDict(
     "DescribeHarvestJobResponseTypeDef",
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationOutputTypeDef,
+        "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HarvestJobTypeDef = TypedDict(
     "HarvestJobTypeDef",
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationOutputTypeDef,
+        "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
     },
     total=False,
 )
 
 _RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
@@ -579,15 +495,15 @@
         "Url": str,
     },
 )
 _OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
     "_OptionalSpekeKeyProviderOutputTypeDef",
     {
         "CertificateArn": str,
-        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
 class SpekeKeyProviderOutputTypeDef(
     _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
 ):
@@ -618,20 +534,47 @@
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
+    {
+        "IncludeChannelId": str,
+        "IncludeStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListHarvestJobsResponseTypeDef = TypedDict(
     "ListHarvestJobsResponseTypeDef",
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCmafEncryptionOutputTypeDef = TypedDict(
     "_RequiredCmafEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
@@ -765,121 +708,121 @@
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ConfigureLogsResponseTypeDef = TypedDict(
     "ConfigureLogsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateChannelCredentialsResponseTypeDef = TypedDict(
     "RotateChannelCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateIngestEndpointCredentialsResponseTypeDef = TypedDict(
     "RotateIngestEndpointCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
+        "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CmafPackageTypeDef = TypedDict(
     "CmafPackageTypeDef",
     {
         "Encryption": CmafEncryptionOutputTypeDef,
         "HlsManifests": List[HlsManifestTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
 DashPackageOutputTypeDef = TypedDict(
     "DashPackageOutputTypeDef",
     {
@@ -891,15 +834,15 @@
         "ManifestWindowSeconds": int,
         "MinBufferTimeSeconds": int,
         "MinUpdatePeriodSeconds": int,
         "PeriodTriggers": List[Literal["ADS"]],
         "Profile": ProfileType,
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
         "SuggestedPresentationDelaySeconds": int,
         "UtcTiming": UtcTimingType,
         "UtcTimingUri": str,
     },
     total=False,
 )
 
@@ -912,27 +855,27 @@
         "Encryption": HlsEncryptionOutputTypeDef,
         "IncludeDvbSubtitles": bool,
         "IncludeIframeOnlyStream": bool,
         "PlaylistType": PlaylistTypeType,
         "PlaylistWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
         "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
 MssPackageOutputTypeDef = TypedDict(
     "MssPackageOutputTypeDef",
     {
         "Encryption": MssEncryptionOutputTypeDef,
         "ManifestWindowSeconds": int,
         "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
 CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
     "CmafPackageCreateOrUpdateParametersTypeDef",
     {
@@ -999,23 +942,23 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateOriginEndpointResponseTypeDef = TypedDict(
     "CreateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1023,23 +966,23 @@
         "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOriginEndpointResponseTypeDef = TypedDict(
     "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1047,23 +990,23 @@
         "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginEndpointTypeDef = TypedDict(
     "OriginEndpointTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1079,15 +1022,15 @@
     total=False,
 )
 
 UpdateOriginEndpointResponseTypeDef = TypedDict(
     "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
@@ -1095,15 +1038,15 @@
         "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -1166,10 +1109,10 @@
     pass
 
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaPackage 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,59 +345,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
-    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
-    EgressAccessLogsOutputTypeDef,
-    IngressAccessLogsOutputTypeDef,
+    EgressAccessLogsTypeDef,
+    IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
-    StreamSelectionOutputTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
+    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
-    S3DestinationOutputTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RotateChannelCredentialsRequestRequestTypeDef,
     RotateIngestEndpointCredentialsRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListHarvestJobsResponseTypeDef,
     CmafEncryptionOutputTypeDef,
     DashEncryptionOutputTypeDef,
     HlsEncryptionOutputTypeDef,
     MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
@@ -425,15 +419,15 @@
     UpdateOriginEndpointResponseTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationOutputTypeDef:
+def get_structure() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.12/setup.py` & `mypy-boto3-mediapackage-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackage 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

