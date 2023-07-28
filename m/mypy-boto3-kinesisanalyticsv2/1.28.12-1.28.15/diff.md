# Comparing `tmp/mypy-boto3-kinesisanalyticsv2-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesisanalyticsv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.12.tar", last modified: Thu Jul 27 05:34:54 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12.tar` & `mypy-boto3-kinesisanalyticsv2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.240465 mypy-boto3-kinesisanalyticsv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-07-27 05:34:54.228466 mypy-boto3-kinesisanalyticsv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.228466 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-27 05:24:45.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74032 2023-07-27 05:24:47.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73919 2023-07-27 05:24:47.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.228466 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:54.240465 mypy-boto3-kinesisanalyticsv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-28 20:29:19.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69775 2023-07-28 20:29:23.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69672 2023-07-28 20:29:22.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/LICENSE` & `mypy-boto3-kinesisanalyticsv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,136 +342,124 @@
 `mypy_boto3_kinesisanalyticsv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
-    ApplicationRestoreConfigurationOutputTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
-    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
-    CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
-    MavenReferenceOutputTypeDef,
-    S3ContentLocationOutputTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteApplicationSnapshotRequestRequestTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
-    DeleteApplicationVpcConfigurationResponseTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
-    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
     PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
-    FlinkRunConfigurationOutputTypeDef,
     FlinkRunConfigurationTypeDef,
-    InputParallelismOutputTypeDef,
-    InputStartingPositionConfigurationOutputTypeDef,
+    InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
     InputLambdaProcessorDescriptionTypeDef,
     InputLambdaProcessorTypeDef,
     InputLambdaProcessorUpdateTypeDef,
-    InputParallelismTypeDef,
     InputParallelismUpdateTypeDef,
     RecordColumnTypeDef,
     KinesisFirehoseInputTypeDef,
     KinesisStreamsInputTypeDef,
     KinesisFirehoseInputUpdateTypeDef,
     KinesisStreamsInputUpdateTypeDef,
-    JSONMappingParametersOutputTypeDef,
     JSONMappingParametersTypeDef,
     KinesisFirehoseOutputDescriptionTypeDef,
     KinesisFirehoseOutputTypeDef,
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
-    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ZeppelinMonitoringConfigurationDescriptionTypeDef,
     ZeppelinMonitoringConfigurationTypeDef,
     ZeppelinMonitoringConfigurationUpdateTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
+    CreateApplicationPresignedUrlResponseTypeDef,
     DeleteApplicationCloudWatchLoggingOptionResponseTypeDef,
+    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
+    DeleteApplicationOutputResponseTypeDef,
+    DeleteApplicationReferenceDataSourceResponseTypeDef,
+    DeleteApplicationVpcConfigurationResponseTypeDef,
     AddApplicationVpcConfigurationRequestRequestTypeDef,
     AddApplicationVpcConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
     CatalogConfigurationTypeDef,
     CatalogConfigurationUpdateTypeDef,
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
@@ -484,42 +472,41 @@
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
     AddApplicationInputProcessingConfigurationResponseTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
-    SourceSchemaOutputTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
+    InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
-    InputUpdateTypeDef,
     InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
     AddApplicationInputRequestRequestTypeDef,
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/README.md` & `mypy-boto3-kinesisanalyticsv2-1.28.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,136 +310,124 @@
 `mypy_boto3_kinesisanalyticsv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
-    ApplicationRestoreConfigurationOutputTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
-    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
-    CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
-    MavenReferenceOutputTypeDef,
-    S3ContentLocationOutputTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteApplicationSnapshotRequestRequestTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
-    DeleteApplicationVpcConfigurationResponseTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
-    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
     PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
-    FlinkRunConfigurationOutputTypeDef,
     FlinkRunConfigurationTypeDef,
-    InputParallelismOutputTypeDef,
-    InputStartingPositionConfigurationOutputTypeDef,
+    InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
     InputLambdaProcessorDescriptionTypeDef,
     InputLambdaProcessorTypeDef,
     InputLambdaProcessorUpdateTypeDef,
-    InputParallelismTypeDef,
     InputParallelismUpdateTypeDef,
     RecordColumnTypeDef,
     KinesisFirehoseInputTypeDef,
     KinesisStreamsInputTypeDef,
     KinesisFirehoseInputUpdateTypeDef,
     KinesisStreamsInputUpdateTypeDef,
-    JSONMappingParametersOutputTypeDef,
     JSONMappingParametersTypeDef,
     KinesisFirehoseOutputDescriptionTypeDef,
     KinesisFirehoseOutputTypeDef,
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
-    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ZeppelinMonitoringConfigurationDescriptionTypeDef,
     ZeppelinMonitoringConfigurationTypeDef,
     ZeppelinMonitoringConfigurationUpdateTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
+    CreateApplicationPresignedUrlResponseTypeDef,
     DeleteApplicationCloudWatchLoggingOptionResponseTypeDef,
+    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
+    DeleteApplicationOutputResponseTypeDef,
+    DeleteApplicationReferenceDataSourceResponseTypeDef,
+    DeleteApplicationVpcConfigurationResponseTypeDef,
     AddApplicationVpcConfigurationRequestRequestTypeDef,
     AddApplicationVpcConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
     CatalogConfigurationTypeDef,
     CatalogConfigurationUpdateTypeDef,
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
@@ -452,42 +440,41 @@
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
     AddApplicationInputProcessingConfigurationResponseTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
