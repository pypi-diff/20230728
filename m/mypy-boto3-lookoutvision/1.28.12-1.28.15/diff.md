# Comparing `tmp/mypy-boto3-lookoutvision-1.28.12.tar.gz` & `tmp/mypy-boto3-lookoutvision-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutvision-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutvision-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
```

## Comparing `mypy-boto3-lookoutvision-1.28.12.tar` & `mypy-boto3-lookoutvision-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.016452 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28476 2023-07-27 05:25:40.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28429 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.873427 mypy-boto3-lookoutvision-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-07-28 20:43:11.869427 mypy-boto3-lookoutvision-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.845427 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-28 20:30:37.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-28 20:30:37.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-07-28 20:30:37.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.869427 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.873427 mypy-boto3-lookoutvision-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/setup.py
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/LICENSE` & `mypy-boto3-lookoutvision-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.12
-Summary: Type annotations for boto3.LookoutforVision 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,82 +345,78 @@
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
     DatasetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
-    DeleteModelResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
-    S3LocationOutputTypeDef,
-    TagOutputTypeDef,
-    TargetPlatformOutputTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
-    ListModelsRequestListModelsPaginateTypeDef,
     ListModelsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartModelPackagingJobResponseTypeDef,
     StartModelRequestRequestTypeDef,
-    StartModelResponseTypeDef,
     StopModelRequestRequestTypeDef,
-    StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
-    UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
-    CreateDatasetResponseTypeDef,
     ProjectDescriptionTypeDef,
+    CreateDatasetResponseTypeDef,
+    DeleteModelResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    StartModelPackagingJobResponseTypeDef,
+    StartModelResponseTypeDef,
+    StopModelResponseTypeDef,
+    UpdateDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
-    OutputConfigOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GreengrassConfigurationOutputTypeDef,
     OutputConfigTypeDef,
+    GreengrassConfigurationOutputTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    ListModelsRequestListModelsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
+    CreateModelRequestRequestTypeDef,
     ModelDescriptionTypeDef,
     ModelPackagingConfigurationOutputTypeDef,
-    CreateModelRequestRequestTypeDef,
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/README.md` & `mypy-boto3-lookoutvision-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,82 +313,78 @@
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
     DatasetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
-    DeleteModelResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
-    S3LocationOutputTypeDef,
-    TagOutputTypeDef,
-    TargetPlatformOutputTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
-    ListModelsRequestListModelsPaginateTypeDef,
     ListModelsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartModelPackagingJobResponseTypeDef,
     StartModelRequestRequestTypeDef,
-    StartModelResponseTypeDef,
     StopModelRequestRequestTypeDef,
-    StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
-    UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
-    CreateDatasetResponseTypeDef,
     ProjectDescriptionTypeDef,
+    CreateDatasetResponseTypeDef,
+    DeleteModelResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    StartModelPackagingJobResponseTypeDef,
+    StartModelResponseTypeDef,
+    StopModelResponseTypeDef,
+    UpdateDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
-    OutputConfigOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GreengrassConfigurationOutputTypeDef,
     OutputConfigTypeDef,
+    GreengrassConfigurationOutputTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    ListModelsRequestListModelsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
+    CreateModelRequestRequestTypeDef,
     ModelDescriptionTypeDef,
     ModelPackagingConfigurationOutputTypeDef,
