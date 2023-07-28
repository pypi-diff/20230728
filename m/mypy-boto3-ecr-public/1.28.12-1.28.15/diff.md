# Comparing `tmp/mypy-boto3-ecr-public-1.28.12.tar.gz` & `tmp/mypy-boto3-ecr-public-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-public-1.28.12.tar", last modified: Thu Jul 27 05:34:37 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-public-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
```

## Comparing `mypy-boto3-ecr-public-1.28.12.tar` & `mypy-boto3-ecr-public-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14355 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.800523 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24135 2023-07-27 05:21:31.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-07-27 05:21:31.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-07-28 20:24:47.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/setup.py
```

### Comparing `mypy-boto3-ecr-public-1.28.12/LICENSE` & `mypy-boto3-ecr-public-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/PKG-INFO` & `mypy-boto3-ecr-public-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.12
-Summary: Type annotations for boto3.ECRPublic 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,71 +343,69 @@
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
-    ImageIdentifierOutputTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.12/README.md` & `mypy-boto3-ecr-public-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,71 +311,69 @@
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
-    ImageIdentifierOutputTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.py` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.pyi` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__main__.py` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECRPublic 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ECRPublic 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.py` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.pyi` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.py` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.pyi` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.py` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 
@@ -83,30 +83,30 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagespaginator)
         """
 
 
 class DescribeRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
         """
 
 
@@ -117,13 +117,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.pyi` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 class DescribeImagesPaginator(Paginator):
@@ -79,29 +79,29 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagespaginator)
         """
 
 class DescribeRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
         """
 
 class DescribeRepositoriesPaginator(Paginator):
@@ -111,13 +111,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.py` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,71 +31,69 @@
 
 
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
-    "ImageIdentifierOutputTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
     "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
-    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
     "ImageDetailTypeDef",
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
     "DescribeRegistriesRequestRequestTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "RegistryCatalogDataTypeDef",
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "PutRepositoryCatalogDataRequestRequestTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
+    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
@@ -148,25 +146,27 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
     },
     total=False,
 )
 
