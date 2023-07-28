# Comparing `tmp/mypy-boto3-kinesisanalytics-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesisanalytics-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalytics-1.28.12.tar", last modified: Thu Jul 27 05:34:54 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalytics-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalytics-1.28.12.tar` & `mypy-boto3-kinesisanalytics-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.012466 mypy-boto3-kinesisanalytics-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-07-27 05:34:54.004466 mypy-boto3-kinesisanalytics-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.996466 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29122 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.004466 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:54.012466 mypy-boto3-kinesisanalytics-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.781344 mypy-boto3-kinesisanalytics-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-28 20:43:05.781344 mypy-boto3-kinesisanalytics-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.765343 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26473 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:17.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.781344 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.785344 mypy-boto3-kinesisanalytics-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:29:16.000000 mypy-boto3-kinesisanalytics-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/LICENSE` & `mypy-boto3-kinesisanalytics-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/PKG-INFO` & `mypy-boto3-kinesisanalytics-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalytics
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,89 +304,80 @@
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
-    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
-    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
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
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
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
     ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/README.md` & `mypy-boto3-kinesisanalytics-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,89 +272,80 @@
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
-    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
-    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
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
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
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
     ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__main__.py` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalytics 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KinesisAnalytics 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics\nOther"
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

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.py` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.pyi` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.py` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.pyi` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.py` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,95 +18,85 @@
 from .literals import ApplicationStatusType, InputStartingPositionType, RecordFormatTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
-    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
-    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
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
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
-    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
-    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
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
     "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
@@ -134,22 +124,20 @@
     "_OptionalCloudWatchLoggingOptionDescriptionTypeDef",
     {
         "CloudWatchLoggingOptionId": str,
     },
     total=False,
 )
 
-
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
-
 ApplicationSummaryTypeDef = TypedDict(
     "ApplicationSummaryTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
     },
@@ -166,29 +154,19 @@
     {
         "LogStreamARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
 )
 
-
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
-
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
@@ -203,18 +181,27 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
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
 
 DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOptionId": str,
@@ -259,21 +246,14 @@
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
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
 
@@ -290,30 +270,22 @@
     {
         "RoleARN": str,
         "BucketARN": str,
         "FileKey": str,
     },
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
 KinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "KinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
     total=False,
@@ -350,22 +322,14 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
     total=False,
 )
@@ -381,19 +345,17 @@
     "_OptionalRecordColumnTypeDef",
     {
         "Mapping": str,
     },
     total=False,
 )
 
-
 class RecordColumnTypeDef(_RequiredRecordColumnTypeDef, _OptionalRecordColumnTypeDef):
     pass
 
-
 KinesisFirehoseInputTypeDef = TypedDict(
     "KinesisFirehoseInputTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
 )
@@ -420,21 +382,14 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
 
@@ -528,55 +483,14 @@
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
 S3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "S3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
         "ReferenceRoleARN": str,
     },
@@ -597,25 +511,14 @@
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
         "ReferenceRoleARNUpdate": str,
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
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -632,36 +535,44 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOption": CloudWatchLoggingOptionTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationSummary": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "HasMoreApplications": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputConfigurationTypeDef = TypedDict(
     "InputConfigurationTypeDef",
     {
         "Id": str,
@@ -687,23 +598,14 @@
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
@@ -713,15 +615,15 @@
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
@@ -735,19 +637,17 @@
         "KinesisStreamsOutput": KinesisStreamsOutputTypeDef,
         "KinesisFirehoseOutput": KinesisFirehoseOutputTypeDef,
         "LambdaOutput": LambdaOutputTypeDef,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-
 _RequiredOutputUpdateTypeDef = TypedDict(
     "_RequiredOutputUpdateTypeDef",
     {
         "OutputId": str,
     },
 )
 _OptionalOutputUpdateTypeDef = TypedDict(
@@ -758,27 +658,17 @@
         "KinesisFirehoseOutputUpdate": KinesisFirehoseOutputUpdateTypeDef,
         "LambdaOutputUpdate": LambdaOutputUpdateTypeDef,
         "DestinationSchemaUpdate": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
-
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "InputConfigurations": Sequence[InputConfigurationTypeDef],
     },
 )
@@ -801,95 +691,70 @@
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
         "S3Configuration": S3ConfigurationTypeDef,
         "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
     },
     total=False,
 )
 
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
     "_OptionalRecordFormatTypeDef",
     {
         "MappingParameters": MappingParametersTypeDef,
     },
     total=False,
 )
 