-    CreateModelRequestRequestTypeDef,
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.py` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.pyi` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.py` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.pyi` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.py` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.pyi` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.py` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,58 +68,58 @@
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: Union[datetime, str] = ...,
         AfterCreationDate: Union[datetime, str] = ...,
         SourceRefContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listdatasetentriespaginator)
         """
 
 
 class ListModelPackagingJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelPackagingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
         """
 
 
 class ListModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.pyi` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,55 +65,55 @@
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: Union[datetime, str] = ...,
         AfterCreationDate: Union[datetime, str] = ...,
         SourceRefContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listdatasetentriespaginator)
         """
 
 class ListModelPackagingJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelPackagingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
         """
 
 class ListModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.py` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,86 +30,81 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PixelAnomalyTypeDef",
     "DatasetMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
     "InputS3ObjectTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
-    "DeleteModelResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
-    "S3LocationOutputTypeDef",
-    "TagOutputTypeDef",
-    "TargetPlatformOutputTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelPackagingJobsRequestRequestTypeDef",
     "ModelPackagingJobMetadataTypeDef",
-    "ListModelsRequestListModelsPaginateTypeDef",
     "ListModelsRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModelPerformanceTypeDef",
     "OutputS3ObjectTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartModelPackagingJobResponseTypeDef",
     "StartModelRequestRequestTypeDef",
-    "StartModelResponseTypeDef",
     "StopModelRequestRequestTypeDef",
-    "StopModelResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
-    "UpdateDatasetEntriesResponseTypeDef",
     "AnomalyTypeDef",
-    "CreateDatasetResponseTypeDef",
     "ProjectDescriptionTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "DeleteModelResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "StartModelPackagingJobResponseTypeDef",
+    "StartModelResponseTypeDef",
+    "StopModelResponseTypeDef",
+    "UpdateDatasetEntriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
-    "OutputConfigOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GreengrassConfigurationOutputTypeDef",
     "OutputConfigTypeDef",
+    "GreengrassConfigurationOutputTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    "ListModelsRequestListModelsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
+    "CreateModelRequestRequestTypeDef",
     "ModelDescriptionTypeDef",
     "ModelPackagingConfigurationOutputTypeDef",
-    "CreateModelRequestRequestTypeDef",
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
@@ -133,14 +128,25 @@
         "CreationTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -155,21 +161,19 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
 ProjectMetadataTypeDef = TypedDict(
     "ProjectMetadataTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
     },
@@ -198,19 +202,17 @@
     "_OptionalInputS3ObjectTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
-
 class InputS3ObjectTypeDef(_RequiredInputS3ObjectTypeDef, _OptionalInputS3ObjectTypeDef):
     pass
 
-
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -218,21 +220,19 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -240,58 +240,38 @@
     "_OptionalDeleteModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
-
-DeleteModelResponseTypeDef = TypedDict(
-    "DeleteModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -333,82 +313,31 @@
     "ImageSourceTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
-    pass
-
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-_RequiredTargetPlatformOutputTypeDef = TypedDict(
-    "_RequiredTargetPlatformOutputTypeDef",
-    {
-        "Os": Literal["LINUX"],
-        "Arch": TargetPlatformArchType,
-    },
-)
-_OptionalTargetPlatformOutputTypeDef = TypedDict(
-    "_OptionalTargetPlatformOutputTypeDef",
-    {
-        "Accelerator": Literal["NVIDIA"],
-    },
-    total=False,
-)
-
-
-class TargetPlatformOutputTypeDef(
-    _RequiredTargetPlatformOutputTypeDef, _OptionalTargetPlatformOutputTypeDef
-):
-    pass
-
-
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3LocationTypeDef = TypedDict(
     "_OptionalS3LocationTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": Literal["LINUX"],
         "Arch": TargetPlatformArchType,
     },
 )
@@ -416,57 +345,37 @@
     "_OptionalTargetPlatformTypeDef",
     {
         "Accelerator": Literal["NVIDIA"],
     },
     total=False,
 )
 
-
 class TargetPlatformTypeDef(_RequiredTargetPlatformTypeDef, _OptionalTargetPlatformTypeDef):
     pass
 
-
 GreengrassOutputDetailsTypeDef = TypedDict(
     "GreengrassOutputDetailsTypeDef",
     {
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "SourceRefContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -480,53 +389,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SourceRefContains": str,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
-    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -534,22 +410,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListModelPackagingJobsRequestRequestTypeDef(
     _RequiredListModelPackagingJobsRequestRequestTypeDef,
     _OptionalListModelPackagingJobsRequestRequestTypeDef,
 ):
     pass
 
-
 ModelPackagingJobMetadataTypeDef = TypedDict(
     "ModelPackagingJobMetadataTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
         "ModelPackagingJobDescription": str,
@@ -558,36 +432,14 @@
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_RequiredListModelsRequestListModelsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_OptionalListModelsRequestListModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListModelsRequestListModelsPaginateTypeDef(
-    _RequiredListModelsRequestListModelsPaginateTypeDef,
-    _OptionalListModelsRequestListModelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListModelsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestRequestTypeDef = TypedDict(
@@ -595,29 +447,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -644,43 +486,14 @@
     "OutputS3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
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
-StartModelPackagingJobResponseTypeDef = TypedDict(
-    "StartModelPackagingJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartModelRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "MinInferenceUnits": int,
     },
@@ -690,29 +503,19 @@
     {
         "ClientToken": str,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
-
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
-
-StartModelResponseTypeDef = TypedDict(
-    "StartModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopModelRequestRequestTypeDef = TypedDict(
     "_RequiredStopModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -720,29 +523,19 @@
     "_OptionalStopModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
-
-StopModelResponseTypeDef = TypedDict(
-    "StopModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -759,80 +552,135 @@
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateDatasetEntriesResponseTypeDef = TypedDict(
-    "UpdateDatasetEntriesResponseTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnomalyTypeDef = TypedDict(
     "AnomalyTypeDef",
     {
         "Name": str,
         "PixelAnomaly": PixelAnomalyTypeDef,
     },
     total=False,
 )
 
+ProjectDescriptionTypeDef = TypedDict(
+    "ProjectDescriptionTypeDef",
+    {
+        "ProjectArn": str,
+        "ProjectName": str,
+        "CreationTimestamp": datetime,
+        "Datasets": List[DatasetMetadataTypeDef],
+    },
+    total=False,
+)
+
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "DatasetMetadata": DatasetMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectDescriptionTypeDef = TypedDict(
-    "ProjectDescriptionTypeDef",
+DeleteModelResponseTypeDef = TypedDict(
+    "DeleteModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
     {
         "ProjectArn": str,
-        "ProjectName": str,
-        "CreationTimestamp": datetime,
-        "Datasets": List[DatasetMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartModelPackagingJobResponseTypeDef = TypedDict(
+    "StartModelPackagingJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartModelResponseTypeDef = TypedDict(
+    "StartModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopModelResponseTypeDef = TypedDict(
+    "StopModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDatasetEntriesResponseTypeDef = TypedDict(
+    "UpdateDatasetEntriesResponseTypeDef",
+    {
+        "Status": DatasetStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "ProjectMetadata": ProjectMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "ProjectName": str,
@@ -850,63 +698,46 @@
     "DatasetGroundTruthManifestTypeDef",
     {
         "S3Object": InputS3ObjectTypeDef,
     },
     total=False,
 )
 
-OutputConfigOutputTypeDef = TypedDict(
-    "OutputConfigOutputTypeDef",
-    {
-        "S3Location": S3LocationOutputTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+OutputConfigTypeDef = TypedDict(
+    "OutputConfigTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Location": S3LocationTypeDef,
     },
 )
 
 _RequiredGreengrassConfigurationOutputTypeDef = TypedDict(
     "_RequiredGreengrassConfigurationOutputTypeDef",
     {
-        "S3OutputLocation": S3LocationOutputTypeDef,
+        "S3OutputLocation": S3LocationTypeDef,
         "ComponentName": str,
     },
 )
 _OptionalGreengrassConfigurationOutputTypeDef = TypedDict(
     "_OptionalGreengrassConfigurationOutputTypeDef",
     {
         "CompilerOptions": str,
         "TargetDevice": Literal["jetson_xavier"],
-        "TargetPlatform": TargetPlatformOutputTypeDef,
+        "TargetPlatform": TargetPlatformTypeDef,
         "ComponentVersion": str,
         "ComponentDescription": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class GreengrassConfigurationOutputTypeDef(
     _RequiredGreengrassConfigurationOutputTypeDef, _OptionalGreengrassConfigurationOutputTypeDef
 ):
     pass
 
-
-OutputConfigTypeDef = TypedDict(
-    "OutputConfigTypeDef",
-    {
-        "S3Location": S3LocationTypeDef,
-    },
-)
-
 _RequiredGreengrassConfigurationTypeDef = TypedDict(
     "_RequiredGreengrassConfigurationTypeDef",
     {
         "S3OutputLocation": S3LocationTypeDef,
         "ComponentName": str,
     },
 )
@@ -919,35 +750,107 @@
         "ComponentVersion": str,
         "ComponentDescription": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class GreengrassConfigurationTypeDef(
     _RequiredGreengrassConfigurationTypeDef, _OptionalGreengrassConfigurationTypeDef
 ):
     pass
 
-
 ModelPackagingOutputDetailsTypeDef = TypedDict(
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": Union[datetime, str],
+        "AfterCreationDate": Union[datetime, str],
+        "SourceRefContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
+    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_RequiredListModelsRequestListModelsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_OptionalListModelsRequestListModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListModelsRequestListModelsPaginateTypeDef(
+    _RequiredListModelsRequestListModelsPaginateTypeDef,
+    _OptionalListModelsRequestListModelsPaginateTypeDef,
+):
+    pass
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelMetadataTypeDef = TypedDict(
     "ModelMetadataTypeDef",
     {
         "CreationTimestamp": datetime,
@@ -973,45 +876,68 @@
     total=False,
 )
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "ProjectDescription": ProjectDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetSourceTypeDef = TypedDict(
     "DatasetSourceTypeDef",
     {
         "GroundTruthManifest": DatasetGroundTruthManifestTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateModelRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateModelRequestRequestTypeDef",
+    {
+        "ProjectName": str,
+        "OutputConfig": OutputConfigTypeDef,
+    },
+)
+_OptionalCreateModelRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateModelRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ClientToken": str,
+        "KmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateModelRequestRequestTypeDef(
+    _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
+):
+    pass
+
 ModelDescriptionTypeDef = TypedDict(
     "ModelDescriptionTypeDef",
     {
         "ModelVersion": str,
         "ModelArn": str,
         "CreationTimestamp": datetime,
         "Description": str,
         "Status": ModelStatusType,
         "StatusMessage": str,
         "Performance": ModelPerformanceTypeDef,
-        "OutputConfig": OutputConfigOutputTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
         "EvaluationManifest": OutputS3ObjectTypeDef,
         "EvaluationResult": OutputS3ObjectTypeDef,
         "EvaluationEndTimestamp": datetime,
         "KmsKeyId": str,
         "MinInferenceUnits": int,
         "MaxInferenceUnits": int,
     },
@@ -1021,68 +947,43 @@
 ModelPackagingConfigurationOutputTypeDef = TypedDict(
     "ModelPackagingConfigurationOutputTypeDef",
     {
         "Greengrass": GreengrassConfigurationOutputTypeDef,
     },
 )
 
-_RequiredCreateModelRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateModelRequestRequestTypeDef",
-    {
-        "ProjectName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateModelRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateModelRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ClientToken": str,
-        "KmsKeyId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateModelRequestRequestTypeDef(
-    _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
-):
-    pass
-
-
 ModelPackagingConfigurationTypeDef = TypedDict(
     "ModelPackagingConfigurationTypeDef",
     {
         "Greengrass": GreengrassConfigurationTypeDef,
     },
 )
 
 CreateModelResponseTypeDef = TypedDict(
     "CreateModelResponseTypeDef",
     {
         "ModelMetadata": ModelMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "Models": List[ModelMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectAnomaliesResponseTypeDef = TypedDict(
     "DetectAnomaliesResponseTypeDef",
     {
         "DetectAnomalyResult": DetectAnomalyResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
@@ -1094,26 +995,24 @@
     {
         "DatasetSource": DatasetSourceTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
@@ -1145,22 +1044,20 @@
         "JobName": str,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartModelPackagingJobRequestRequestTypeDef(
     _RequiredStartModelPackagingJobRequestRequestTypeDef,
     _OptionalStartModelPackagingJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.pyi` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,85 +30,82 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "PixelAnomalyTypeDef",
     "DatasetMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
     "InputS3ObjectTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