-ImageIdentifierTypeDef = TypedDict(
-    "ImageIdentifierTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "imageDigest": str,
-        "imageTag": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ImageIdentifierOutputTypeDef = TypedDict(
-    "ImageIdentifierOutputTypeDef",
+ImageIdentifierTypeDef = TypedDict(
+    "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
@@ -190,25 +190,14 @@
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RepositoryCatalogDataInputTypeDef = TypedDict(
     "RepositoryCatalogDataInputTypeDef",
     {
         "description": str,
         "architectures": Sequence[str],
         "operatingSystems": Sequence[str],
         "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
@@ -271,24 +260,14 @@
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -303,37 +282,24 @@
 
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
-    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -364,41 +330,23 @@
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
         "artifactMediaType": str,
     },
     total=False,
 )
 
-DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRegistriesRequestRequestTypeDef = TypedDict(
     "DescribeRegistriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -454,24 +402,14 @@
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReferencedImageDetailTypeDef = TypedDict(
     "ReferencedImageDetailTypeDef",
     {
         "imageDigest": str,
         "imageSizeInBytes": int,
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
@@ -498,49 +436,21 @@
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -576,25 +486,14 @@
         "name": str,
         "status": RegistryAliasStatusType,
         "primaryRegistryAlias": bool,
         "defaultRegistryAlias": bool,
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -611,24 +510,14 @@
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -654,84 +543,110 @@
 
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
 
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
+    {
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": AuthorizationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
     {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeleteImageRequestRequestTypeDef",
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
     {
-        "repositoryName": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeleteImageRequestRequestTypeDef",
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class BatchDeleteImageRequestRequestTypeDef(
-    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class DescribeImagesRequestDescribeImagesPaginateTypeDef(
-    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
-    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+class BatchDeleteImageRequestRequestTypeDef(
+    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
@@ -755,27 +670,27 @@
 ):
     pass
 
 
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 _RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
@@ -819,145 +734,210 @@
 
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 GetRepositoryCatalogDataResponseTypeDef = TypedDict(
     "GetRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryCatalogDataResponseTypeDef = TypedDict(
     "PutRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
+    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "repositoryName": str,
     },
 )
+_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "registryId": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeImagesRequestDescribeImagesPaginateTypeDef(
+    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
+    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+):
+    pass
+
+
+DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegistryCatalogDataResponseTypeDef = TypedDict(
     "GetRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryCatalogDataResponseTypeDef = TypedDict(
     "PutRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTagDetailTypeDef = TypedDict(
     "ImageTagDetailTypeDef",
     {
         "imageTag": str,
         "createdAt": datetime,
         "imageDetail": ReferencedImageDetailTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegistryTypeDef = TypedDict(
     "RegistryTypeDef",
     {
         "registryId": str,
         "registryArn": str,
         "registryUri": str,
         "verified": bool,
         "aliases": List[RegistryAliasTypeDef],
     },
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierOutputTypeDef],
+        "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegistriesResponseTypeDef = TypedDict(
     "DescribeRegistriesResponseTypeDef",
     {
         "registries": List[RegistryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.pyi` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,71 +30,69 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
-    "ImageIdentifierOutputTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
     "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
-    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
     "ImageDetailTypeDef",
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
     "DescribeRegistriesRequestRequestTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "RegistryCatalogDataTypeDef",
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "PutRepositoryCatalogDataRequestRequestTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
+    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
@@ -145,25 +143,27 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
     },
     total=False,
 )
 
-ImageIdentifierTypeDef = TypedDict(
-    "ImageIdentifierTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "imageDigest": str,
-        "imageTag": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ImageIdentifierOutputTypeDef = TypedDict(
-    "ImageIdentifierOutputTypeDef",
+ImageIdentifierTypeDef = TypedDict(
+    "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
@@ -185,25 +185,14 @@
 
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RepositoryCatalogDataInputTypeDef = TypedDict(
     "RepositoryCatalogDataInputTypeDef",
     {
         "description": str,
         "architectures": Sequence[str],
         "operatingSystems": Sequence[str],
         "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
@@ -264,24 +253,14 @@
 
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -294,35 +273,24 @@
 )
 
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
-    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -351,41 +319,23 @@
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
         "artifactMediaType": str,
     },
     total=False,
 )
 
-DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRegistriesRequestRequestTypeDef = TypedDict(
     "DescribeRegistriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -437,24 +387,14 @@
 
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReferencedImageDetailTypeDef = TypedDict(
     "ReferencedImageDetailTypeDef",
     {
         "imageDigest": str,
         "imageSizeInBytes": int,
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
@@ -479,49 +419,21 @@
 
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -555,25 +467,14 @@
         "name": str,
         "status": RegistryAliasStatusType,
         "primaryRegistryAlias": bool,
         "defaultRegistryAlias": bool,
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -588,24 +489,14 @@
 
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -629,81 +520,109 @@
 )
 
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
+    {
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": AuthorizationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
     {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeleteImageRequestRequestTypeDef",
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
     {
-        "repositoryName": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeleteImageRequestRequestTypeDef",
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class BatchDeleteImageRequestRequestTypeDef(
-    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
-):
-    pass
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class DescribeImagesRequestDescribeImagesPaginateTypeDef(
-    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
-    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+class BatchDeleteImageRequestRequestTypeDef(
+    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -724,27 +643,27 @@
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 _RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
@@ -784,145 +703,206 @@
 )
 
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 GetRepositoryCatalogDataResponseTypeDef = TypedDict(
     "GetRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryCatalogDataResponseTypeDef = TypedDict(
     "PutRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
+    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "registryId": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class DescribeImagesRequestDescribeImagesPaginateTypeDef(
+    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
+    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
+):
+    pass
+
+DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegistryCatalogDataResponseTypeDef = TypedDict(
     "GetRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryCatalogDataResponseTypeDef = TypedDict(
     "PutRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTagDetailTypeDef = TypedDict(
     "ImageTagDetailTypeDef",
     {
         "imageTag": str,
         "createdAt": datetime,
         "imageDetail": ReferencedImageDetailTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegistryTypeDef = TypedDict(
     "RegistryTypeDef",
     {
         "registryId": str,
         "registryArn": str,
         "registryUri": str,
         "verified": bool,
         "aliases": List[RegistryAliasTypeDef],
     },
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierOutputTypeDef],
+        "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegistriesResponseTypeDef = TypedDict(
     "DescribeRegistriesResponseTypeDef",
     {
         "registries": List[RegistryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/PKG-INFO` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.12
-Summary: Type annotations for boto3.ECRPublic 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,71 +343,69 @@
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
-    ImageIdentifierOutputTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/SOURCES.txt` & `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.12/setup.py` & `mypy-boto3-ecr-public-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr-public",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECRPublic 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