-
 class RecordFormatTypeDef(_RequiredRecordFormatTypeDef, _OptionalRecordFormatTypeDef):
     pass
 
-
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Output": OutputTypeDef,
     },
 )
 
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
     total=False,
 )
 
-
 class SourceSchemaOutputTypeDef(
     _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
 ):
     pass
 
-
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
@@ -897,42 +762,62 @@
     "_OptionalSourceSchemaTypeDef",
     {
         "RecordEncoding": str,
     },
     total=False,
 )
 
-
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
@@ -945,45 +830,19 @@
     "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
         "ReferenceSchema": SourceSchemaOutputTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceDescriptionTypeDef(
     _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
 ):
     pass
 
-
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
@@ -994,19 +853,17 @@
         "KinesisStreamsInput": KinesisStreamsInputTypeDef,
         "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
-
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
-
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
 )
@@ -1014,21 +871,19 @@
     "_OptionalReferenceDataSourceTypeDef",
     {
         "S3ReferenceDataSource": S3ReferenceDataSourceTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceTypeDef(
     _RequiredReferenceDataSourceTypeDef, _OptionalReferenceDataSourceTypeDef
 ):
     pass
 
-
 _RequiredReferenceDataSourceUpdateTypeDef = TypedDict(
     "_RequiredReferenceDataSourceUpdateTypeDef",
     {
         "ReferenceId": str,
     },
 )
 _OptionalReferenceDataSourceUpdateTypeDef = TypedDict(
@@ -1037,21 +892,19 @@
         "TableNameUpdate": str,
         "S3ReferenceDataSourceUpdate": S3ReferenceDataSourceUpdateTypeDef,
         "ReferenceSchemaUpdate": SourceSchemaTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
-
 _RequiredApplicationDetailTypeDef = TypedDict(
     "_RequiredApplicationDetailTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
         "ApplicationVersionId": int,
@@ -1068,21 +921,19 @@
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
         "ApplicationCode": str,
     },
     total=False,
 )
 
-
 class ApplicationDetailTypeDef(
     _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
 ):
     pass
 
-
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -1103,21 +954,19 @@
         "CloudWatchLoggingOptions": Sequence[CloudWatchLoggingOptionTypeDef],
         "ApplicationCode": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -1135,15 +984,15 @@
     total=False,
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.pyi` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,94 +18,86 @@
 from .literals import ApplicationStatusType, InputStartingPositionType, RecordFormatTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
-    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
-    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
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
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
-    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
-    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
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
     "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
@@ -133,20 +125,22 @@
     "_OptionalCloudWatchLoggingOptionDescriptionTypeDef",
     {
         "CloudWatchLoggingOptionId": str,
     },
     total=False,
 )
 
+
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
+
 ApplicationSummaryTypeDef = TypedDict(
     "ApplicationSummaryTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
     },
@@ -163,26 +157,20 @@
     {
         "LogStreamARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
 )
 
+
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
-CSVMappingParametersOutputTypeDef = TypedDict(
-    "CSVMappingParametersOutputTypeDef",
-    {
-        "RecordRowDelimiter": str,
-        "RecordColumnDelimiter": str,
-    },
-)
 
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
@@ -198,17 +186,30 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
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
 DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOptionId": str,
     },
@@ -252,21 +253,14 @@
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
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
 
@@ -283,30 +277,22 @@
     {
         "RoleARN": str,
         "BucketARN": str,
         "FileKey": str,
     },
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
 KinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "KinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
     total=False,
@@ -343,22 +329,14 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
     total=False,
 )
@@ -374,17 +352,19 @@
     "_OptionalRecordColumnTypeDef",
     {
         "Mapping": str,
     },
     total=False,
 )
 
+
 class RecordColumnTypeDef(_RequiredRecordColumnTypeDef, _OptionalRecordColumnTypeDef):
     pass
 
+
 KinesisFirehoseInputTypeDef = TypedDict(
     "KinesisFirehoseInputTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
 )
@@ -411,21 +391,14 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
 
@@ -519,51 +492,14 @@
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
 S3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "S3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
         "ReferenceRoleARN": str,
     },
@@ -584,25 +520,14 @@
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
         "ReferenceRoleARNUpdate": str,
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
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -619,36 +544,44 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOption": CloudWatchLoggingOptionTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationSummary": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "HasMoreApplications": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputConfigurationTypeDef = TypedDict(
     "InputConfigurationTypeDef",
     {
         "Id": str,
@@ -674,23 +607,14 @@
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
@@ -700,15 +624,15 @@
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
@@ -722,17 +646,19 @@
         "KinesisStreamsOutput": KinesisStreamsOutputTypeDef,
         "KinesisFirehoseOutput": KinesisFirehoseOutputTypeDef,
         "LambdaOutput": LambdaOutputTypeDef,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+
 _RequiredOutputUpdateTypeDef = TypedDict(
     "_RequiredOutputUpdateTypeDef",
     {
         "OutputId": str,
     },
 )
 _OptionalOutputUpdateTypeDef = TypedDict(
@@ -743,24 +669,18 @@
         "KinesisFirehoseOutputUpdate": KinesisFirehoseOutputUpdateTypeDef,
         "LambdaOutputUpdate": LambdaOutputUpdateTypeDef,
         "DestinationSchemaUpdate": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
+
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "InputConfigurations": Sequence[InputConfigurationTypeDef],
     },
@@ -784,88 +704,73 @@
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
         "S3Configuration": S3ConfigurationTypeDef,
         "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
     },
     total=False,
 )
 
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
     "_OptionalRecordFormatTypeDef",
     {
         "MappingParameters": MappingParametersTypeDef,
     },
     total=False,
 )
 
+
 class RecordFormatTypeDef(_RequiredRecordFormatTypeDef, _OptionalRecordFormatTypeDef):
     pass
 
+
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Output": OutputTypeDef,
     },
 )
 
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
     total=False,
 )
 
+
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
 
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
@@ -874,40 +779,66 @@
     "_OptionalSourceSchemaTypeDef",
     {
         "RecordEncoding": str,
     },
     total=False,
 )
 
+
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
+
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
@@ -920,40 +851,20 @@
     "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
         "ReferenceSchema": SourceSchemaOutputTypeDef,
     },
     total=False,
 )
 
+
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
 
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
@@ -965,17 +876,19 @@
         "KinesisStreamsInput": KinesisStreamsInputTypeDef,
         "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
+
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
+
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
 )
@@ -983,19 +896,21 @@
     "_OptionalReferenceDataSourceTypeDef",
     {
         "S3ReferenceDataSource": S3ReferenceDataSourceTypeDef,
     },
     total=False,
 )
 
+
 class ReferenceDataSourceTypeDef(
     _RequiredReferenceDataSourceTypeDef, _OptionalReferenceDataSourceTypeDef
 ):
     pass
 
+
 _RequiredReferenceDataSourceUpdateTypeDef = TypedDict(
     "_RequiredReferenceDataSourceUpdateTypeDef",
     {
         "ReferenceId": str,
     },
 )
 _OptionalReferenceDataSourceUpdateTypeDef = TypedDict(
@@ -1004,19 +919,21 @@
         "TableNameUpdate": str,
         "S3ReferenceDataSourceUpdate": S3ReferenceDataSourceUpdateTypeDef,
         "ReferenceSchemaUpdate": SourceSchemaTypeDef,
     },
     total=False,
 )
 
+
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
+
 _RequiredApplicationDetailTypeDef = TypedDict(
     "_RequiredApplicationDetailTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
         "ApplicationVersionId": int,
@@ -1033,19 +950,21 @@
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
         "ApplicationCode": str,
     },
     total=False,
 )
 
+
 class ApplicationDetailTypeDef(
     _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
 ):
     pass
 
+
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -1066,19 +985,21 @@
         "CloudWatchLoggingOptions": Sequence[CloudWatchLoggingOptionTypeDef],
         "ApplicationCode": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -1096,15 +1017,15 @@
     total=False,
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalytics
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,89 +304,80 @@
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
-    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
-    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
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
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
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
     ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalytics-1.28.15/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.12/setup.py` & `mypy-boto3-kinesisanalytics-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalytics",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisAnalytics 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.KinesisAnalytics 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