-    "DeleteModelResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
-    "S3LocationOutputTypeDef",
-    "TagOutputTypeDef",
-    "TargetPlatformOutputTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelPackagingJobsRequestRequestTypeDef",
     "ModelPackagingJobMetadataTypeDef",
-    "ListModelsRequestListModelsPaginateTypeDef",
     "ListModelsRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModelPerformanceTypeDef",
     "OutputS3ObjectTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartModelPackagingJobResponseTypeDef",
     "StartModelRequestRequestTypeDef",
-    "StartModelResponseTypeDef",
     "StopModelRequestRequestTypeDef",
-    "StopModelResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
-    "UpdateDatasetEntriesResponseTypeDef",
     "AnomalyTypeDef",
-    "CreateDatasetResponseTypeDef",
     "ProjectDescriptionTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "DeleteModelResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "StartModelPackagingJobResponseTypeDef",
+    "StartModelResponseTypeDef",
+    "StopModelResponseTypeDef",
+    "UpdateDatasetEntriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
-    "OutputConfigOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GreengrassConfigurationOutputTypeDef",
     "OutputConfigTypeDef",
+    "GreengrassConfigurationOutputTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    "ListModelsRequestListModelsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
+    "CreateModelRequestRequestTypeDef",
     "ModelDescriptionTypeDef",
     "ModelPackagingConfigurationOutputTypeDef",