-    SourceSchemaOutputTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
+    InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
-    InputUpdateTypeDef,
     InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
     AddApplicationInputRequestRequestTypeDef,
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__main__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListApplicationSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
     """
 
     def paginate(
-        self, *, ApplicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
         """
 
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListApplicationSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
     """
 
     def paginate(
-        self, *, ApplicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,136 +38,124 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationTypeDef",
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
-    "ApplicationRestoreConfigurationOutputTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
-    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "S3ApplicationCodeLocationDescriptionTypeDef",
     "S3ContentLocationTypeDef",
     "S3ContentLocationUpdateTypeDef",
     "CreateApplicationPresignedUrlRequestRequestTypeDef",
-    "CreateApplicationPresignedUrlResponseTypeDef",
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
-    "MavenReferenceOutputTypeDef",
-    "S3ContentLocationOutputTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
-    "DeleteApplicationOutputResponseTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteApplicationSnapshotRequestRequestTypeDef",
     "DeleteApplicationVpcConfigurationRequestRequestTypeDef",
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
-    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
     "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
-    "FlinkRunConfigurationOutputTypeDef",
     "FlinkRunConfigurationTypeDef",
-    "InputParallelismOutputTypeDef",
-    "InputStartingPositionConfigurationOutputTypeDef",
+    "InputParallelismTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
     "InputLambdaProcessorDescriptionTypeDef",
     "InputLambdaProcessorTypeDef",
     "InputLambdaProcessorUpdateTypeDef",
-    "InputParallelismTypeDef",
     "InputParallelismUpdateTypeDef",
     "RecordColumnTypeDef",
     "KinesisFirehoseInputTypeDef",
     "KinesisStreamsInputTypeDef",
     "KinesisFirehoseInputUpdateTypeDef",
     "KinesisStreamsInputUpdateTypeDef",
-    "JSONMappingParametersOutputTypeDef",
     "JSONMappingParametersTypeDef",
     "KinesisFirehoseOutputDescriptionTypeDef",
     "KinesisFirehoseOutputTypeDef",
     "KinesisFirehoseOutputUpdateTypeDef",
     "KinesisStreamsOutputDescriptionTypeDef",
     "KinesisStreamsOutputTypeDef",
     "KinesisStreamsOutputUpdateTypeDef",
     "LambdaOutputDescriptionTypeDef",
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
-    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationSnapshotsRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ZeppelinMonitoringConfigurationDescriptionTypeDef",
     "ZeppelinMonitoringConfigurationTypeDef",
     "ZeppelinMonitoringConfigurationUpdateTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "CreateApplicationPresignedUrlResponseTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    "DeleteApplicationOutputResponseTypeDef",
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "AddApplicationVpcConfigurationRequestRequestTypeDef",
     "AddApplicationVpcConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "CatalogConfigurationDescriptionTypeDef",
     "CatalogConfigurationTypeDef",
     "CatalogConfigurationUpdateTypeDef",
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
@@ -180,42 +168,41 @@
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
-    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ApplicationCodeConfigurationDescriptionTypeDef",
     "ApplicationCodeConfigurationTypeDef",
     "ApplicationCodeConfigurationUpdateTypeDef",
     "ZeppelinApplicationConfigurationDescriptionTypeDef",
     "ZeppelinApplicationConfigurationTypeDef",
     "ZeppelinApplicationConfigurationUpdateTypeDef",
     "RunConfigurationTypeDef",
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
-    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "SourceSchemaOutputTypeDef",
     "InputSchemaUpdateTypeDef",
+    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
+    "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
-    "InputUpdateTypeDef",
     "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
@@ -261,14 +248,25 @@
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
 
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
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -337,36 +335,14 @@
 ApplicationMaintenanceConfigurationUpdateTypeDef = TypedDict(
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     {
         "ApplicationMaintenanceWindowStartTimeUpdate": str,
     },
 )
 
-_RequiredApplicationRestoreConfigurationOutputTypeDef = TypedDict(
-    "_RequiredApplicationRestoreConfigurationOutputTypeDef",
-    {
-        "ApplicationRestoreType": ApplicationRestoreTypeType,
-    },
-)
-_OptionalApplicationRestoreConfigurationOutputTypeDef = TypedDict(
-    "_OptionalApplicationRestoreConfigurationOutputTypeDef",
-    {
-        "SnapshotName": str,
-    },
-    total=False,
-)
-
-
-class ApplicationRestoreConfigurationOutputTypeDef(
-    _RequiredApplicationRestoreConfigurationOutputTypeDef,
-    _OptionalApplicationRestoreConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredApplicationRestoreConfigurationTypeDef = TypedDict(
     "_RequiredApplicationRestoreConfigurationTypeDef",
     {
         "ApplicationRestoreType": ApplicationRestoreTypeType,
     },
 )
 _OptionalApplicationRestoreConfigurationTypeDef = TypedDict(
@@ -413,22 +389,14 @@
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
-CSVMappingParametersOutputTypeDef = TypedDict(
-    "CSVMappingParametersOutputTypeDef",
-    {
-        "RecordRowDelimiter": str,
-        "RecordColumnDelimiter": str,
-    },
-)
-
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -594,22 +562,14 @@
 class CreateApplicationPresignedUrlRequestRequestTypeDef(
     _RequiredCreateApplicationPresignedUrlRequestRequestTypeDef,
     _OptionalCreateApplicationPresignedUrlRequestRequestTypeDef,
 ):
     pass
 
 
-CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
-    "CreateApplicationPresignedUrlResponseTypeDef",
-    {
-        "AuthorizedUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -629,45 +589,14 @@
     "CreateApplicationSnapshotRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "SnapshotName": str,
     },
 )
 
-MavenReferenceOutputTypeDef = TypedDict(
-    "MavenReferenceOutputTypeDef",
-    {
-        "GroupId": str,
-        "ArtifactId": str,
-        "Version": str,
-    },
-)
-
-_RequiredS3ContentLocationOutputTypeDef = TypedDict(
-    "_RequiredS3ContentLocationOutputTypeDef",
-    {
-        "BucketARN": str,
-        "FileKey": str,
-    },
-)
-_OptionalS3ContentLocationOutputTypeDef = TypedDict(
-    "_OptionalS3ContentLocationOutputTypeDef",
-    {
-        "ObjectVersion": str,
-    },
-    total=False,
-)
-
-
-class S3ContentLocationOutputTypeDef(
-    _RequiredS3ContentLocationOutputTypeDef, _OptionalS3ContentLocationOutputTypeDef
-):
-    pass
-
-
 MavenReferenceTypeDef = TypedDict(
     "MavenReferenceTypeDef",
     {
         "GroupId": str,
         "ArtifactId": str,
         "Version": str,
     },
@@ -702,59 +631,32 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "InputId": str,
     },
 )
 
-DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationOutputRequestRequestTypeDef = TypedDict(
     "DeleteApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "OutputId": str,
     },
 )
 
-DeleteApplicationOutputResponseTypeDef = TypedDict(
-    "DeleteApplicationOutputResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CreateTimestamp": Union[datetime, str],
     },
 )
@@ -788,23 +690,14 @@
 class DeleteApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalDeleteApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ContentBaseLocationDescriptionTypeDef = TypedDict(
     "_RequiredS3ContentBaseLocationDescriptionTypeDef",
     {
         "BucketARN": str,
     },
 )
 _OptionalS3ContentBaseLocationDescriptionTypeDef = TypedDict(
@@ -908,21 +801,14 @@
     "DescribeApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "ApplicationVersionId": int,
     },
 )
 
-DestinationSchemaOutputTypeDef = TypedDict(
-    "DestinationSchemaOutputTypeDef",
-    {
-        "RecordFormatType": RecordFormatTypeType,
-    },
-)
-
 DestinationSchemaTypeDef = TypedDict(
     "DestinationSchemaTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 
@@ -1042,46 +928,30 @@
         "ParallelismUpdate": int,
         "ParallelismPerKPUUpdate": int,
         "AutoScalingEnabledUpdate": bool,
     },
     total=False,
 )
 
-FlinkRunConfigurationOutputTypeDef = TypedDict(
-    "FlinkRunConfigurationOutputTypeDef",
-    {
-        "AllowNonRestoredState": bool,
-    },
-    total=False,
-)
-
 FlinkRunConfigurationTypeDef = TypedDict(
     "FlinkRunConfigurationTypeDef",
     {
         "AllowNonRestoredState": bool,
     },
     total=False,
 )
 
-InputParallelismOutputTypeDef = TypedDict(
-    "InputParallelismOutputTypeDef",
+InputParallelismTypeDef = TypedDict(
+    "InputParallelismTypeDef",
     {
         "Count": int,
     },
     total=False,
 )
 
-InputStartingPositionConfigurationOutputTypeDef = TypedDict(
-    "InputStartingPositionConfigurationOutputTypeDef",
-    {
-        "InputStartingPosition": InputStartingPositionType,
-    },
-    total=False,
-)
-
 _RequiredKinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "_RequiredKinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalKinesisFirehoseInputDescriptionTypeDef = TypedDict(
@@ -1151,22 +1021,14 @@
 InputLambdaProcessorUpdateTypeDef = TypedDict(
     "InputLambdaProcessorUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-InputParallelismTypeDef = TypedDict(
-    "InputParallelismTypeDef",
-    {
-        "Count": int,
-    },
-    total=False,
-)
-
 InputParallelismUpdateTypeDef = TypedDict(
     "InputParallelismUpdateTypeDef",
     {
         "CountUpdate": int,
     },
 )
 
@@ -1214,21 +1076,14 @@
 KinesisStreamsInputUpdateTypeDef = TypedDict(
     "KinesisStreamsInputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-JSONMappingParametersOutputTypeDef = TypedDict(
-    "JSONMappingParametersOutputTypeDef",
-    {
-        "RecordRowPath": str,
-    },
-)
-
 JSONMappingParametersTypeDef = TypedDict(
     "JSONMappingParametersTypeDef",
     {
         "RecordRowPath": str,
     },
 )
 
@@ -1334,36 +1189,24 @@
 LambdaOutputUpdateTypeDef = TypedDict(
     "LambdaOutputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-    },
-)
-_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
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
-class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
-    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationSnapshotsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
@@ -1402,22 +1245,14 @@
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1426,65 +1261,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
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
-_RequiredRecordColumnOutputTypeDef = TypedDict(
-    "_RequiredRecordColumnOutputTypeDef",
-    {
-        "Name": str,
-        "SqlType": str,
-    },
-)
-_OptionalRecordColumnOutputTypeDef = TypedDict(
-    "_OptionalRecordColumnOutputTypeDef",
-    {
-        "Mapping": str,
-    },
-    total=False,
-)
-
-
-class RecordColumnOutputTypeDef(
-    _RequiredRecordColumnOutputTypeDef, _OptionalRecordColumnOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredS3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -1518,25 +1302,14 @@
     {
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
     },
     total=False,
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
 RollbackApplicationRequestRequestTypeDef = TypedDict(
     "RollbackApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
     },
 )
@@ -1618,25 +1391,69 @@
 
 AddApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
+    "CreateApplicationPresignedUrlResponseTypeDef",
+    {
+        "AuthorizedUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationOutputResponseTypeDef = TypedDict(
+    "DeleteApplicationOutputResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredAddApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1662,26 +1479,26 @@
 
 AddApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "AddApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationResponseTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationMaintenanceConfigurationDescription": (
             ApplicationMaintenanceConfigurationDescriptionTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1692,24 +1509,24 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "ApplicationVersionSummaries": List[ApplicationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CatalogConfigurationDescriptionTypeDef = TypedDict(
     "CatalogConfigurationDescriptionTypeDef",
     {
         "GlueDataCatalogConfigurationDescription": GlueDataCatalogConfigurationDescriptionTypeDef,
@@ -1757,28 +1574,36 @@
         "TextContentUpdate": str,
         "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CustomArtifactConfigurationDescriptionTypeDef = TypedDict(
     "CustomArtifactConfigurationDescriptionTypeDef",
     {
         "ArtifactType": ArtifactTypeType,
-        "S3ContentLocationDescription": S3ContentLocationOutputTypeDef,
-        "MavenReferenceDescription": MavenReferenceOutputTypeDef,
+        "S3ContentLocationDescription": S3ContentLocationTypeDef,
+        "MavenReferenceDescription": MavenReferenceTypeDef,
     },
     total=False,
 )
 
 _RequiredCustomArtifactConfigurationTypeDef = TypedDict(
     "_RequiredCustomArtifactConfigurationTypeDef",
     {
@@ -1823,24 +1648,24 @@
     total=False,
 )
 
 DescribeApplicationSnapshotResponseTypeDef = TypedDict(
     "DescribeApplicationSnapshotResponseTypeDef",
     {
         "SnapshotDetails": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationSnapshotsResponseTypeDef = TypedDict(
     "ListApplicationSnapshotsResponseTypeDef",
     {
         "SnapshotSummaries": List[SnapshotDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlRunConfigurationTypeDef = TypedDict(
     "SqlRunConfigurationTypeDef",
     {
         "InputId": str,
@@ -1900,16 +1725,16 @@
     },
     total=False,
 )
 
 RunConfigurationDescriptionTypeDef = TypedDict(
     "RunConfigurationDescriptionTypeDef",
     {
-        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationOutputTypeDef,
-        "FlinkRunConfigurationDescription": FlinkRunConfigurationOutputTypeDef,
+        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationTypeDef,
+        "FlinkRunConfigurationDescription": FlinkRunConfigurationTypeDef,
     },
     total=False,
 )
 
 RunConfigurationUpdateTypeDef = TypedDict(
     "RunConfigurationUpdateTypeDef",
     {
@@ -1937,23 +1762,14 @@
 InputProcessingConfigurationUpdateTypeDef = TypedDict(
     "InputProcessingConfigurationUpdateTypeDef",
     {
         "InputLambdaProcessorUpdate": InputLambdaProcessorUpdateTypeDef,
     },
 )
 
-MappingParametersOutputTypeDef = TypedDict(
-    "MappingParametersOutputTypeDef",
-    {
-        "JSONMappingParameters": JSONMappingParametersOutputTypeDef,
-        "CSVMappingParameters": CSVMappingParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 MappingParametersTypeDef = TypedDict(
     "MappingParametersTypeDef",
     {
         "JSONMappingParameters": JSONMappingParametersTypeDef,
         "CSVMappingParameters": CSVMappingParametersTypeDef,
     },
     total=False,
@@ -1963,15 +1779,15 @@
     "OutputDescriptionTypeDef",
     {
         "OutputId": str,
         "Name": str,
         "KinesisStreamsOutputDescription": KinesisStreamsOutputDescriptionTypeDef,
         "KinesisFirehoseOutputDescription": KinesisFirehoseOutputDescriptionTypeDef,
         "LambdaOutputDescription": LambdaOutputDescriptionTypeDef,
-        "DestinationSchema": DestinationSchemaOutputTypeDef,
+        "DestinationSchema": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
@@ -2013,20 +1829,42 @@
 )
 
 
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+    },
+)
+_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
+    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
@@ -2140,15 +1978,15 @@
 AddApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputId": str,
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationInputProcessingConfigurationRequestRequestTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -2179,35 +2017,14 @@
 class DiscoverInputSchemaRequestRequestTypeDef(
     _RequiredDiscoverInputSchemaRequestRequestTypeDef,
     _OptionalDiscoverInputSchemaRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredRecordFormatOutputTypeDef = TypedDict(
-    "_RequiredRecordFormatOutputTypeDef",
-    {
-        "RecordFormatType": RecordFormatTypeType,
-    },
-)
-_OptionalRecordFormatOutputTypeDef = TypedDict(
-    "_OptionalRecordFormatOutputTypeDef",
-    {
-        "MappingParameters": MappingParametersOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RecordFormatOutputTypeDef(
-    _RequiredRecordFormatOutputTypeDef, _OptionalRecordFormatOutputTypeDef
-):
-    pass
-
-
 _RequiredRecordFormatTypeDef = TypedDict(
     "_RequiredRecordFormatTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 _OptionalRecordFormatTypeDef = TypedDict(
@@ -2225,15 +2042,15 @@
 
 AddApplicationOutputResponseTypeDef = TypedDict(
     "AddApplicationOutputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -2259,19 +2076,29 @@
 
 class StartApplicationRequestRequestTypeDef(
     _RequiredStartApplicationRequestRequestTypeDef, _OptionalStartApplicationRequestRequestTypeDef
 ):
     pass
 
 
+InputSchemaUpdateTypeDef = TypedDict(
+    "InputSchemaUpdateTypeDef",
+    {
+        "RecordFormatUpdate": RecordFormatTypeDef,
+        "RecordEncodingUpdate": str,
+        "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
+    },
+    total=False,
+)
+
 _RequiredSourceSchemaOutputTypeDef = TypedDict(
     "_RequiredSourceSchemaOutputTypeDef",
     {
-        "RecordFormat": RecordFormatOutputTypeDef,
-        "RecordColumns": List[RecordColumnOutputTypeDef],
+        "RecordFormat": RecordFormatTypeDef,
+        "RecordColumns": List[RecordColumnTypeDef],
     },
 )
 _OptionalSourceSchemaOutputTypeDef = TypedDict(
     "_OptionalSourceSchemaOutputTypeDef",
     {
         "RecordEncoding": str,
     },
@@ -2281,24 +2108,14 @@
 
 class SourceSchemaOutputTypeDef(
     _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
 ):
     pass
 
 
-InputSchemaUpdateTypeDef = TypedDict(
-    "InputSchemaUpdateTypeDef",
-    {
-        "RecordFormatUpdate": RecordFormatTypeDef,
-        "RecordEncodingUpdate": str,
-        "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
-    },
-    total=False,
-)
-
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -2311,37 +2128,61 @@
 )
 
 
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
 
+_RequiredInputUpdateTypeDef = TypedDict(
+    "_RequiredInputUpdateTypeDef",
+    {
+        "InputId": str,
+    },
+)
+_OptionalInputUpdateTypeDef = TypedDict(
+    "_OptionalInputUpdateTypeDef",
+    {
+        "NamePrefixUpdate": str,
+        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
+        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
+        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
+        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
+        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
+    },
+    total=False,
+)
+
+
+class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
+    pass
+
+
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
         "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDescriptionTypeDef = TypedDict(
     "InputDescriptionTypeDef",
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
         "InputSchema": SourceSchemaOutputTypeDef,
-        "InputParallelism": InputParallelismOutputTypeDef,
-        "InputStartingPositionConfiguration": InputStartingPositionConfigurationOutputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
+        "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
@@ -2361,38 +2202,14 @@
 
 class ReferenceDataSourceDescriptionTypeDef(
     _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
 ):
     pass
 
 
-_RequiredInputUpdateTypeDef = TypedDict(
-    "_RequiredInputUpdateTypeDef",
-    {
-        "InputId": str,
-    },
-)
-_OptionalInputUpdateTypeDef = TypedDict(
-    "_OptionalInputUpdateTypeDef",
-    {
-        "NamePrefixUpdate": str,
-        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
-        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
-        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
-        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
-        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
-    },
-    total=False,
-)
-
-
-class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
-    pass
-
-
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -2459,25 +2276,25 @@
 
 AddApplicationInputResponseTypeDef = TypedDict(
     "AddApplicationInputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlApplicationConfigurationDescriptionTypeDef = TypedDict(
     "SqlApplicationConfigurationDescriptionTypeDef",
     {
         "InputDescriptions": List[InputDescriptionTypeDef],
@@ -2663,42 +2480,42 @@
     pass
 
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationVersionResponseTypeDef = TypedDict(
     "DescribeApplicationVersionResponseTypeDef",
     {
         "ApplicationVersionDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackApplicationResponseTypeDef = TypedDict(
     "RollbackApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,136 +37,124 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationTypeDef",
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
-    "ApplicationRestoreConfigurationOutputTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
-    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "S3ApplicationCodeLocationDescriptionTypeDef",
     "S3ContentLocationTypeDef",
     "S3ContentLocationUpdateTypeDef",
     "CreateApplicationPresignedUrlRequestRequestTypeDef",
-    "CreateApplicationPresignedUrlResponseTypeDef",
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
-    "MavenReferenceOutputTypeDef",
-    "S3ContentLocationOutputTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
-    "DeleteApplicationOutputResponseTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteApplicationSnapshotRequestRequestTypeDef",
     "DeleteApplicationVpcConfigurationRequestRequestTypeDef",
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
-    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
     "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
-    "FlinkRunConfigurationOutputTypeDef",
     "FlinkRunConfigurationTypeDef",
-    "InputParallelismOutputTypeDef",
-    "InputStartingPositionConfigurationOutputTypeDef",
+    "InputParallelismTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
     "InputLambdaProcessorDescriptionTypeDef",
     "InputLambdaProcessorTypeDef",
     "InputLambdaProcessorUpdateTypeDef",
-    "InputParallelismTypeDef",
     "InputParallelismUpdateTypeDef",
     "RecordColumnTypeDef",
     "KinesisFirehoseInputTypeDef",
     "KinesisStreamsInputTypeDef",
     "KinesisFirehoseInputUpdateTypeDef",
     "KinesisStreamsInputUpdateTypeDef",
-    "JSONMappingParametersOutputTypeDef",
     "JSONMappingParametersTypeDef",
     "KinesisFirehoseOutputDescriptionTypeDef",
     "KinesisFirehoseOutputTypeDef",
     "KinesisFirehoseOutputUpdateTypeDef",
     "KinesisStreamsOutputDescriptionTypeDef",
     "KinesisStreamsOutputTypeDef",
     "KinesisStreamsOutputUpdateTypeDef",
     "LambdaOutputDescriptionTypeDef",
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
-    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationSnapshotsRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ZeppelinMonitoringConfigurationDescriptionTypeDef",
     "ZeppelinMonitoringConfigurationTypeDef",
     "ZeppelinMonitoringConfigurationUpdateTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "CreateApplicationPresignedUrlResponseTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    "DeleteApplicationOutputResponseTypeDef",
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "AddApplicationVpcConfigurationRequestRequestTypeDef",
     "AddApplicationVpcConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "CatalogConfigurationDescriptionTypeDef",
     "CatalogConfigurationTypeDef",
     "CatalogConfigurationUpdateTypeDef",
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
@@ -179,42 +167,41 @@
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
-    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ApplicationCodeConfigurationDescriptionTypeDef",
     "ApplicationCodeConfigurationTypeDef",
     "ApplicationCodeConfigurationUpdateTypeDef",
     "ZeppelinApplicationConfigurationDescriptionTypeDef",
     "ZeppelinApplicationConfigurationTypeDef",
     "ZeppelinApplicationConfigurationUpdateTypeDef",
     "RunConfigurationTypeDef",
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
-    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "SourceSchemaOutputTypeDef",
     "InputSchemaUpdateTypeDef",
+    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
+    "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
-    "InputUpdateTypeDef",
     "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
@@ -258,14 +245,25 @@
 
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
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
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -332,34 +330,14 @@
 ApplicationMaintenanceConfigurationUpdateTypeDef = TypedDict(
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     {
         "ApplicationMaintenanceWindowStartTimeUpdate": str,
     },
 )
 
-_RequiredApplicationRestoreConfigurationOutputTypeDef = TypedDict(
-    "_RequiredApplicationRestoreConfigurationOutputTypeDef",
-    {
-        "ApplicationRestoreType": ApplicationRestoreTypeType,
-    },
-)
-_OptionalApplicationRestoreConfigurationOutputTypeDef = TypedDict(
-    "_OptionalApplicationRestoreConfigurationOutputTypeDef",
-    {
-        "SnapshotName": str,
-    },
-    total=False,
-)
-
-class ApplicationRestoreConfigurationOutputTypeDef(
-    _RequiredApplicationRestoreConfigurationOutputTypeDef,
-    _OptionalApplicationRestoreConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredApplicationRestoreConfigurationTypeDef = TypedDict(
     "_RequiredApplicationRestoreConfigurationTypeDef",
     {
         "ApplicationRestoreType": ApplicationRestoreTypeType,
     },
 )
 _OptionalApplicationRestoreConfigurationTypeDef = TypedDict(
@@ -402,22 +380,14 @@
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
-CSVMappingParametersOutputTypeDef = TypedDict(
-    "CSVMappingParametersOutputTypeDef",
-    {
-        "RecordRowDelimiter": str,
-        "RecordColumnDelimiter": str,
-    },
-)
-
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -573,22 +543,14 @@
 
 class CreateApplicationPresignedUrlRequestRequestTypeDef(
     _RequiredCreateApplicationPresignedUrlRequestRequestTypeDef,
     _OptionalCreateApplicationPresignedUrlRequestRequestTypeDef,
 ):
     pass
 
-CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
-    "CreateApplicationPresignedUrlResponseTypeDef",
-    {
-        "AuthorizedUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -606,43 +568,14 @@
     "CreateApplicationSnapshotRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "SnapshotName": str,
     },
 )
 
-MavenReferenceOutputTypeDef = TypedDict(
-    "MavenReferenceOutputTypeDef",
-    {
-        "GroupId": str,
-        "ArtifactId": str,
-        "Version": str,
-    },
-)
-
-_RequiredS3ContentLocationOutputTypeDef = TypedDict(
-    "_RequiredS3ContentLocationOutputTypeDef",
-    {
-        "BucketARN": str,
-        "FileKey": str,
-    },
-)
-_OptionalS3ContentLocationOutputTypeDef = TypedDict(
-    "_OptionalS3ContentLocationOutputTypeDef",
-    {
-        "ObjectVersion": str,
-    },
-    total=False,
-)
-
-class S3ContentLocationOutputTypeDef(
-    _RequiredS3ContentLocationOutputTypeDef, _OptionalS3ContentLocationOutputTypeDef
-):
-    pass
-
 MavenReferenceTypeDef = TypedDict(
     "MavenReferenceTypeDef",
     {
         "GroupId": str,
         "ArtifactId": str,
         "Version": str,
     },
@@ -675,59 +608,32 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "InputId": str,
     },
 )
 
-DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationOutputRequestRequestTypeDef = TypedDict(
     "DeleteApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "OutputId": str,
     },
 )
 
-DeleteApplicationOutputResponseTypeDef = TypedDict(
-    "DeleteApplicationOutputResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CreateTimestamp": Union[datetime, str],
     },
 )
@@ -759,23 +665,14 @@
 
 class DeleteApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalDeleteApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ContentBaseLocationDescriptionTypeDef = TypedDict(
     "_RequiredS3ContentBaseLocationDescriptionTypeDef",
     {
         "BucketARN": str,
     },
 )
 _OptionalS3ContentBaseLocationDescriptionTypeDef = TypedDict(
@@ -871,21 +768,14 @@
     "DescribeApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "ApplicationVersionId": int,
     },
 )
 
-DestinationSchemaOutputTypeDef = TypedDict(
-    "DestinationSchemaOutputTypeDef",
-    {
-        "RecordFormatType": RecordFormatTypeType,
-    },
-)
-
 DestinationSchemaTypeDef = TypedDict(
     "DestinationSchemaTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 
@@ -1001,46 +891,30 @@
         "ParallelismUpdate": int,
         "ParallelismPerKPUUpdate": int,
         "AutoScalingEnabledUpdate": bool,
     },
     total=False,
 )
 
-FlinkRunConfigurationOutputTypeDef = TypedDict(
-    "FlinkRunConfigurationOutputTypeDef",
-    {
-        "AllowNonRestoredState": bool,
-    },
-    total=False,
-)
-
 FlinkRunConfigurationTypeDef = TypedDict(
     "FlinkRunConfigurationTypeDef",
     {
         "AllowNonRestoredState": bool,
     },
     total=False,
 )
 
-InputParallelismOutputTypeDef = TypedDict(
-    "InputParallelismOutputTypeDef",
+InputParallelismTypeDef = TypedDict(
+    "InputParallelismTypeDef",
     {
         "Count": int,
     },
     total=False,
 )
 
-InputStartingPositionConfigurationOutputTypeDef = TypedDict(
-    "InputStartingPositionConfigurationOutputTypeDef",
-    {
-        "InputStartingPosition": InputStartingPositionType,
-    },
-    total=False,
-)
-
 _RequiredKinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "_RequiredKinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalKinesisFirehoseInputDescriptionTypeDef = TypedDict(
@@ -1104,22 +978,14 @@
 InputLambdaProcessorUpdateTypeDef = TypedDict(
     "InputLambdaProcessorUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-InputParallelismTypeDef = TypedDict(
-    "InputParallelismTypeDef",
-    {
-        "Count": int,
-    },
-    total=False,
-)
-
 InputParallelismUpdateTypeDef = TypedDict(
     "InputParallelismUpdateTypeDef",
     {
         "CountUpdate": int,
     },
 )
 
@@ -1165,21 +1031,14 @@
 KinesisStreamsInputUpdateTypeDef = TypedDict(
     "KinesisStreamsInputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-JSONMappingParametersOutputTypeDef = TypedDict(
-    "JSONMappingParametersOutputTypeDef",
-    {
-        "RecordRowPath": str,
-    },
-)
-
 JSONMappingParametersTypeDef = TypedDict(
     "JSONMappingParametersTypeDef",
     {
         "RecordRowPath": str,
     },
 )
 
@@ -1279,34 +1138,24 @@
 LambdaOutputUpdateTypeDef = TypedDict(
     "LambdaOutputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-    },
-)
-_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
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
 
-class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
-    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationSnapshotsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
@@ -1341,22 +1190,14 @@
 
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1365,61 +1206,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
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
-_RequiredRecordColumnOutputTypeDef = TypedDict(
-    "_RequiredRecordColumnOutputTypeDef",
-    {
-        "Name": str,
-        "SqlType": str,
-    },
-)
-_OptionalRecordColumnOutputTypeDef = TypedDict(
-    "_OptionalRecordColumnOutputTypeDef",
-    {
-        "Mapping": str,
-    },
-    total=False,
-)
-
-class RecordColumnOutputTypeDef(
-    _RequiredRecordColumnOutputTypeDef, _OptionalRecordColumnOutputTypeDef
-):
-    pass
-
 _RequiredS3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredS3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -1451,25 +1245,14 @@
     {
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
     },
     total=False,
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
 RollbackApplicationRequestRequestTypeDef = TypedDict(
     "RollbackApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
     },
 )
@@ -1547,25 +1330,69 @@
 
 AddApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
+    "CreateApplicationPresignedUrlResponseTypeDef",
+    {
+        "AuthorizedUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationOutputResponseTypeDef = TypedDict(
+    "DeleteApplicationOutputResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredAddApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1589,26 +1416,26 @@
 
 AddApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "AddApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationResponseTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationMaintenanceConfigurationDescription": (
             ApplicationMaintenanceConfigurationDescriptionTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1619,24 +1446,24 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "ApplicationVersionSummaries": List[ApplicationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CatalogConfigurationDescriptionTypeDef = TypedDict(
     "CatalogConfigurationDescriptionTypeDef",
     {
         "GlueDataCatalogConfigurationDescription": GlueDataCatalogConfigurationDescriptionTypeDef,
@@ -1684,28 +1511,36 @@
         "TextContentUpdate": str,
         "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CustomArtifactConfigurationDescriptionTypeDef = TypedDict(
     "CustomArtifactConfigurationDescriptionTypeDef",
     {
         "ArtifactType": ArtifactTypeType,
-        "S3ContentLocationDescription": S3ContentLocationOutputTypeDef,
-        "MavenReferenceDescription": MavenReferenceOutputTypeDef,
+        "S3ContentLocationDescription": S3ContentLocationTypeDef,
+        "MavenReferenceDescription": MavenReferenceTypeDef,
     },
     total=False,
 )
 
 _RequiredCustomArtifactConfigurationTypeDef = TypedDict(
     "_RequiredCustomArtifactConfigurationTypeDef",
     {
@@ -1748,24 +1583,24 @@
     total=False,
 )
 
 DescribeApplicationSnapshotResponseTypeDef = TypedDict(
     "DescribeApplicationSnapshotResponseTypeDef",
     {
         "SnapshotDetails": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationSnapshotsResponseTypeDef = TypedDict(
     "ListApplicationSnapshotsResponseTypeDef",
     {
         "SnapshotSummaries": List[SnapshotDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlRunConfigurationTypeDef = TypedDict(
     "SqlRunConfigurationTypeDef",
     {
         "InputId": str,
@@ -1825,16 +1660,16 @@
     },
     total=False,
 )
 
 RunConfigurationDescriptionTypeDef = TypedDict(
     "RunConfigurationDescriptionTypeDef",
     {
-        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationOutputTypeDef,
-        "FlinkRunConfigurationDescription": FlinkRunConfigurationOutputTypeDef,
+        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationTypeDef,
+        "FlinkRunConfigurationDescription": FlinkRunConfigurationTypeDef,
     },
     total=False,
 )
 
 RunConfigurationUpdateTypeDef = TypedDict(
     "RunConfigurationUpdateTypeDef",
     {
@@ -1862,23 +1697,14 @@
 InputProcessingConfigurationUpdateTypeDef = TypedDict(
     "InputProcessingConfigurationUpdateTypeDef",
     {
         "InputLambdaProcessorUpdate": InputLambdaProcessorUpdateTypeDef,
     },
 )
 
-MappingParametersOutputTypeDef = TypedDict(
-    "MappingParametersOutputTypeDef",
-    {
-        "JSONMappingParameters": JSONMappingParametersOutputTypeDef,
-        "CSVMappingParameters": CSVMappingParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 MappingParametersTypeDef = TypedDict(
     "MappingParametersTypeDef",
     {
         "JSONMappingParameters": JSONMappingParametersTypeDef,
         "CSVMappingParameters": CSVMappingParametersTypeDef,
     },
     total=False,
@@ -1888,15 +1714,15 @@
     "OutputDescriptionTypeDef",
     {
         "OutputId": str,
         "Name": str,
         "KinesisStreamsOutputDescription": KinesisStreamsOutputDescriptionTypeDef,
         "KinesisFirehoseOutputDescription": KinesisFirehoseOutputDescriptionTypeDef,
         "LambdaOutputDescription": LambdaOutputDescriptionTypeDef,
-        "DestinationSchema": DestinationSchemaOutputTypeDef,
+        "DestinationSchema": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
@@ -1934,21 +1760,41 @@
     },
     total=False,
 )
 
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationName": str,
     },
 )
+_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
+    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
@@ -2055,15 +1901,15 @@
 AddApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputId": str,
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationInputProcessingConfigurationRequestRequestTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -2092,33 +1938,14 @@
 
 class DiscoverInputSchemaRequestRequestTypeDef(
     _RequiredDiscoverInputSchemaRequestRequestTypeDef,
     _OptionalDiscoverInputSchemaRequestRequestTypeDef,
 ):
     pass
 
-_RequiredRecordFormatOutputTypeDef = TypedDict(
-    "_RequiredRecordFormatOutputTypeDef",
-    {
-        "RecordFormatType": RecordFormatTypeType,
-    },
-)
-_OptionalRecordFormatOutputTypeDef = TypedDict(
-    "_OptionalRecordFormatOutputTypeDef",
-    {
-        "MappingParameters": MappingParametersOutputTypeDef,
-    },
-    total=False,
-)
-
-class RecordFormatOutputTypeDef(
-    _RequiredRecordFormatOutputTypeDef, _OptionalRecordFormatOutputTypeDef
-):
-    pass
-
 _RequiredRecordFormatTypeDef = TypedDict(
     "_RequiredRecordFormatTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 _OptionalRecordFormatTypeDef = TypedDict(
@@ -2134,15 +1961,15 @@
 
 AddApplicationOutputResponseTypeDef = TypedDict(
     "AddApplicationOutputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -2166,19 +1993,29 @@
 )
 
 class StartApplicationRequestRequestTypeDef(
     _RequiredStartApplicationRequestRequestTypeDef, _OptionalStartApplicationRequestRequestTypeDef
 ):
     pass
 
+InputSchemaUpdateTypeDef = TypedDict(
+    "InputSchemaUpdateTypeDef",
+    {
+        "RecordFormatUpdate": RecordFormatTypeDef,
+        "RecordEncodingUpdate": str,
+        "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
+    },
+    total=False,
+)
+
 _RequiredSourceSchemaOutputTypeDef = TypedDict(
     "_RequiredSourceSchemaOutputTypeDef",
     {
-        "RecordFormat": RecordFormatOutputTypeDef,
-        "RecordColumns": List[RecordColumnOutputTypeDef],
+        "RecordFormat": RecordFormatTypeDef,
+        "RecordColumns": List[RecordColumnTypeDef],
     },
 )
 _OptionalSourceSchemaOutputTypeDef = TypedDict(
     "_OptionalSourceSchemaOutputTypeDef",
     {
         "RecordEncoding": str,
     },
@@ -2186,24 +2023,14 @@
 )
 
 class SourceSchemaOutputTypeDef(
     _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
 ):
     pass
 
-InputSchemaUpdateTypeDef = TypedDict(
-    "InputSchemaUpdateTypeDef",
-    {
-        "RecordFormatUpdate": RecordFormatTypeDef,
-        "RecordEncodingUpdate": str,
-        "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
-    },
-    total=False,
-)
-
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -2214,37 +2041,59 @@
     },
     total=False,
 )
 
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
+_RequiredInputUpdateTypeDef = TypedDict(
+    "_RequiredInputUpdateTypeDef",
+    {
+        "InputId": str,
+    },
+)
+_OptionalInputUpdateTypeDef = TypedDict(
+    "_OptionalInputUpdateTypeDef",
+    {
+        "NamePrefixUpdate": str,
+        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
+        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
+        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
+        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
+        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
+    },
+    total=False,
+)
+
+class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
+    pass
+
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
         "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDescriptionTypeDef = TypedDict(
     "InputDescriptionTypeDef",
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
         "InputSchema": SourceSchemaOutputTypeDef,
-        "InputParallelism": InputParallelismOutputTypeDef,
-        "InputStartingPositionConfiguration": InputStartingPositionConfigurationOutputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
+        "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
@@ -2262,36 +2111,14 @@
 )
 
 class ReferenceDataSourceDescriptionTypeDef(
     _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
 ):
     pass
 
-_RequiredInputUpdateTypeDef = TypedDict(
-    "_RequiredInputUpdateTypeDef",
-    {
-        "InputId": str,
-    },
-)
-_OptionalInputUpdateTypeDef = TypedDict(
-    "_OptionalInputUpdateTypeDef",
-    {
-        "NamePrefixUpdate": str,
-        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
-        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
-        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
-        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
-        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
-    },
-    total=False,
-)
-
-class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
-    pass
-
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -2352,25 +2179,25 @@
 
 AddApplicationInputResponseTypeDef = TypedDict(
     "AddApplicationInputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlApplicationConfigurationDescriptionTypeDef = TypedDict(
     "SqlApplicationConfigurationDescriptionTypeDef",
     {
         "InputDescriptions": List[InputDescriptionTypeDef],
@@ -2550,42 +2377,42 @@
 ):
     pass
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationVersionResponseTypeDef = TypedDict(
     "DescribeApplicationVersionResponseTypeDef",
     {
         "ApplicationVersionDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackApplicationResponseTypeDef = TypedDict(
     "RollbackApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,136 +342,124 @@
 `mypy_boto3_kinesisanalyticsv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
-    ApplicationRestoreConfigurationOutputTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
-    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
-    CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
-    MavenReferenceOutputTypeDef,
-    S3ContentLocationOutputTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteApplicationSnapshotRequestRequestTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
-    DeleteApplicationVpcConfigurationResponseTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
-    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
     PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
-    FlinkRunConfigurationOutputTypeDef,
     FlinkRunConfigurationTypeDef,
-    InputParallelismOutputTypeDef,
-    InputStartingPositionConfigurationOutputTypeDef,
+    InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
     InputLambdaProcessorDescriptionTypeDef,
     InputLambdaProcessorTypeDef,
     InputLambdaProcessorUpdateTypeDef,
-    InputParallelismTypeDef,
     InputParallelismUpdateTypeDef,
     RecordColumnTypeDef,
     KinesisFirehoseInputTypeDef,
     KinesisStreamsInputTypeDef,
     KinesisFirehoseInputUpdateTypeDef,
     KinesisStreamsInputUpdateTypeDef,
-    JSONMappingParametersOutputTypeDef,
     JSONMappingParametersTypeDef,
     KinesisFirehoseOutputDescriptionTypeDef,
     KinesisFirehoseOutputTypeDef,
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
-    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ZeppelinMonitoringConfigurationDescriptionTypeDef,
     ZeppelinMonitoringConfigurationTypeDef,
     ZeppelinMonitoringConfigurationUpdateTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
+    CreateApplicationPresignedUrlResponseTypeDef,
     DeleteApplicationCloudWatchLoggingOptionResponseTypeDef,
+    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
+    DeleteApplicationOutputResponseTypeDef,
+    DeleteApplicationReferenceDataSourceResponseTypeDef,
+    DeleteApplicationVpcConfigurationResponseTypeDef,
     AddApplicationVpcConfigurationRequestRequestTypeDef,
     AddApplicationVpcConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
     CatalogConfigurationTypeDef,
     CatalogConfigurationUpdateTypeDef,
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
@@ -484,42 +472,41 @@
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
     AddApplicationInputProcessingConfigurationResponseTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
-    SourceSchemaOutputTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
+    InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
-    InputUpdateTypeDef,
     InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
     AddApplicationInputRequestRequestTypeDef,
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.12/setup.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalyticsv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

