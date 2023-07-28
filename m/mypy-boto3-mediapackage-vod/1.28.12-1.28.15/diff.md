# Comparing `tmp/mypy-boto3-mediapackage-vod-1.28.12.tar.gz` & `tmp/mypy-boto3-mediapackage-vod-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.12.tar", last modified: Thu Jul 27 05:35:01 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-vod-1.28.12.tar` & `mypy-boto3-mediapackage-vod-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.104441 mypy-boto3-mediapackage-vod-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-27 05:35:01.100441 mypy-boto3-mediapackage-vod-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.096441 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26582 2023-07-27 05:26:23.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.100441 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:01.104441 mypy-boto3-mediapackage-vod-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.341475 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/setup.py
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/LICENSE` & `mypy-boto3-mediapackage-vod-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaPackageVod 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,62 +343,55 @@
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
-    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
-    EgressAccessLogsOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
-    StreamSelectionOutputTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssetsRequestRequestTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
     CreatePackagingGroupRequestRequestTypeDef,
+    PackagingGroupTypeDef,
     ConfigureLogsResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
-    PackagingGroupTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAssetsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
-    DashManifestOutputTypeDef,
-    HlsManifestOutputTypeDef,
-    MssManifestOutputTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
+    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
+    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsResponseTypeDef,
     CmafEncryptionOutputTypeDef,
     DashEncryptionOutputTypeDef,
     HlsEncryptionOutputTypeDef,
     MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/README.md` & `mypy-boto3-mediapackage-vod-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,62 +311,55 @@
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
-    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
-    EgressAccessLogsOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
-    StreamSelectionOutputTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssetsRequestRequestTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
     CreatePackagingGroupRequestRequestTypeDef,
+    PackagingGroupTypeDef,
     ConfigureLogsResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
-    PackagingGroupTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAssetsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
-    DashManifestOutputTypeDef,
-    HlsManifestOutputTypeDef,
-    MssManifestOutputTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
+    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
+    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsResponseTypeDef,
     CmafEncryptionOutputTypeDef,
     DashEncryptionOutputTypeDef,
     HlsEncryptionOutputTypeDef,
     MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.py` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.pyi` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__main__.py` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackageVod 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaPackageVod 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.py` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.pyi` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.py` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.pyi` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.py` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,61 +36,56 @@
 
 __all__ = (
     "ListAssetsPaginator",
     "ListPackagingConfigurationsPaginator",
     "ListPackagingGroupsPaginator",
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
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
         """
 
-
 class ListPackagingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
         """
 
-
 class ListPackagingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.pyi` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,56 +36,61 @@
 
 __all__ = (
     "ListAssetsPaginator",
     "ListPackagingConfigurationsPaginator",
     "ListPackagingGroupsPaginator",
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
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
         """
 
+
 class ListPackagingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
         """
 
+
 class ListPackagingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.py` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -31,65 +31,57 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssetShallowTypeDef",
-    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
-    "EgressAccessLogsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
-    "StreamSelectionOutputTypeDef",
     "StreamSelectionTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeletePackagingConfigurationRequestRequestTypeDef",
     "DeletePackagingGroupRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribePackagingConfigurationRequestRequestTypeDef",
     "DescribePackagingGroupRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
-    "ListAssetsRequestListAssetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssetsRequestRequestTypeDef",
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingConfigurationsRequestRequestTypeDef",
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListAssetsResponseTypeDef",
     "UpdatePackagingGroupRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
     "CreatePackagingGroupRequestRequestTypeDef",
+    "PackagingGroupTypeDef",
     "ConfigureLogsResponseTypeDef",
     "CreatePackagingGroupResponseTypeDef",
     "DescribePackagingGroupResponseTypeDef",
-    "PackagingGroupTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAssetsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
-    "DashManifestOutputTypeDef",
-    "HlsManifestOutputTypeDef",
-    "MssManifestOutputTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsResponseTypeDef",
     "CmafEncryptionOutputTypeDef",
     "DashEncryptionOutputTypeDef",
     "HlsEncryptionOutputTypeDef",
     "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
@@ -121,22 +113,14 @@
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
     },
     total=False,
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
@@ -145,20 +129,23 @@
     "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