-    "CreateModelRequestRequestTypeDef",
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
@@ -132,14 +129,25 @@
         "CreationTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -154,19 +162,21 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
 ProjectMetadataTypeDef = TypedDict(
     "ProjectMetadataTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
     },
@@ -195,17 +205,19 @@
     "_OptionalInputS3ObjectTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
+
 class InputS3ObjectTypeDef(_RequiredInputS3ObjectTypeDef, _OptionalInputS3ObjectTypeDef):
     pass
 
+
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -213,19 +225,21 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -233,26 +247,20 @@
     "_OptionalDeleteModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
-DeleteModelResponseTypeDef = TypedDict(
-    "DeleteModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
@@ -260,26 +268,20 @@
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
@@ -322,76 +324,33 @@
     "ImageSourceTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
-    pass
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-_RequiredTargetPlatformOutputTypeDef = TypedDict(
-    "_RequiredTargetPlatformOutputTypeDef",
-    {
-        "Os": Literal["LINUX"],
-        "Arch": TargetPlatformArchType,
-    },
-)
-_OptionalTargetPlatformOutputTypeDef = TypedDict(
-    "_OptionalTargetPlatformOutputTypeDef",
-    {
-        "Accelerator": Literal["NVIDIA"],
-    },
-    total=False,
-)
-
-class TargetPlatformOutputTypeDef(
-    _RequiredTargetPlatformOutputTypeDef, _OptionalTargetPlatformOutputTypeDef
-):
-    pass
-
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3LocationTypeDef = TypedDict(
     "_OptionalS3LocationTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": Literal["LINUX"],
         "Arch": TargetPlatformArchType,
     },
 )
@@ -399,53 +358,39 @@
     "_OptionalTargetPlatformTypeDef",
     {
         "Accelerator": Literal["NVIDIA"],
     },
     total=False,
 )
 
+
 class TargetPlatformTypeDef(_RequiredTargetPlatformTypeDef, _OptionalTargetPlatformTypeDef):
     pass
 
+
 GreengrassOutputDetailsTypeDef = TypedDict(
     "GreengrassOutputDetailsTypeDef",
     {
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "SourceRefContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -459,48 +404,21 @@
         "NextToken": str,
         "MaxResults": int,
         "SourceRefContains": str,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
-    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-):
-    pass
 
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
@@ -509,20 +427,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListModelPackagingJobsRequestRequestTypeDef(
     _RequiredListModelPackagingJobsRequestRequestTypeDef,
     _OptionalListModelPackagingJobsRequestRequestTypeDef,
 ):
     pass
 
+
 ModelPackagingJobMetadataTypeDef = TypedDict(
     "ModelPackagingJobMetadataTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
         "ModelPackagingJobDescription": str,
@@ -531,34 +451,14 @@
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_RequiredListModelsRequestListModelsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_OptionalListModelsRequestListModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListModelsRequestListModelsPaginateTypeDef(
-    _RequiredListModelsRequestListModelsPaginateTypeDef,
-    _OptionalListModelsRequestListModelsPaginateTypeDef,
-):
-    pass
-
 _RequiredListModelsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestRequestTypeDef = TypedDict(
@@ -566,26 +466,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
@@ -613,43 +507,14 @@
     "OutputS3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
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
-StartModelPackagingJobResponseTypeDef = TypedDict(
-    "StartModelPackagingJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartModelRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "MinInferenceUnits": int,
     },
@@ -659,26 +524,20 @@
     {
         "ClientToken": str,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
+
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
-StartModelResponseTypeDef = TypedDict(
-    "StartModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStopModelRequestRequestTypeDef = TypedDict(
     "_RequiredStopModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
@@ -687,26 +546,20 @@
     "_OptionalStopModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
-StopModelResponseTypeDef = TypedDict(
-    "StopModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
@@ -724,78 +577,137 @@
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-UpdateDatasetEntriesResponseTypeDef = TypedDict(
-    "UpdateDatasetEntriesResponseTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AnomalyTypeDef = TypedDict(
     "AnomalyTypeDef",
     {
         "Name": str,
         "PixelAnomaly": PixelAnomalyTypeDef,
     },
     total=False,
 )
 
+ProjectDescriptionTypeDef = TypedDict(
+    "ProjectDescriptionTypeDef",
+    {
+        "ProjectArn": str,
+        "ProjectName": str,
+        "CreationTimestamp": datetime,
+        "Datasets": List[DatasetMetadataTypeDef],
+    },
+    total=False,
+)
+
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "DatasetMetadata": DatasetMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectDescriptionTypeDef = TypedDict(
-    "ProjectDescriptionTypeDef",
+DeleteModelResponseTypeDef = TypedDict(
+    "DeleteModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
     {
         "ProjectArn": str,
-        "ProjectName": str,
-        "CreationTimestamp": datetime,
-        "Datasets": List[DatasetMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartModelPackagingJobResponseTypeDef = TypedDict(
+    "StartModelPackagingJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartModelResponseTypeDef = TypedDict(
+    "StartModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopModelResponseTypeDef = TypedDict(
+    "StopModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDatasetEntriesResponseTypeDef = TypedDict(
+    "UpdateDatasetEntriesResponseTypeDef",
+    {
+        "Status": DatasetStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "ProjectMetadata": ProjectMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "ProjectName": str,
@@ -813,60 +725,47 @@
     "DatasetGroundTruthManifestTypeDef",
     {
         "S3Object": InputS3ObjectTypeDef,
     },
     total=False,
 )
 
-OutputConfigOutputTypeDef = TypedDict(
-    "OutputConfigOutputTypeDef",
-    {
-        "S3Location": S3LocationOutputTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+OutputConfigTypeDef = TypedDict(
+    "OutputConfigTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Location": S3LocationTypeDef,
     },
 )
 
 _RequiredGreengrassConfigurationOutputTypeDef = TypedDict(
     "_RequiredGreengrassConfigurationOutputTypeDef",
     {
-        "S3OutputLocation": S3LocationOutputTypeDef,
+        "S3OutputLocation": S3LocationTypeDef,
         "ComponentName": str,
     },
 )
 _OptionalGreengrassConfigurationOutputTypeDef = TypedDict(
     "_OptionalGreengrassConfigurationOutputTypeDef",
     {
         "CompilerOptions": str,
         "TargetDevice": Literal["jetson_xavier"],
-        "TargetPlatform": TargetPlatformOutputTypeDef,
+        "TargetPlatform": TargetPlatformTypeDef,
         "ComponentVersion": str,
         "ComponentDescription": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class GreengrassConfigurationOutputTypeDef(
     _RequiredGreengrassConfigurationOutputTypeDef, _OptionalGreengrassConfigurationOutputTypeDef
 ):
     pass
 
-OutputConfigTypeDef = TypedDict(
-    "OutputConfigTypeDef",
-    {
-        "S3Location": S3LocationTypeDef,
-    },
-)
 
 _RequiredGreengrassConfigurationTypeDef = TypedDict(
     "_RequiredGreengrassConfigurationTypeDef",
     {
         "S3OutputLocation": S3LocationTypeDef,
         "ComponentName": str,
     },
@@ -880,33 +779,115 @@
         "ComponentVersion": str,
         "ComponentDescription": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class GreengrassConfigurationTypeDef(
     _RequiredGreengrassConfigurationTypeDef, _OptionalGreengrassConfigurationTypeDef
 ):
     pass
 
+
 ModelPackagingOutputDetailsTypeDef = TypedDict(
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": Union[datetime, str],
+        "AfterCreationDate": Union[datetime, str],
+        "SourceRefContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
+    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_RequiredListModelsRequestListModelsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_OptionalListModelsRequestListModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListModelsRequestListModelsPaginateTypeDef(
+    _RequiredListModelsRequestListModelsPaginateTypeDef,
+    _OptionalListModelsRequestListModelsPaginateTypeDef,
+):
+    pass
+
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelMetadataTypeDef = TypedDict(
     "ModelMetadataTypeDef",
     {
         "CreationTimestamp": datetime,
@@ -932,45 +913,70 @@
     total=False,
 )
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "ProjectDescription": ProjectDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetSourceTypeDef = TypedDict(
     "DatasetSourceTypeDef",
     {
         "GroundTruthManifest": DatasetGroundTruthManifestTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateModelRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateModelRequestRequestTypeDef",
+    {
+        "ProjectName": str,
+        "OutputConfig": OutputConfigTypeDef,
+    },
+)
+_OptionalCreateModelRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateModelRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ClientToken": str,
+        "KmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateModelRequestRequestTypeDef(
+    _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
+):
+    pass
+
+
 ModelDescriptionTypeDef = TypedDict(
     "ModelDescriptionTypeDef",
     {
         "ModelVersion": str,
         "ModelArn": str,
         "CreationTimestamp": datetime,
         "Description": str,
         "Status": ModelStatusType,
         "StatusMessage": str,
         "Performance": ModelPerformanceTypeDef,
-        "OutputConfig": OutputConfigOutputTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
         "EvaluationManifest": OutputS3ObjectTypeDef,
         "EvaluationResult": OutputS3ObjectTypeDef,
         "EvaluationEndTimestamp": datetime,
         "KmsKeyId": str,
         "MinInferenceUnits": int,
         "MaxInferenceUnits": int,
     },
@@ -980,66 +986,43 @@
 ModelPackagingConfigurationOutputTypeDef = TypedDict(
     "ModelPackagingConfigurationOutputTypeDef",
     {
         "Greengrass": GreengrassConfigurationOutputTypeDef,
     },
 )
 
-_RequiredCreateModelRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateModelRequestRequestTypeDef",
-    {
-        "ProjectName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateModelRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateModelRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ClientToken": str,
-        "KmsKeyId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateModelRequestRequestTypeDef(
-    _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
-):
-    pass
-
 ModelPackagingConfigurationTypeDef = TypedDict(
     "ModelPackagingConfigurationTypeDef",
     {
         "Greengrass": GreengrassConfigurationTypeDef,
     },
 )
 
 CreateModelResponseTypeDef = TypedDict(
     "CreateModelResponseTypeDef",
     {
         "ModelMetadata": ModelMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "Models": List[ModelMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectAnomaliesResponseTypeDef = TypedDict(
     "DetectAnomaliesResponseTypeDef",
     {
         "DetectAnomalyResult": DetectAnomalyResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
@@ -1051,24 +1034,26 @@
     {
         "DatasetSource": DatasetSourceTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
@@ -1100,20 +1085,22 @@
         "JobName": str,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartModelPackagingJobRequestRequestTypeDef(
     _RequiredStartModelPackagingJobRequestRequestTypeDef,
     _OptionalStartModelPackagingJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.12
-Summary: Type annotations for boto3.LookoutforVision 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,82 +345,78 @@
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
     DatasetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
-    DeleteModelResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
-    S3LocationOutputTypeDef,
-    TagOutputTypeDef,
-    TargetPlatformOutputTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
-    ListModelsRequestListModelsPaginateTypeDef,
     ListModelsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartModelPackagingJobResponseTypeDef,
     StartModelRequestRequestTypeDef,
-    StartModelResponseTypeDef,
     StopModelRequestRequestTypeDef,
-    StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
-    UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
-    CreateDatasetResponseTypeDef,
     ProjectDescriptionTypeDef,
+    CreateDatasetResponseTypeDef,
+    DeleteModelResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    StartModelPackagingJobResponseTypeDef,
+    StartModelResponseTypeDef,
+    StopModelResponseTypeDef,
+    UpdateDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
-    OutputConfigOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GreengrassConfigurationOutputTypeDef,
     OutputConfigTypeDef,
+    GreengrassConfigurationOutputTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    ListModelsRequestListModelsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
+    CreateModelRequestRequestTypeDef,
     ModelDescriptionTypeDef,
     ModelPackagingConfigurationOutputTypeDef,
-    CreateModelRequestRequestTypeDef,
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
```

### Comparing `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/SOURCES.txt` & `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.12/setup.py` & `mypy-boto3-lookoutvision-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutvision",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutforVision 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LookoutforVision 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