-EgressAccessLogsOutputTypeDef = TypedDict(
-    "EgressAccessLogsOutputTypeDef",
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
 
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
@@ -171,41 +158,29 @@
     {
         "ResourceId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAssetRequestRequestTypeDef(
     _RequiredCreateAssetRequestRequestTypeDef, _OptionalCreateAssetRequestRequestTypeDef
 ):
     pass
 
-
 EgressEndpointTypeDef = TypedDict(
     "EgressEndpointTypeDef",
     {
         "PackagingConfigurationId": str,
         "Status": str,
         "Url": str,
     },
     total=False,
 )
 
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
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -250,83 +225,52 @@
 DescribePackagingGroupRequestRequestTypeDef = TypedDict(
     "DescribePackagingGroupRequestRequestTypeDef",
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
 
-ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
-    "ListAssetsRequestListAssetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PackagingGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
-ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
-    {
-        "PackagingGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPackagingConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
-ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagingGroupsRequestRequestTypeDef = TypedDict(
     "ListPackagingGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -335,43 +279,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -380,66 +295,53 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListAssetsResponseTypeDef = TypedDict(
-    "ListAssetsResponseTypeDef",
-    {
-        "Assets": List[AssetShallowTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePackagingGroupRequestRequestTypeDef(
     _RequiredUpdatePackagingGroupRequestRequestTypeDef,
     _OptionalUpdatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredConfigureLogsRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureLogsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigureLogsRequestRequestTypeDef = TypedDict(
     "_OptionalConfigureLogsRequestRequestTypeDef",
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
     },
     total=False,
 )
 
-
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -448,92 +350,114 @@
         "Authorization": AuthorizationTypeDef,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
+PackagingGroupTypeDef = TypedDict(
+    "PackagingGroupTypeDef",
+    {
+        "ApproximateAssetCount": int,
+        "Arn": str,
+        "Authorization": AuthorizationTypeDef,
+        "CreatedAt": str,
+        "DomainName": str,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "Id": str,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
 
 ConfigureLogsResponseTypeDef = TypedDict(
     "ConfigureLogsResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackagingGroupResponseTypeDef = TypedDict(
     "CreatePackagingGroupResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagingGroupResponseTypeDef = TypedDict(
     "DescribePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PackagingGroupTypeDef = TypedDict(
-    "PackagingGroupTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssetsResponseTypeDef = TypedDict(
+    "ListAssetsResponseTypeDef",
+    {
+        "Assets": List[AssetShallowTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ApproximateAssetCount": int,
-        "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
-        "CreatedAt": str,
-        "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
-        "Id": str,
         "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 UpdatePackagingGroupResponseTypeDef = TypedDict(
     "UpdatePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -541,15 +465,15 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssetResponseTypeDef = TypedDict(
     "DescribeAssetResponseTypeDef",
     {
         "Arn": str,
@@ -557,51 +481,16 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DashManifestOutputTypeDef = TypedDict(
-    "DashManifestOutputTypeDef",
-    {
-        "ManifestLayout": ManifestLayoutType,
-        "ManifestName": str,
-        "MinBufferTimeSeconds": int,
-        "Profile": ProfileType,
-        "ScteMarkersSource": ScteMarkersSourceType,
-        "StreamSelection": StreamSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
-HlsManifestOutputTypeDef = TypedDict(
-    "HlsManifestOutputTypeDef",
-    {
-        "AdMarkers": AdMarkersType,
-        "IncludeIframeOnlyStream": bool,
-        "ManifestName": str,
-        "ProgramDateTimeIntervalSeconds": int,
-        "RepeatExtXKey": bool,
-        "StreamSelection": StreamSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
-MssManifestOutputTypeDef = TypedDict(
-    "MssManifestOutputTypeDef",
-    {
-        "ManifestName": str,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DashManifestTypeDef = TypedDict(
     "DashManifestTypeDef",
     {
         "ManifestLayout": ManifestLayoutType,
         "ManifestName": str,
@@ -642,26 +531,24 @@
         "SystemIds": List[str],
         "Url": str,
     },
 )
 _OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
     "_OptionalSpekeKeyProviderOutputTypeDef",
     {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SpekeKeyProviderOutputTypeDef(
     _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
 ):
     pass
 
-
 _RequiredSpekeKeyProviderTypeDef = TypedDict(
     "_RequiredSpekeKeyProviderTypeDef",
     {
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
@@ -670,25 +557,49 @@
     "_OptionalSpekeKeyProviderTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
+ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    {
+        "PackagingGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
+    {
+        "PackagingGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListPackagingGroupsResponseTypeDef = TypedDict(
     "ListPackagingGroupsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCmafEncryptionOutputTypeDef = TypedDict(
     "_RequiredCmafEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
@@ -698,21 +609,19 @@
     "_OptionalCmafEncryptionOutputTypeDef",
     {
         "ConstantInitializationVector": str,
     },
     total=False,
 )
 
-
 class CmafEncryptionOutputTypeDef(
     _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
 ):
     pass
 
-
 DashEncryptionOutputTypeDef = TypedDict(
     "DashEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
 
@@ -727,21 +636,19 @@
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": EncryptionMethodType,
     },
     total=False,
 )
 
-
 class HlsEncryptionOutputTypeDef(
     _RequiredHlsEncryptionOutputTypeDef, _OptionalHlsEncryptionOutputTypeDef
 ):
     pass
 
-
 MssEncryptionOutputTypeDef = TypedDict(
     "MssEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
 
@@ -755,19 +662,17 @@
     "_OptionalCmafEncryptionTypeDef",
     {
         "ConstantInitializationVector": str,
     },
     total=False,
 )
 
-
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
-
 DashEncryptionTypeDef = TypedDict(
     "DashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
@@ -782,53 +687,49 @@
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": EncryptionMethodType,
     },
     total=False,
 )
 
-
 class HlsEncryptionTypeDef(_RequiredHlsEncryptionTypeDef, _OptionalHlsEncryptionTypeDef):
     pass
 
-
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
 _RequiredCmafPackageOutputTypeDef = TypedDict(
     "_RequiredCmafPackageOutputTypeDef",
     {
-        "HlsManifests": List[HlsManifestOutputTypeDef],
+        "HlsManifests": List[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageOutputTypeDef = TypedDict(
     "_OptionalCmafPackageOutputTypeDef",
     {
         "Encryption": CmafEncryptionOutputTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
-
 class CmafPackageOutputTypeDef(
     _RequiredCmafPackageOutputTypeDef, _OptionalCmafPackageOutputTypeDef
 ):
     pass
 
-
 _RequiredDashPackageOutputTypeDef = TypedDict(
     "_RequiredDashPackageOutputTypeDef",
     {
-        "DashManifests": List[DashManifestOutputTypeDef],
+        "DashManifests": List[DashManifestTypeDef],
     },
 )
 _OptionalDashPackageOutputTypeDef = TypedDict(
     "_OptionalDashPackageOutputTypeDef",
     {
         "Encryption": DashEncryptionOutputTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
@@ -836,63 +737,57 @@
         "PeriodTriggers": List[Literal["ADS"]],
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
     },
     total=False,
 )
 
-
 class DashPackageOutputTypeDef(
     _RequiredDashPackageOutputTypeDef, _OptionalDashPackageOutputTypeDef
 ):
     pass
 
-
 _RequiredHlsPackageOutputTypeDef = TypedDict(
     "_RequiredHlsPackageOutputTypeDef",
     {
-        "HlsManifests": List[HlsManifestOutputTypeDef],
+        "HlsManifests": List[HlsManifestTypeDef],
     },
 )
 _OptionalHlsPackageOutputTypeDef = TypedDict(
     "_OptionalHlsPackageOutputTypeDef",
     {
         "Encryption": HlsEncryptionOutputTypeDef,
         "IncludeDvbSubtitles": bool,
         "SegmentDurationSeconds": int,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
-
 class HlsPackageOutputTypeDef(_RequiredHlsPackageOutputTypeDef, _OptionalHlsPackageOutputTypeDef):
     pass
 
-
 _RequiredMssPackageOutputTypeDef = TypedDict(
     "_RequiredMssPackageOutputTypeDef",
     {
-        "MssManifests": List[MssManifestOutputTypeDef],
+        "MssManifests": List[MssManifestTypeDef],
     },
 )
 _OptionalMssPackageOutputTypeDef = TypedDict(
     "_OptionalMssPackageOutputTypeDef",
     {
         "Encryption": MssEncryptionOutputTypeDef,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
-
 class MssPackageOutputTypeDef(_RequiredMssPackageOutputTypeDef, _OptionalMssPackageOutputTypeDef):
     pass
 
-
 _RequiredCmafPackageTypeDef = TypedDict(
     "_RequiredCmafPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageTypeDef = TypedDict(
@@ -901,19 +796,17 @@
         "Encryption": CmafEncryptionTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
-
 class CmafPackageTypeDef(_RequiredCmafPackageTypeDef, _OptionalCmafPackageTypeDef):
     pass
 
-
 _RequiredDashPackageTypeDef = TypedDict(
     "_RequiredDashPackageTypeDef",
     {
         "DashManifests": Sequence[DashManifestTypeDef],
     },
 )
 _OptionalDashPackageTypeDef = TypedDict(
@@ -925,19 +818,17 @@
         "PeriodTriggers": Sequence[Literal["ADS"]],
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
     },
     total=False,
 )
 
-
 class DashPackageTypeDef(_RequiredDashPackageTypeDef, _OptionalDashPackageTypeDef):
     pass
 
-
 _RequiredHlsPackageTypeDef = TypedDict(
     "_RequiredHlsPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalHlsPackageTypeDef = TypedDict(
@@ -947,19 +838,17 @@
         "IncludeDvbSubtitles": bool,
         "SegmentDurationSeconds": int,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
-
 class HlsPackageTypeDef(_RequiredHlsPackageTypeDef, _OptionalHlsPackageTypeDef):
     pass
 
-
 _RequiredMssPackageTypeDef = TypedDict(
     "_RequiredMssPackageTypeDef",
     {
         "MssManifests": Sequence[MssManifestTypeDef],
     },
 )
 _OptionalMssPackageTypeDef = TypedDict(
@@ -967,32 +856,30 @@
     {
         "Encryption": MssEncryptionTypeDef,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
-
 class MssPackageTypeDef(_RequiredMssPackageTypeDef, _OptionalMssPackageTypeDef):
     pass
 
-
 CreatePackagingConfigurationResponseTypeDef = TypedDict(
     "CreatePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
@@ -1000,15 +887,15 @@
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
@@ -1039,23 +926,21 @@
         "HlsPackage": HlsPackageTypeDef,
         "MssPackage": MssPackageTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePackagingConfigurationRequestRequestTypeDef(
     _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
     _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.pyi` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,64 +31,58 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssetShallowTypeDef",
-    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
-    "EgressAccessLogsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
-    "StreamSelectionOutputTypeDef",
     "StreamSelectionTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeletePackagingConfigurationRequestRequestTypeDef",
     "DeletePackagingGroupRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribePackagingConfigurationRequestRequestTypeDef",
     "DescribePackagingGroupRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
-    "ListAssetsRequestListAssetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssetsRequestRequestTypeDef",
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingConfigurationsRequestRequestTypeDef",
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListAssetsResponseTypeDef",
     "UpdatePackagingGroupRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
     "CreatePackagingGroupRequestRequestTypeDef",
+    "PackagingGroupTypeDef",
     "ConfigureLogsResponseTypeDef",
     "CreatePackagingGroupResponseTypeDef",
     "DescribePackagingGroupResponseTypeDef",
-    "PackagingGroupTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAssetsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
-    "DashManifestOutputTypeDef",
-    "HlsManifestOutputTypeDef",
-    "MssManifestOutputTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsResponseTypeDef",
     "CmafEncryptionOutputTypeDef",
     "DashEncryptionOutputTypeDef",
     "HlsEncryptionOutputTypeDef",
     "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
@@ -120,22 +114,14 @@
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
     },
     total=False,
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
@@ -144,20 +130,23 @@
     "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
-EgressAccessLogsOutputTypeDef = TypedDict(
-    "EgressAccessLogsOutputTypeDef",
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
 
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
@@ -170,39 +159,31 @@
     {
         "ResourceId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAssetRequestRequestTypeDef(
     _RequiredCreateAssetRequestRequestTypeDef, _OptionalCreateAssetRequestRequestTypeDef
 ):
     pass
 
+
 EgressEndpointTypeDef = TypedDict(
     "EgressEndpointTypeDef",
     {
         "PackagingConfigurationId": str,
         "Status": str,
         "Url": str,
     },
     total=False,
 )
 
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
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -247,83 +228,52 @@
 DescribePackagingGroupRequestRequestTypeDef = TypedDict(
     "DescribePackagingGroupRequestRequestTypeDef",
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
 
-ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
-    "ListAssetsRequestListAssetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PackagingGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
-ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
-    {
-        "PackagingGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPackagingConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
-ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagingGroupsRequestRequestTypeDef = TypedDict(
     "ListPackagingGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -332,43 +282,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -377,62 +298,57 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListAssetsResponseTypeDef = TypedDict(
-    "ListAssetsResponseTypeDef",
-    {
-        "Assets": List[AssetShallowTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePackagingGroupRequestRequestTypeDef(
     _RequiredUpdatePackagingGroupRequestRequestTypeDef,
     _OptionalUpdatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredConfigureLogsRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureLogsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigureLogsRequestRequestTypeDef = TypedDict(
     "_OptionalConfigureLogsRequestRequestTypeDef",
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
     },
     total=False,
 )
 
+
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -441,90 +357,116 @@
         "Authorization": AuthorizationTypeDef,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
+
+PackagingGroupTypeDef = TypedDict(
+    "PackagingGroupTypeDef",
+    {
+        "ApproximateAssetCount": int,
+        "Arn": str,
+        "Authorization": AuthorizationTypeDef,
+        "CreatedAt": str,
+        "DomainName": str,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "Id": str,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ConfigureLogsResponseTypeDef = TypedDict(
     "ConfigureLogsResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackagingGroupResponseTypeDef = TypedDict(
     "CreatePackagingGroupResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagingGroupResponseTypeDef = TypedDict(
     "DescribePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PackagingGroupTypeDef = TypedDict(
-    "PackagingGroupTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssetsResponseTypeDef = TypedDict(
+    "ListAssetsResponseTypeDef",
+    {
+        "Assets": List[AssetShallowTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ApproximateAssetCount": int,
-        "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
-        "CreatedAt": str,
-        "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
-        "Id": str,
         "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 UpdatePackagingGroupResponseTypeDef = TypedDict(
     "UpdatePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationOutputTypeDef,
+        "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -532,15 +474,15 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssetResponseTypeDef = TypedDict(
     "DescribeAssetResponseTypeDef",
     {
         "Arn": str,
@@ -548,51 +490,16 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DashManifestOutputTypeDef = TypedDict(
-    "DashManifestOutputTypeDef",
-    {
-        "ManifestLayout": ManifestLayoutType,
-        "ManifestName": str,
-        "MinBufferTimeSeconds": int,
-        "Profile": ProfileType,
-        "ScteMarkersSource": ScteMarkersSourceType,
-        "StreamSelection": StreamSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
-HlsManifestOutputTypeDef = TypedDict(
-    "HlsManifestOutputTypeDef",
-    {
-        "AdMarkers": AdMarkersType,
-        "IncludeIframeOnlyStream": bool,
-        "ManifestName": str,
-        "ProgramDateTimeIntervalSeconds": int,
-        "RepeatExtXKey": bool,
-        "StreamSelection": StreamSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
-MssManifestOutputTypeDef = TypedDict(
-    "MssManifestOutputTypeDef",
-    {
-        "ManifestName": str,
-        "StreamSelection": StreamSelectionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DashManifestTypeDef = TypedDict(
     "DashManifestTypeDef",
     {
         "ManifestLayout": ManifestLayoutType,
         "ManifestName": str,
@@ -633,24 +540,26 @@
         "SystemIds": List[str],
         "Url": str,
     },
 )
 _OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
     "_OptionalSpekeKeyProviderOutputTypeDef",
     {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SpekeKeyProviderOutputTypeDef(
     _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
 ):
     pass
 
+
 _RequiredSpekeKeyProviderTypeDef = TypedDict(
     "_RequiredSpekeKeyProviderTypeDef",
     {
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
@@ -659,23 +568,51 @@
     "_OptionalSpekeKeyProviderTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
+
+ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    {
+        "PackagingGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
+    {
+        "PackagingGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPackagingGroupsResponseTypeDef = TypedDict(
     "ListPackagingGroupsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCmafEncryptionOutputTypeDef = TypedDict(
     "_RequiredCmafEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
@@ -685,19 +622,21 @@
     "_OptionalCmafEncryptionOutputTypeDef",
     {
         "ConstantInitializationVector": str,
     },
     total=False,
 )
 
+
 class CmafEncryptionOutputTypeDef(
     _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
 ):
     pass
 
+
 DashEncryptionOutputTypeDef = TypedDict(
     "DashEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
 
@@ -712,19 +651,21 @@
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": EncryptionMethodType,
     },
     total=False,
 )
 
+
 class HlsEncryptionOutputTypeDef(
     _RequiredHlsEncryptionOutputTypeDef, _OptionalHlsEncryptionOutputTypeDef
 ):
     pass
 
+
 MssEncryptionOutputTypeDef = TypedDict(
     "MssEncryptionOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
 )
 
@@ -738,17 +679,19 @@
     "_OptionalCmafEncryptionTypeDef",
     {
         "ConstantInitializationVector": str,
     },
     total=False,
 )
 
+
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
+
 DashEncryptionTypeDef = TypedDict(
     "DashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
@@ -763,49 +706,53 @@
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": EncryptionMethodType,
     },
     total=False,
 )
 
+
 class HlsEncryptionTypeDef(_RequiredHlsEncryptionTypeDef, _OptionalHlsEncryptionTypeDef):
     pass
 
+
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
 _RequiredCmafPackageOutputTypeDef = TypedDict(
     "_RequiredCmafPackageOutputTypeDef",
     {
-        "HlsManifests": List[HlsManifestOutputTypeDef],
+        "HlsManifests": List[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageOutputTypeDef = TypedDict(
     "_OptionalCmafPackageOutputTypeDef",
     {
         "Encryption": CmafEncryptionOutputTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
+
 class CmafPackageOutputTypeDef(
     _RequiredCmafPackageOutputTypeDef, _OptionalCmafPackageOutputTypeDef
 ):
     pass
 
+
 _RequiredDashPackageOutputTypeDef = TypedDict(
     "_RequiredDashPackageOutputTypeDef",
     {
-        "DashManifests": List[DashManifestOutputTypeDef],
+        "DashManifests": List[DashManifestTypeDef],
     },
 )
 _OptionalDashPackageOutputTypeDef = TypedDict(
     "_OptionalDashPackageOutputTypeDef",
     {
         "Encryption": DashEncryptionOutputTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
@@ -813,57 +760,63 @@
         "PeriodTriggers": List[Literal["ADS"]],
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
     },
     total=False,
 )
 
+
 class DashPackageOutputTypeDef(
     _RequiredDashPackageOutputTypeDef, _OptionalDashPackageOutputTypeDef
 ):
     pass
 
+
 _RequiredHlsPackageOutputTypeDef = TypedDict(
     "_RequiredHlsPackageOutputTypeDef",
     {
-        "HlsManifests": List[HlsManifestOutputTypeDef],
+        "HlsManifests": List[HlsManifestTypeDef],
     },
 )
 _OptionalHlsPackageOutputTypeDef = TypedDict(
     "_OptionalHlsPackageOutputTypeDef",
     {
         "Encryption": HlsEncryptionOutputTypeDef,
         "IncludeDvbSubtitles": bool,
         "SegmentDurationSeconds": int,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
+
 class HlsPackageOutputTypeDef(_RequiredHlsPackageOutputTypeDef, _OptionalHlsPackageOutputTypeDef):
     pass
 
+
 _RequiredMssPackageOutputTypeDef = TypedDict(
     "_RequiredMssPackageOutputTypeDef",
     {
-        "MssManifests": List[MssManifestOutputTypeDef],
+        "MssManifests": List[MssManifestTypeDef],
     },
 )
 _OptionalMssPackageOutputTypeDef = TypedDict(
     "_OptionalMssPackageOutputTypeDef",
     {
         "Encryption": MssEncryptionOutputTypeDef,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
+
 class MssPackageOutputTypeDef(_RequiredMssPackageOutputTypeDef, _OptionalMssPackageOutputTypeDef):
     pass
 
+
 _RequiredCmafPackageTypeDef = TypedDict(
     "_RequiredCmafPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageTypeDef = TypedDict(
@@ -872,17 +825,19 @@
         "Encryption": CmafEncryptionTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
+
 class CmafPackageTypeDef(_RequiredCmafPackageTypeDef, _OptionalCmafPackageTypeDef):
     pass
 
+
 _RequiredDashPackageTypeDef = TypedDict(
     "_RequiredDashPackageTypeDef",
     {
         "DashManifests": Sequence[DashManifestTypeDef],
     },
 )
 _OptionalDashPackageTypeDef = TypedDict(
@@ -894,17 +849,19 @@
         "PeriodTriggers": Sequence[Literal["ADS"]],
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
     },
     total=False,
 )
 
+
 class DashPackageTypeDef(_RequiredDashPackageTypeDef, _OptionalDashPackageTypeDef):
     pass
 
+
 _RequiredHlsPackageTypeDef = TypedDict(
     "_RequiredHlsPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalHlsPackageTypeDef = TypedDict(
@@ -914,17 +871,19 @@
         "IncludeDvbSubtitles": bool,
         "SegmentDurationSeconds": int,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
+
 class HlsPackageTypeDef(_RequiredHlsPackageTypeDef, _OptionalHlsPackageTypeDef):
     pass
 
+
 _RequiredMssPackageTypeDef = TypedDict(
     "_RequiredMssPackageTypeDef",
     {
         "MssManifests": Sequence[MssManifestTypeDef],
     },
 )
 _OptionalMssPackageTypeDef = TypedDict(
@@ -932,30 +891,32 @@
     {
         "Encryption": MssEncryptionTypeDef,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
+
 class MssPackageTypeDef(_RequiredMssPackageTypeDef, _OptionalMssPackageTypeDef):
     pass
 
+
 CreatePackagingConfigurationResponseTypeDef = TypedDict(
     "CreatePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
@@ -963,15 +924,15 @@
         "CreatedAt": str,
         "DashPackage": DashPackageOutputTypeDef,
         "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
@@ -1002,21 +963,23 @@
         "HlsPackage": HlsPackageTypeDef,
         "MssPackage": MssPackageTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePackagingConfigurationRequestRequestTypeDef(
     _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
     _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaPackageVod 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,62 +343,55 @@
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
-    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
-    EgressAccessLogsOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
-    StreamSelectionOutputTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssetsRequestRequestTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
     CreatePackagingGroupRequestRequestTypeDef,
+    PackagingGroupTypeDef,
     ConfigureLogsResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
-    PackagingGroupTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAssetsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
-    DashManifestOutputTypeDef,
-    HlsManifestOutputTypeDef,
-    MssManifestOutputTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
+    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
+    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsResponseTypeDef,
     CmafEncryptionOutputTypeDef,
     DashEncryptionOutputTypeDef,
     HlsEncryptionOutputTypeDef,
     MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.12/setup.py` & `mypy-boto3-mediapackage-vod-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage-vod",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackageVod 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MediaPackageVod 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

