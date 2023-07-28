# Comparing `tmp/mypy-boto3-iotanalytics-1.28.12.tar.gz` & `tmp/mypy-boto3-iotanalytics-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotanalytics-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iotanalytics-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iotanalytics-1.28.12.tar` & `mypy-boto3-iotanalytics-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.096484 mypy-boto3-iotanalytics-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-27 05:34:49.092484 mypy-boto3-iotanalytics-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.088484 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64203 2023-07-27 05:23:59.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64094 2023-07-27 05:23:59.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.092484 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.096484 mypy-boto3-iotanalytics-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:57.000000 mypy-boto3-iotanalytics-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-07-28 20:28:19.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51447 2023-07-28 20:28:18.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:16.000000 mypy-boto3-iotanalytics-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/LICENSE` & `mypy-boto3-iotanalytics-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.15/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iotanalytics
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,182 +316,146 @@
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
+    ResponseMetadataTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
-    ChannelActivityOutputTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
-    CustomerManagedChannelS3StorageOutputTypeDef,
-    CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
-    RetentionPeriodOutputTypeDef,
-    ColumnOutputTypeDef,
+    CustomerManagedChannelS3StorageSummaryTypeDef,
+    RetentionPeriodTypeDef,
     ColumnTypeDef,
-    ResourceConfigurationOutputTypeDef,
     ResourceConfigurationTypeDef,
-    RetentionPeriodTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
-    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
-    CreatePipelineResponseTypeDef,
-    CustomerManagedDatastoreS3StorageOutputTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
-    IotEventsDestinationConfigurationOutputTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
-    DatasetContentVersionValueOutputTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
-    ScheduleOutputTypeDef,
-    TriggeringDatasetOutputTypeDef,
     ScheduleTypeDef,
     TriggeringDatasetTypeDef,
-    VersioningConfigurationOutputTypeDef,
-    DatastoreActivityOutputTypeDef,
     DatastoreActivityTypeDef,
-    IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
-    PartitionOutputTypeDef,
-    TimestampPartitionOutputTypeDef,
     PartitionTypeDef,
     TimestampPartitionTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteDatasetContentRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeletePipelineRequestRequestTypeDef,
-    DeltaTimeOutputTypeDef,
-    DeltaTimeSessionWindowConfigurationOutputTypeDef,
     DeltaTimeSessionWindowConfigurationTypeDef,
     DeltaTimeTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
-    LoggingOptionsOutputTypeDef,
+    LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
-    DeviceRegistryEnrichActivityOutputTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
-    DeviceShadowEnrichActivityOutputTypeDef,
     DeviceShadowEnrichActivityTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FilterActivityOutputTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
-    GlueConfigurationOutputTypeDef,
     GlueConfigurationTypeDef,
-    LambdaActivityOutputTypeDef,
     LambdaActivityTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    LoggingOptionsTypeDef,
-    MathActivityOutputTypeDef,
     MathActivityTypeDef,
-    OutputFileUriValueOutputTypeDef,
     OutputFileUriValueTypeDef,
-    PaginatorConfigTypeDef,
     RemoveAttributesActivityOutputTypeDef,
     SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RunPipelineActivityResponseTypeDef,
     SampleChannelDataRequestRequestTypeDef,
-    SampleChannelDataResponseTypeDef,
-    StartPipelineReprocessingResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
     BatchPutMessageRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    CreateDatasetContentResponseTypeDef,
+    CreatePipelineResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RunPipelineActivityResponseTypeDef,
+    SampleChannelDataResponseTypeDef,
+    StartPipelineReprocessingResponseTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageOutputTypeDef,
-    ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
+    ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
-    DatasetTriggerOutputTypeDef,
     DatasetTriggerTypeDef,
-    DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
-    DatastorePartitionOutputTypeDef,
     DatastorePartitionTypeDef,
-    QueryFilterOutputTypeDef,
-    LateDataRuleConfigurationOutputTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    S3DestinationConfigurationOutputTypeDef,
-    S3DestinationConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    VariableOutputTypeDef,
+    S3DestinationConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     VariableTypeDef,
     PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
     ChannelTypeDef,
-    ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ChannelSummaryTypeDef,
     ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
-    DatastoreStorageOutputTypeDef,
     DatastoreStorageSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
     DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
-    SqlQueryDatasetActionOutputTypeDef,
-    LateDataRuleOutputTypeDef,
     LateDataRuleTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
-    DatasetContentDeliveryDestinationOutputTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
     ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ListChannelsResponseTypeDef,
     FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
     DatastoreSummaryTypeDef,
-    DatasetContentDeliveryRuleOutputTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
     DatastoreTypeDef,
     CreateDatastoreRequestRequestTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/README.md` & `mypy-boto3-iotanalytics-1.28.15/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iotanalytics
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,182 +348,146 @@
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
+    ResponseMetadataTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
-    ChannelActivityOutputTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
-    CustomerManagedChannelS3StorageOutputTypeDef,
-    CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
-    RetentionPeriodOutputTypeDef,
-    ColumnOutputTypeDef,
+    CustomerManagedChannelS3StorageSummaryTypeDef,
+    RetentionPeriodTypeDef,
     ColumnTypeDef,
-    ResourceConfigurationOutputTypeDef,
     ResourceConfigurationTypeDef,
-    RetentionPeriodTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
-    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
-    CreatePipelineResponseTypeDef,
-    CustomerManagedDatastoreS3StorageOutputTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
-    IotEventsDestinationConfigurationOutputTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
-    DatasetContentVersionValueOutputTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
-    ScheduleOutputTypeDef,
-    TriggeringDatasetOutputTypeDef,
     ScheduleTypeDef,
     TriggeringDatasetTypeDef,
-    VersioningConfigurationOutputTypeDef,
-    DatastoreActivityOutputTypeDef,
     DatastoreActivityTypeDef,
-    IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
-    PartitionOutputTypeDef,
-    TimestampPartitionOutputTypeDef,
     PartitionTypeDef,
     TimestampPartitionTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteDatasetContentRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeletePipelineRequestRequestTypeDef,
-    DeltaTimeOutputTypeDef,
-    DeltaTimeSessionWindowConfigurationOutputTypeDef,
     DeltaTimeSessionWindowConfigurationTypeDef,
     DeltaTimeTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
-    LoggingOptionsOutputTypeDef,
+    LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
-    DeviceRegistryEnrichActivityOutputTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
-    DeviceShadowEnrichActivityOutputTypeDef,
     DeviceShadowEnrichActivityTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FilterActivityOutputTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
-    GlueConfigurationOutputTypeDef,
     GlueConfigurationTypeDef,
-    LambdaActivityOutputTypeDef,
     LambdaActivityTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    LoggingOptionsTypeDef,
-    MathActivityOutputTypeDef,
     MathActivityTypeDef,
-    OutputFileUriValueOutputTypeDef,
     OutputFileUriValueTypeDef,
-    PaginatorConfigTypeDef,
     RemoveAttributesActivityOutputTypeDef,
     SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RunPipelineActivityResponseTypeDef,
     SampleChannelDataRequestRequestTypeDef,
-    SampleChannelDataResponseTypeDef,
-    StartPipelineReprocessingResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
     BatchPutMessageRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    CreateDatasetContentResponseTypeDef,
+    CreatePipelineResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RunPipelineActivityResponseTypeDef,
+    SampleChannelDataResponseTypeDef,
+    StartPipelineReprocessingResponseTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageOutputTypeDef,
-    ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
+    ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
-    DatasetTriggerOutputTypeDef,
     DatasetTriggerTypeDef,
-    DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
-    DatastorePartitionOutputTypeDef,
     DatastorePartitionTypeDef,
-    QueryFilterOutputTypeDef,
-    LateDataRuleConfigurationOutputTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    S3DestinationConfigurationOutputTypeDef,
-    S3DestinationConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    VariableOutputTypeDef,
+    S3DestinationConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     VariableTypeDef,
     PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
     ChannelTypeDef,
-    ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ChannelSummaryTypeDef,
     ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
-    DatastoreStorageOutputTypeDef,
     DatastoreStorageSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
     DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
-    SqlQueryDatasetActionOutputTypeDef,
-    LateDataRuleOutputTypeDef,
     LateDataRuleTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
-    DatasetContentDeliveryDestinationOutputTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
     ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ListChannelsResponseTypeDef,
     FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
     DatastoreSummaryTypeDef,
-    DatasetContentDeliveryRuleOutputTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
     DatastoreTypeDef,
     CreateDatastoreRequestRequestTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.py` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.pyi` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__main__.py` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTAnalytics 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTAnalytics 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.py` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.pyi` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.py` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.pyi` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.py` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -45,96 +45,89 @@
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
     "ListPipelinesPaginator",
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
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
         """
 
-
 class ListDatasetContentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
     """
 
     def paginate(
         self,
         *,
         datasetName: str,
         scheduledOnOrAfter: Union[datetime, str] = ...,
         scheduledBefore: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
-
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
         """
 
-
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
         """
 
-
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.pyi` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,89 +45,96 @@
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
     "ListPipelinesPaginator",
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
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
         """
 
+
 class ListDatasetContentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
     """
 
     def paginate(
         self,
         *,
         datasetName: str,
         scheduledOnOrAfter: Union[datetime, str] = ...,
         scheduledBefore: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
+
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
         """
 
+
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
         """
 
+
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.py` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,182 +39,146 @@
 
 
 __all__ = (
     "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "MessageTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
-    "ChannelActivityOutputTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
-    "CustomerManagedChannelS3StorageOutputTypeDef",
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
-    "RetentionPeriodOutputTypeDef",
-    "ColumnOutputTypeDef",
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
+    "RetentionPeriodTypeDef",
     "ColumnTypeDef",
-    "ResourceConfigurationOutputTypeDef",
     "ResourceConfigurationTypeDef",
-    "RetentionPeriodTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
-    "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
-    "CreatePipelineResponseTypeDef",
-    "CustomerManagedDatastoreS3StorageOutputTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
-    "IotEventsDestinationConfigurationOutputTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
-    "DatasetContentVersionValueOutputTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
-    "ScheduleOutputTypeDef",
-    "TriggeringDatasetOutputTypeDef",
     "ScheduleTypeDef",
     "TriggeringDatasetTypeDef",
-    "VersioningConfigurationOutputTypeDef",
-    "DatastoreActivityOutputTypeDef",
     "DatastoreActivityTypeDef",
-    "IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
-    "PartitionOutputTypeDef",
-    "TimestampPartitionOutputTypeDef",
     "PartitionTypeDef",
     "TimestampPartitionTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteDatasetContentRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
     "DeletePipelineRequestRequestTypeDef",
-    "DeltaTimeOutputTypeDef",
-    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
     "DeltaTimeSessionWindowConfigurationTypeDef",
     "DeltaTimeTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
-    "LoggingOptionsOutputTypeDef",
+    "LoggingOptionsTypeDef",
     "DescribePipelineRequestRequestTypeDef",
-    "DeviceRegistryEnrichActivityOutputTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
-    "DeviceShadowEnrichActivityOutputTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FilterActivityOutputTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
-    "GlueConfigurationOutputTypeDef",
     "GlueConfigurationTypeDef",
-    "LambdaActivityOutputTypeDef",
     "LambdaActivityTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "LoggingOptionsTypeDef",
-    "MathActivityOutputTypeDef",
     "MathActivityTypeDef",
-    "OutputFileUriValueOutputTypeDef",
     "OutputFileUriValueTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveAttributesActivityOutputTypeDef",
     "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataRequestRequestTypeDef",
-    "SampleChannelDataResponseTypeDef",
-    "StartPipelineReprocessingResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageResponseTypeDef",
     "BatchPutMessageRequestRequestTypeDef",
+    "BatchPutMessageResponseTypeDef",
+    "CreateDatasetContentResponseTypeDef",
+    "CreatePipelineResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "RunPipelineActivityResponseTypeDef",
+    "SampleChannelDataResponseTypeDef",
+    "StartPipelineReprocessingResponseTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
     "ChannelStorageOutputTypeDef",
-    "ChannelStorageSummaryTypeDef",
     "ChannelStorageTypeDef",
+    "ChannelStorageSummaryTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
-    "DatasetTriggerOutputTypeDef",
     "DatasetTriggerTypeDef",
-    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
-    "DatastorePartitionOutputTypeDef",
     "DatastorePartitionTypeDef",
-    "QueryFilterOutputTypeDef",
-    "LateDataRuleConfigurationOutputTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "S3DestinationConfigurationOutputTypeDef",
-    "S3DestinationConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
-    "VariableOutputTypeDef",
+    "S3DestinationConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "VariableTypeDef",
     "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
     "ChannelTypeDef",
-    "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "ChannelSummaryTypeDef",
     "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
-    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageSummaryTypeDef",
+    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageTypeDef",
     "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
-    "SqlQueryDatasetActionOutputTypeDef",
-    "LateDataRuleOutputTypeDef",
     "LateDataRuleTypeDef",
+    "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
-    "DatasetContentDeliveryDestinationOutputTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
     "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
     "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
     "DatastoreSummaryTypeDef",
-    "DatasetContentDeliveryRuleOutputTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
     "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
     "DatastoreTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
@@ -284,44 +248,33 @@
     "MessageTypeDef",
     {
         "messageId": str,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "CancelPipelineReprocessingRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "pipelineName": str,
-        "reprocessingId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-_RequiredChannelActivityOutputTypeDef = TypedDict(
-    "_RequiredChannelActivityOutputTypeDef",
-    {
-        "name": str,
-        "channelName": str,
-    },
-)
-_OptionalChannelActivityOutputTypeDef = TypedDict(
-    "_OptionalChannelActivityOutputTypeDef",
+CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "CancelPipelineReprocessingRequestRequestTypeDef",
     {
-        "next": str,
+        "pipelineName": str,
+        "reprocessingId": str,
     },
-    total=False,
 )
 
-
-class ChannelActivityOutputTypeDef(
-    _RequiredChannelActivityOutputTypeDef, _OptionalChannelActivityOutputTypeDef
-):
-    pass
-
-
 _RequiredChannelActivityTypeDef = TypedDict(
     "_RequiredChannelActivityTypeDef",
     {
         "name": str,
         "channelName": str,
     },
 )
@@ -351,119 +304,71 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
-_RequiredCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
-    "_RequiredCustomerManagedChannelS3StorageOutputTypeDef",
+_RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
+    "_RequiredCustomerManagedChannelS3StorageTypeDef",
     {
         "bucket": str,
         "roleArn": str,
     },
 )
-_OptionalCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
-    "_OptionalCustomerManagedChannelS3StorageOutputTypeDef",
+_OptionalCustomerManagedChannelS3StorageTypeDef = TypedDict(
+    "_OptionalCustomerManagedChannelS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
 
-class CustomerManagedChannelS3StorageOutputTypeDef(
-    _RequiredCustomerManagedChannelS3StorageOutputTypeDef,
-    _OptionalCustomerManagedChannelS3StorageOutputTypeDef,
+class CustomerManagedChannelS3StorageTypeDef(
+    _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
 
 CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
     total=False,
 )
 
-_RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
-    "_RequiredCustomerManagedChannelS3StorageTypeDef",
-    {
-        "bucket": str,
-        "roleArn": str,
-    },
-)
-_OptionalCustomerManagedChannelS3StorageTypeDef = TypedDict(
-    "_OptionalCustomerManagedChannelS3StorageTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-
-class CustomerManagedChannelS3StorageTypeDef(
-    _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
-):
-    pass
-
-
-RetentionPeriodOutputTypeDef = TypedDict(
-    "RetentionPeriodOutputTypeDef",
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
 )
 
-ColumnOutputTypeDef = TypedDict(
-    "ColumnOutputTypeDef",
-    {
-        "name": str,
-        "type": str,
-    },
-)
-
 ColumnTypeDef = TypedDict(
     "ColumnTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
-ResourceConfigurationOutputTypeDef = TypedDict(
-    "ResourceConfigurationOutputTypeDef",
-    {
-        "computeType": ComputeTypeType,
-        "volumeSizeInGB": int,
-    },
-)
-
 ResourceConfigurationTypeDef = TypedDict(
     "ResourceConfigurationTypeDef",
     {
         "computeType": ComputeTypeType,
         "volumeSizeInGB": int,
     },
 )
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
-    {
-        "unlimited": bool,
-        "numberOfDays": int,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -486,63 +391,23 @@
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
 
-CreateDatasetContentResponseTypeDef = TypedDict(
-    "CreateDatasetContentResponseTypeDef",
-    {
-        "versionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
 )
 
-CreatePipelineResponseTypeDef = TypedDict(
-    "CreatePipelineResponseTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "bucket": str,
-        "roleArn": str,
-    },
-)
-_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-
-class CustomerManagedDatastoreS3StorageOutputTypeDef(
-    _RequiredCustomerManagedDatastoreS3StorageOutputTypeDef,
-    _OptionalCustomerManagedDatastoreS3StorageOutputTypeDef,
-):
-    pass
-
-
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -577,22 +442,14 @@
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
 )
 
-IotEventsDestinationConfigurationOutputTypeDef = TypedDict(
-    "IotEventsDestinationConfigurationOutputTypeDef",
-    {
-        "inputName": str,
-        "roleArn": str,
-    },
-)
-
 IotEventsDestinationConfigurationTypeDef = TypedDict(
     "IotEventsDestinationConfigurationTypeDef",
     {
         "inputName": str,
         "roleArn": str,
     },
 )
@@ -602,21 +459,14 @@
     {
         "state": DatasetContentStateType,
         "reason": str,
     },
     total=False,
 )
 
-DatasetContentVersionValueOutputTypeDef = TypedDict(
-    "DatasetContentVersionValueOutputTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-
 DatasetContentVersionValueTypeDef = TypedDict(
     "DatasetContentVersionValueTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -625,29 +475,14 @@
     {
         "entryName": str,
         "dataURI": str,
     },
     total=False,
 )
 
-ScheduleOutputTypeDef = TypedDict(
-    "ScheduleOutputTypeDef",
-    {
-        "expression": str,
-    },
-    total=False,
-)
-
-TriggeringDatasetOutputTypeDef = TypedDict(
-    "TriggeringDatasetOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "expression": str,
     },
     total=False,
 )
@@ -655,61 +490,22 @@
 TriggeringDatasetTypeDef = TypedDict(
     "TriggeringDatasetTypeDef",
     {
         "name": str,
     },
 )
 
-VersioningConfigurationOutputTypeDef = TypedDict(
-    "VersioningConfigurationOutputTypeDef",
-    {
-        "unlimited": bool,
-        "maxVersions": int,
-    },
-    total=False,
-)
-
-DatastoreActivityOutputTypeDef = TypedDict(
-    "DatastoreActivityOutputTypeDef",
-    {
-        "name": str,
-        "datastoreName": str,
-    },
-)
-
 DatastoreActivityTypeDef = TypedDict(
     "DatastoreActivityTypeDef",
     {
         "name": str,
         "datastoreName": str,
     },
 )
 
-_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "bucket": str,
-    },
-)
-_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-
-class IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef(
-    _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
-    _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
-):
-    pass
-
-
 IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -733,42 +529,14 @@
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
 
-PartitionOutputTypeDef = TypedDict(
-    "PartitionOutputTypeDef",
-    {
-        "attributeName": str,
-    },
-)
-
-_RequiredTimestampPartitionOutputTypeDef = TypedDict(
-    "_RequiredTimestampPartitionOutputTypeDef",
-    {
-        "attributeName": str,
-    },
-)
-_OptionalTimestampPartitionOutputTypeDef = TypedDict(
-    "_OptionalTimestampPartitionOutputTypeDef",
-    {
-        "timestampFormat": str,
-    },
-    total=False,
-)
-
-
-class TimestampPartitionOutputTypeDef(
-    _RequiredTimestampPartitionOutputTypeDef, _OptionalTimestampPartitionOutputTypeDef
-):
-    pass
-
-
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -839,29 +607,14 @@
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
-DeltaTimeOutputTypeDef = TypedDict(
-    "DeltaTimeOutputTypeDef",
-    {
-        "offsetSeconds": int,
-        "timeExpression": str,
-    },
-)
-
-DeltaTimeSessionWindowConfigurationOutputTypeDef = TypedDict(
-    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
-    {
-        "timeoutInMinutes": int,
-    },
-)
-
 DeltaTimeSessionWindowConfigurationTypeDef = TypedDict(
     "DeltaTimeSessionWindowConfigurationTypeDef",
     {
         "timeoutInMinutes": int,
     },
 )
 
@@ -918,55 +671,30 @@
 
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
 
-LoggingOptionsOutputTypeDef = TypedDict(
-    "LoggingOptionsOutputTypeDef",
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
 )
 
 DescribePipelineRequestRequestTypeDef = TypedDict(
     "DescribePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
-_RequiredDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
-    "_RequiredDeviceRegistryEnrichActivityOutputTypeDef",
-    {
-        "name": str,
-        "attribute": str,
-        "thingName": str,
-        "roleArn": str,
-    },
-)
-_OptionalDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
-    "_OptionalDeviceRegistryEnrichActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class DeviceRegistryEnrichActivityOutputTypeDef(
-    _RequiredDeviceRegistryEnrichActivityOutputTypeDef,
-    _OptionalDeviceRegistryEnrichActivityOutputTypeDef,
-):
-    pass
-
-
 _RequiredDeviceRegistryEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceRegistryEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -983,39 +711,14 @@
 
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
 
-_RequiredDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
-    "_RequiredDeviceShadowEnrichActivityOutputTypeDef",
-    {
-        "name": str,
-        "attribute": str,
-        "thingName": str,
-        "roleArn": str,
-    },
-)
-_OptionalDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
-    "_OptionalDeviceShadowEnrichActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class DeviceShadowEnrichActivityOutputTypeDef(
-    _RequiredDeviceShadowEnrichActivityOutputTypeDef,
-    _OptionalDeviceShadowEnrichActivityOutputTypeDef,
-):
-    pass
-
-
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -1032,43 +735,14 @@
 
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredFilterActivityOutputTypeDef = TypedDict(
-    "_RequiredFilterActivityOutputTypeDef",
-    {
-        "name": str,
-        "filter": str,
-    },
-)
-_OptionalFilterActivityOutputTypeDef = TypedDict(
-    "_OptionalFilterActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class FilterActivityOutputTypeDef(
-    _RequiredFilterActivityOutputTypeDef, _OptionalFilterActivityOutputTypeDef
-):
-    pass
-
-
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -1102,53 +776,22 @@
 
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
 
-GlueConfigurationOutputTypeDef = TypedDict(
-    "GlueConfigurationOutputTypeDef",
-    {
-        "tableName": str,
-        "databaseName": str,
-    },
-)
-
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-_RequiredLambdaActivityOutputTypeDef = TypedDict(
-    "_RequiredLambdaActivityOutputTypeDef",
-    {
-        "name": str,
-        "lambdaName": str,
-        "batchSize": int,
-    },
-)
-_OptionalLambdaActivityOutputTypeDef = TypedDict(
-    "_OptionalLambdaActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class LambdaActivityOutputTypeDef(
-    _RequiredLambdaActivityOutputTypeDef, _OptionalLambdaActivityOutputTypeDef
-):
-    pass
-
-
 _RequiredLambdaActivityTypeDef = TypedDict(
     "_RequiredLambdaActivityTypeDef",
     {
         "name": str,
         "lambdaName": str,
         "batchSize": int,
     },
@@ -1162,55 +805,33 @@
 )
 
 
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
 
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
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
-    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetContentsRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
@@ -1228,56 +849,32 @@
 class ListDatasetContentsRequestRequestTypeDef(
     _RequiredListDatasetContentsRequestRequestTypeDef,
     _OptionalListDatasetContentsRequestRequestTypeDef,
 ):
     pass
 
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1286,54 +883,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
-    {
-        "roleArn": str,
-        "level": Literal["ERROR"],
-        "enabled": bool,
-    },
-)
-
-_RequiredMathActivityOutputTypeDef = TypedDict(
-    "_RequiredMathActivityOutputTypeDef",
-    {
-        "name": str,
-        "attribute": str,
-        "math": str,
-    },
-)
-_OptionalMathActivityOutputTypeDef = TypedDict(
-    "_OptionalMathActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class MathActivityOutputTypeDef(
-    _RequiredMathActivityOutputTypeDef, _OptionalMathActivityOutputTypeDef
-):
-    pass
-
-
 _RequiredMathActivityTypeDef = TypedDict(
     "_RequiredMathActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "math": str,
     },
@@ -1347,38 +904,21 @@
 )
 
 
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
 
-OutputFileUriValueOutputTypeDef = TypedDict(
-    "OutputFileUriValueOutputTypeDef",
-    {
-        "fileName": str,
-    },
-)
-
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
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
 _RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityOutputTypeDef",
     {
         "name": str,
         "attributes": List[str],
     },
 )
@@ -1469,34 +1009,14 @@
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
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
-RunPipelineActivityResponseTypeDef = TypedDict(
-    "RunPipelineActivityResponseTypeDef",
-    {
-        "payloads": List[bytes],
-        "logResult": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
     "_RequiredSampleChannelDataRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
@@ -1512,51 +1032,84 @@
 
 class SampleChannelDataRequestRequestTypeDef(
     _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
 ):
     pass
 
 
-SampleChannelDataResponseTypeDef = TypedDict(
-    "SampleChannelDataResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "payloads": List[bytes],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-StartPipelineReprocessingResponseTypeDef = TypedDict(
-    "StartPipelineReprocessingResponseTypeDef",
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
     {
-        "reprocessingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "channelName": str,
+        "messages": Sequence[MessageTypeDef],
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+BatchPutMessageResponseTypeDef = TypedDict(
+    "BatchPutMessageResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageResponseTypeDef = TypedDict(
-    "BatchPutMessageResponseTypeDef",
+CreateDatasetContentResponseTypeDef = TypedDict(
+    "CreateDatasetContentResponseTypeDef",
     {
-        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "versionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
+CreatePipelineResponseTypeDef = TypedDict(
+    "CreatePipelineResponseTypeDef",
     {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
+        "pipelineName": str,
+        "pipelineArn": str,
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
+RunPipelineActivityResponseTypeDef = TypedDict(
+    "RunPipelineActivityResponseTypeDef",
+    {
+        "payloads": List[bytes],
+        "logResult": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SampleChannelDataResponseTypeDef = TypedDict(
+    "SampleChannelDataResponseTypeDef",
+    {
+        "payloads": List[bytes],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPipelineReprocessingResponseTypeDef = TypedDict(
+    "StartPipelineReprocessingResponseTypeDef",
+    {
+        "reprocessingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
@@ -1596,83 +1149,91 @@
     total=False,
 )
 
 ChannelStorageOutputTypeDef = TypedDict(
     "ChannelStorageOutputTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageOutputTypeDef,
+        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
-ChannelStorageSummaryTypeDef = TypedDict(
-    "ChannelStorageSummaryTypeDef",
+ChannelStorageTypeDef = TypedDict(
+    "ChannelStorageTypeDef",
     {
-        "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
+        "serviceManagedS3": Mapping[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
-ChannelStorageTypeDef = TypedDict(
-    "ChannelStorageTypeDef",
+ChannelStorageSummaryTypeDef = TypedDict(
+    "ChannelStorageSummaryTypeDef",
     {
-        "serviceManagedS3": Mapping[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
     },
     total=False,
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SchemaDefinitionOutputTypeDef = TypedDict(
     "SchemaDefinitionOutputTypeDef",
     {
-        "columns": List[ColumnOutputTypeDef],
+        "columns": List[ColumnTypeDef],
     },
     total=False,
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
     },
     total=False,
 )
 
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
@@ -1691,43 +1252,27 @@
 
 GetDatasetContentResponseTypeDef = TypedDict(
     "GetDatasetContentResponseTypeDef",
     {
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatasetTriggerOutputTypeDef = TypedDict(
-    "DatasetTriggerOutputTypeDef",
-    {
-        "schedule": ScheduleOutputTypeDef,
-        "dataset": TriggeringDatasetOutputTypeDef,
-    },
-    total=False,
-)
-
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
         "dataset": TriggeringDatasetTypeDef,
     },
     total=False,
 )
 
-DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef = TypedDict(
-    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
-    {
-        "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
-    },
-)
-
 DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     },
     total=False,
 )
@@ -1735,48 +1280,23 @@
 DatastoreIotSiteWiseMultiLayerStorageTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     },
 )
 
-DatastorePartitionOutputTypeDef = TypedDict(
-    "DatastorePartitionOutputTypeDef",
-    {
-        "attributePartition": PartitionOutputTypeDef,
-        "timestampPartition": TimestampPartitionOutputTypeDef,
-    },
-    total=False,
-)
-
 DatastorePartitionTypeDef = TypedDict(
     "DatastorePartitionTypeDef",
     {
         "attributePartition": PartitionTypeDef,
         "timestampPartition": TimestampPartitionTypeDef,
     },
     total=False,
 )
 
-QueryFilterOutputTypeDef = TypedDict(
-    "QueryFilterOutputTypeDef",
-    {
-        "deltaTime": DeltaTimeOutputTypeDef,
-    },
-    total=False,
-)
-
-LateDataRuleConfigurationOutputTypeDef = TypedDict(
-    "LateDataRuleConfigurationOutputTypeDef",
-    {
-        "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 LateDataRuleConfigurationTypeDef = TypedDict(
     "LateDataRuleConfigurationTypeDef",
     {
         "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationTypeDef,
     },
     total=False,
 )
@@ -1788,43 +1308,26 @@
     },
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "loggingOptions": LoggingOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredS3DestinationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3DestinationConfigurationOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "roleArn": str,
-    },
-)
-_OptionalS3DestinationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3DestinationConfigurationOutputTypeDef",
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
     {
-        "glueConfiguration": GlueConfigurationOutputTypeDef,
+        "loggingOptions": LoggingOptionsTypeDef,
     },
-    total=False,
 )
 
-
-class S3DestinationConfigurationOutputTypeDef(
-    _RequiredS3DestinationConfigurationOutputTypeDef,
-    _OptionalS3DestinationConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredS3DestinationConfigurationTypeDef = TypedDict(
     "_RequiredS3DestinationConfigurationTypeDef",
     {
         "bucket": str,
         "key": str,
         "roleArn": str,
     },
@@ -1840,50 +1343,69 @@
 
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PutLoggingOptionsRequestRequestTypeDef = TypedDict(
-    "PutLoggingOptionsRequestRequestTypeDef",
+_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "datasetName": str,
     },
 )
-
-_RequiredVariableOutputTypeDef = TypedDict(
-    "_RequiredVariableOutputTypeDef",
+_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
-        "name": str,
+        "scheduledOnOrAfter": Union[datetime, str],
+        "scheduledBefore": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalVariableOutputTypeDef = TypedDict(
-    "_OptionalVariableOutputTypeDef",
+
+
+class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
+    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+):
+    pass
+
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "stringValue": str,
-        "doubleValue": float,
-        "datasetContentVersionValue": DatasetContentVersionValueOutputTypeDef,
-        "outputFileUriValue": OutputFileUriValueOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class VariableOutputTypeDef(_RequiredVariableOutputTypeDef, _OptionalVariableOutputTypeDef):
-    pass
-
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
@@ -1902,24 +1424,24 @@
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
 
 PipelineActivityOutputTypeDef = TypedDict(
     "PipelineActivityOutputTypeDef",
     {
-        "channel": ChannelActivityOutputTypeDef,
-        "lambda": LambdaActivityOutputTypeDef,
-        "datastore": DatastoreActivityOutputTypeDef,
+        "channel": ChannelActivityTypeDef,
+        "lambda": LambdaActivityTypeDef,
+        "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityOutputTypeDef,
         "removeAttributes": RemoveAttributesActivityOutputTypeDef,
         "selectAttributes": SelectAttributesActivityOutputTypeDef,
-        "filter": FilterActivityOutputTypeDef,
-        "math": MathActivityOutputTypeDef,
-        "deviceRegistryEnrich": DeviceRegistryEnrichActivityOutputTypeDef,
-        "deviceShadowEnrich": DeviceShadowEnrichActivityOutputTypeDef,
+        "filter": FilterActivityTypeDef,
+        "math": MathActivityTypeDef,
+        "deviceRegistryEnrich": DeviceRegistryEnrichActivityTypeDef,
+        "deviceShadowEnrich": DeviceShadowEnrichActivityTypeDef,
     },
     total=False,
 )
 
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
@@ -1951,28 +1473,15 @@
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
         "storage": ChannelStorageOutputTypeDef,
         "arn": str,
         "status": ChannelStatusType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
-    },
-    total=False,
-)
-
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
-    {
-        "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
-        "status": ChannelStatusType,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
@@ -2017,14 +1526,27 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
+    {
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
+        "status": ChannelStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+    },
+    total=False,
+)
+
 ParquetConfigurationOutputTypeDef = TypedDict(
     "ParquetConfigurationOutputTypeDef",
     {
         "schemaDefinition": SchemaDefinitionOutputTypeDef,
     },
     total=False,
 )
@@ -2038,47 +1560,47 @@
 )
 
 ListDatasetContentsResponseTypeDef = TypedDict(
     "ListDatasetContentsResponseTypeDef",
     {
         "datasetContentSummaries": List[DatasetContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
         "status": DatasetStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
-        "triggers": List[DatasetTriggerOutputTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
         "actions": List[DatasetActionSummaryTypeDef],
     },
     total=False,
 )
 
-DatastoreStorageOutputTypeDef = TypedDict(
-    "DatastoreStorageOutputTypeDef",
+DatastoreStorageSummaryTypeDef = TypedDict(
+    "DatastoreStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedDatastoreS3StorageOutputTypeDef,
-        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
+        "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
     total=False,
 )
 
-DatastoreStorageSummaryTypeDef = TypedDict(
-    "DatastoreStorageSummaryTypeDef",
+DatastoreStorageOutputTypeDef = TypedDict(
+    "DatastoreStorageOutputTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
-        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
+        "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
 DatastoreStorageTypeDef = TypedDict(
     "DatastoreStorageTypeDef",
     {
@@ -2088,85 +1610,64 @@
     },
     total=False,
 )
 
 DatastorePartitionsOutputTypeDef = TypedDict(
     "DatastorePartitionsOutputTypeDef",
     {
-        "partitions": List[DatastorePartitionOutputTypeDef],
+        "partitions": List[DatastorePartitionTypeDef],
     },
     total=False,
 )
 
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
 
-_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_RequiredSqlQueryDatasetActionOutputTypeDef",
-    {
-        "sqlQuery": str,
-    },
-)
-_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_OptionalSqlQueryDatasetActionOutputTypeDef",
-    {
-        "filters": List[QueryFilterOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class SqlQueryDatasetActionOutputTypeDef(
-    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
-):
-    pass
-
-
-_RequiredLateDataRuleOutputTypeDef = TypedDict(
-    "_RequiredLateDataRuleOutputTypeDef",
+_RequiredLateDataRuleTypeDef = TypedDict(
+    "_RequiredLateDataRuleTypeDef",
     {
-        "ruleConfiguration": LateDataRuleConfigurationOutputTypeDef,
+        "ruleConfiguration": LateDataRuleConfigurationTypeDef,
     },
 )
-_OptionalLateDataRuleOutputTypeDef = TypedDict(
-    "_OptionalLateDataRuleOutputTypeDef",
+_OptionalLateDataRuleTypeDef = TypedDict(
+    "_OptionalLateDataRuleTypeDef",
     {
         "ruleName": str,
     },
     total=False,
 )
 
 
-class LateDataRuleOutputTypeDef(
-    _RequiredLateDataRuleOutputTypeDef, _OptionalLateDataRuleOutputTypeDef
-):
+class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
 
-_RequiredLateDataRuleTypeDef = TypedDict(
-    "_RequiredLateDataRuleTypeDef",
+_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredSqlQueryDatasetActionOutputTypeDef",
     {
-        "ruleConfiguration": LateDataRuleConfigurationTypeDef,
+        "sqlQuery": str,
     },
 )
-_OptionalLateDataRuleTypeDef = TypedDict(
-    "_OptionalLateDataRuleTypeDef",
+_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalSqlQueryDatasetActionOutputTypeDef",
     {
-        "ruleName": str,
+        "filters": List[QueryFilterTypeDef],
     },
     total=False,
 )
 
 
-class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
+class SqlQueryDatasetActionOutputTypeDef(
+    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
+):
     pass
 
 
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
@@ -2183,44 +1684,35 @@
 
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
 
-DatasetContentDeliveryDestinationOutputTypeDef = TypedDict(
-    "DatasetContentDeliveryDestinationOutputTypeDef",
-    {
-        "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationOutputTypeDef,
-        "s3DestinationConfiguration": S3DestinationConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredContainerDatasetActionOutputTypeDef = TypedDict(
     "_RequiredContainerDatasetActionOutputTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
-        "resourceConfiguration": ResourceConfigurationOutputTypeDef,
+        "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
 _OptionalContainerDatasetActionOutputTypeDef = TypedDict(
     "_OptionalContainerDatasetActionOutputTypeDef",
     {
-        "variables": List[VariableOutputTypeDef],
+        "variables": List[VariableTypeDef],
     },
     total=False,
 )
 
 
 class ContainerDatasetActionOutputTypeDef(
     _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
@@ -2303,33 +1795,33 @@
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FileFormatConfigurationOutputTypeDef = TypedDict(
     "FileFormatConfigurationOutputTypeDef",
     {
         "jsonConfiguration": Dict[str, Any],
@@ -2348,15 +1840,15 @@
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
@@ -2367,36 +1859,14 @@
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
         "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
-    "_RequiredDatasetContentDeliveryRuleOutputTypeDef",
-    {
-        "destination": DatasetContentDeliveryDestinationOutputTypeDef,
-    },
-)
-_OptionalDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
-    "_OptionalDatasetContentDeliveryRuleOutputTypeDef",
-    {
-        "entryName": str,
-    },
-    total=False,
-)
-
-
-class DatasetContentDeliveryRuleOutputTypeDef(
-    _RequiredDatasetContentDeliveryRuleOutputTypeDef,
-    _OptionalDatasetContentDeliveryRuleOutputTypeDef,
-):
-    pass
-
-
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
@@ -2434,26 +1904,26 @@
     total=False,
 )
 
 DescribePipelineResponseTypeDef = TypedDict(
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
         "storage": DatastoreStorageOutputTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
         "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
@@ -2508,32 +1978,32 @@
 
 
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "name": str,
         "arn": str,
         "actions": List[DatasetActionOutputTypeDef],
-        "triggers": List[DatasetTriggerOutputTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleOutputTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
         "status": DatasetStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "versioningConfiguration": VersioningConfigurationOutputTypeDef,
-        "lateDataRules": List[LateDataRuleOutputTypeDef],
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "versioningConfiguration": VersioningConfigurationTypeDef,
+        "lateDataRules": List[LateDataRuleTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
@@ -2588,18 +2058,18 @@
 
 
 DescribeDatastoreResponseTypeDef = TypedDict(
     "DescribeDatastoreResponseTypeDef",
     {
         "datastore": DatastoreTypeDef,
         "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.pyi` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -38,182 +38,146 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "MessageTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
-    "ChannelActivityOutputTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
-    "CustomerManagedChannelS3StorageOutputTypeDef",
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
-    "RetentionPeriodOutputTypeDef",
-    "ColumnOutputTypeDef",
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
+    "RetentionPeriodTypeDef",
     "ColumnTypeDef",
-    "ResourceConfigurationOutputTypeDef",
     "ResourceConfigurationTypeDef",
-    "RetentionPeriodTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
-    "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
-    "CreatePipelineResponseTypeDef",
-    "CustomerManagedDatastoreS3StorageOutputTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
-    "IotEventsDestinationConfigurationOutputTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
-    "DatasetContentVersionValueOutputTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
-    "ScheduleOutputTypeDef",
-    "TriggeringDatasetOutputTypeDef",
     "ScheduleTypeDef",
     "TriggeringDatasetTypeDef",
-    "VersioningConfigurationOutputTypeDef",
-    "DatastoreActivityOutputTypeDef",
     "DatastoreActivityTypeDef",
-    "IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
-    "PartitionOutputTypeDef",
-    "TimestampPartitionOutputTypeDef",
     "PartitionTypeDef",
     "TimestampPartitionTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteDatasetContentRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
     "DeletePipelineRequestRequestTypeDef",
-    "DeltaTimeOutputTypeDef",
-    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
     "DeltaTimeSessionWindowConfigurationTypeDef",
     "DeltaTimeTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
-    "LoggingOptionsOutputTypeDef",
+    "LoggingOptionsTypeDef",
     "DescribePipelineRequestRequestTypeDef",
-    "DeviceRegistryEnrichActivityOutputTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
-    "DeviceShadowEnrichActivityOutputTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FilterActivityOutputTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
-    "GlueConfigurationOutputTypeDef",
     "GlueConfigurationTypeDef",
-    "LambdaActivityOutputTypeDef",
     "LambdaActivityTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "LoggingOptionsTypeDef",
-    "MathActivityOutputTypeDef",
     "MathActivityTypeDef",
-    "OutputFileUriValueOutputTypeDef",
     "OutputFileUriValueTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveAttributesActivityOutputTypeDef",
     "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataRequestRequestTypeDef",
-    "SampleChannelDataResponseTypeDef",
-    "StartPipelineReprocessingResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageResponseTypeDef",
     "BatchPutMessageRequestRequestTypeDef",
+    "BatchPutMessageResponseTypeDef",
+    "CreateDatasetContentResponseTypeDef",
+    "CreatePipelineResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "RunPipelineActivityResponseTypeDef",
+    "SampleChannelDataResponseTypeDef",
+    "StartPipelineReprocessingResponseTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
     "ChannelStorageOutputTypeDef",
-    "ChannelStorageSummaryTypeDef",
     "ChannelStorageTypeDef",
+    "ChannelStorageSummaryTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
-    "DatasetTriggerOutputTypeDef",
     "DatasetTriggerTypeDef",
-    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
-    "DatastorePartitionOutputTypeDef",
     "DatastorePartitionTypeDef",
-    "QueryFilterOutputTypeDef",
-    "LateDataRuleConfigurationOutputTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "S3DestinationConfigurationOutputTypeDef",
-    "S3DestinationConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
-    "VariableOutputTypeDef",
+    "S3DestinationConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "VariableTypeDef",
     "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
     "ChannelTypeDef",
-    "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "ChannelSummaryTypeDef",
     "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
-    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageSummaryTypeDef",
+    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageTypeDef",
     "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
-    "SqlQueryDatasetActionOutputTypeDef",
-    "LateDataRuleOutputTypeDef",
     "LateDataRuleTypeDef",
+    "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
-    "DatasetContentDeliveryDestinationOutputTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
     "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
     "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
     "DatastoreSummaryTypeDef",
-    "DatasetContentDeliveryRuleOutputTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
     "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
     "DatastoreTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
@@ -279,42 +243,33 @@
     "MessageTypeDef",
     {
         "messageId": str,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "CancelPipelineReprocessingRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "pipelineName": str,
-        "reprocessingId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-_RequiredChannelActivityOutputTypeDef = TypedDict(
-    "_RequiredChannelActivityOutputTypeDef",
-    {
-        "name": str,
-        "channelName": str,
-    },
-)
-_OptionalChannelActivityOutputTypeDef = TypedDict(
-    "_OptionalChannelActivityOutputTypeDef",
+CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "CancelPipelineReprocessingRequestRequestTypeDef",
     {
-        "next": str,
+        "pipelineName": str,
+        "reprocessingId": str,
     },
-    total=False,
 )
 
-class ChannelActivityOutputTypeDef(
-    _RequiredChannelActivityOutputTypeDef, _OptionalChannelActivityOutputTypeDef
-):
-    pass
-
 _RequiredChannelActivityTypeDef = TypedDict(
     "_RequiredChannelActivityTypeDef",
     {
         "name": str,
         "channelName": str,
     },
 )
@@ -342,115 +297,69 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
-_RequiredCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
-    "_RequiredCustomerManagedChannelS3StorageOutputTypeDef",
+_RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
+    "_RequiredCustomerManagedChannelS3StorageTypeDef",
     {
         "bucket": str,
         "roleArn": str,
     },
 )
-_OptionalCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
-    "_OptionalCustomerManagedChannelS3StorageOutputTypeDef",
+_OptionalCustomerManagedChannelS3StorageTypeDef = TypedDict(
+    "_OptionalCustomerManagedChannelS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-class CustomerManagedChannelS3StorageOutputTypeDef(
-    _RequiredCustomerManagedChannelS3StorageOutputTypeDef,
-    _OptionalCustomerManagedChannelS3StorageOutputTypeDef,
+class CustomerManagedChannelS3StorageTypeDef(
+    _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
 CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
     total=False,
 )
 
-_RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
-    "_RequiredCustomerManagedChannelS3StorageTypeDef",
-    {
-        "bucket": str,
-        "roleArn": str,
-    },
-)
-_OptionalCustomerManagedChannelS3StorageTypeDef = TypedDict(
-    "_OptionalCustomerManagedChannelS3StorageTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-class CustomerManagedChannelS3StorageTypeDef(
-    _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
-):
-    pass
-
-RetentionPeriodOutputTypeDef = TypedDict(
-    "RetentionPeriodOutputTypeDef",
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
 )
 
-ColumnOutputTypeDef = TypedDict(
-    "ColumnOutputTypeDef",
-    {
-        "name": str,
-        "type": str,
-    },
-)
-
 ColumnTypeDef = TypedDict(
     "ColumnTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
-ResourceConfigurationOutputTypeDef = TypedDict(
-    "ResourceConfigurationOutputTypeDef",
-    {
-        "computeType": ComputeTypeType,
-        "volumeSizeInGB": int,
-    },
-)
-
 ResourceConfigurationTypeDef = TypedDict(
     "ResourceConfigurationTypeDef",
     {
         "computeType": ComputeTypeType,
         "volumeSizeInGB": int,
     },
 )
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
-    {
-        "unlimited": bool,
-        "numberOfDays": int,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -471,61 +380,23 @@
 
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
-CreateDatasetContentResponseTypeDef = TypedDict(
-    "CreateDatasetContentResponseTypeDef",
-    {
-        "versionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
 )
 
-CreatePipelineResponseTypeDef = TypedDict(
-    "CreatePipelineResponseTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "bucket": str,
-        "roleArn": str,
-    },
-)
-_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-class CustomerManagedDatastoreS3StorageOutputTypeDef(
-    _RequiredCustomerManagedDatastoreS3StorageOutputTypeDef,
-    _OptionalCustomerManagedDatastoreS3StorageOutputTypeDef,
-):
-    pass
-
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -558,22 +429,14 @@
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
 )
 
-IotEventsDestinationConfigurationOutputTypeDef = TypedDict(
-    "IotEventsDestinationConfigurationOutputTypeDef",
-    {
-        "inputName": str,
-        "roleArn": str,
-    },
-)
-
 IotEventsDestinationConfigurationTypeDef = TypedDict(
     "IotEventsDestinationConfigurationTypeDef",
     {
         "inputName": str,
         "roleArn": str,
     },
 )
@@ -583,21 +446,14 @@
     {
         "state": DatasetContentStateType,
         "reason": str,
     },
     total=False,
 )
 
-DatasetContentVersionValueOutputTypeDef = TypedDict(
-    "DatasetContentVersionValueOutputTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-
 DatasetContentVersionValueTypeDef = TypedDict(
     "DatasetContentVersionValueTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -606,29 +462,14 @@
     {
         "entryName": str,
         "dataURI": str,
     },
     total=False,
 )
 
-ScheduleOutputTypeDef = TypedDict(
-    "ScheduleOutputTypeDef",
-    {
-        "expression": str,
-    },
-    total=False,
-)
-
-TriggeringDatasetOutputTypeDef = TypedDict(
-    "TriggeringDatasetOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "expression": str,
     },
     total=False,
 )
@@ -636,59 +477,22 @@
 TriggeringDatasetTypeDef = TypedDict(
     "TriggeringDatasetTypeDef",
     {
         "name": str,
     },
 )
 
-VersioningConfigurationOutputTypeDef = TypedDict(
-    "VersioningConfigurationOutputTypeDef",
-    {
-        "unlimited": bool,
-        "maxVersions": int,
-    },
-    total=False,
-)
-
-DatastoreActivityOutputTypeDef = TypedDict(
-    "DatastoreActivityOutputTypeDef",
-    {
-        "name": str,
-        "datastoreName": str,
-    },
-)
-
 DatastoreActivityTypeDef = TypedDict(
     "DatastoreActivityTypeDef",
     {
         "name": str,
         "datastoreName": str,
     },
 )
 
-_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "bucket": str,
-    },
-)
-_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
-    "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-class IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef(
-    _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
-    _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
-):
-    pass
-
 IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -710,40 +514,14 @@
 
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
-PartitionOutputTypeDef = TypedDict(
-    "PartitionOutputTypeDef",
-    {
-        "attributeName": str,
-    },
-)
-
-_RequiredTimestampPartitionOutputTypeDef = TypedDict(
-    "_RequiredTimestampPartitionOutputTypeDef",
-    {
-        "attributeName": str,
-    },
-)
-_OptionalTimestampPartitionOutputTypeDef = TypedDict(
-    "_OptionalTimestampPartitionOutputTypeDef",
-    {
-        "timestampFormat": str,
-    },
-    total=False,
-)
-
-class TimestampPartitionOutputTypeDef(
-    _RequiredTimestampPartitionOutputTypeDef, _OptionalTimestampPartitionOutputTypeDef
-):
-    pass
-
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -810,29 +588,14 @@
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
-DeltaTimeOutputTypeDef = TypedDict(
-    "DeltaTimeOutputTypeDef",
-    {
-        "offsetSeconds": int,
-        "timeExpression": str,
-    },
-)
-
-DeltaTimeSessionWindowConfigurationOutputTypeDef = TypedDict(
-    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
-    {
-        "timeoutInMinutes": int,
-    },
-)
-
 DeltaTimeSessionWindowConfigurationTypeDef = TypedDict(
     "DeltaTimeSessionWindowConfigurationTypeDef",
     {
         "timeoutInMinutes": int,
     },
 )
 
@@ -885,53 +648,30 @@
 )
 
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
-LoggingOptionsOutputTypeDef = TypedDict(
-    "LoggingOptionsOutputTypeDef",
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
 )
 
 DescribePipelineRequestRequestTypeDef = TypedDict(
     "DescribePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
-_RequiredDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
-    "_RequiredDeviceRegistryEnrichActivityOutputTypeDef",
-    {
-        "name": str,
-        "attribute": str,
-        "thingName": str,
-        "roleArn": str,
-    },
-)
-_OptionalDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
-    "_OptionalDeviceRegistryEnrichActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class DeviceRegistryEnrichActivityOutputTypeDef(
-    _RequiredDeviceRegistryEnrichActivityOutputTypeDef,
-    _OptionalDeviceRegistryEnrichActivityOutputTypeDef,
-):
-    pass
-
 _RequiredDeviceRegistryEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceRegistryEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -946,37 +686,14 @@
 )
 
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
-_RequiredDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
-    "_RequiredDeviceShadowEnrichActivityOutputTypeDef",
-    {
-        "name": str,
-        "attribute": str,
-        "thingName": str,
-        "roleArn": str,
-    },
-)
-_OptionalDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
-    "_OptionalDeviceShadowEnrichActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class DeviceShadowEnrichActivityOutputTypeDef(
-    _RequiredDeviceShadowEnrichActivityOutputTypeDef,
-    _OptionalDeviceShadowEnrichActivityOutputTypeDef,
-):
-    pass
-
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -991,41 +708,14 @@
 )
 
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredFilterActivityOutputTypeDef = TypedDict(
-    "_RequiredFilterActivityOutputTypeDef",
-    {
-        "name": str,
-        "filter": str,
-    },
-)
-_OptionalFilterActivityOutputTypeDef = TypedDict(
-    "_OptionalFilterActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class FilterActivityOutputTypeDef(
-    _RequiredFilterActivityOutputTypeDef, _OptionalFilterActivityOutputTypeDef
-):
-    pass
-
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -1055,51 +745,22 @@
 )
 
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
-GlueConfigurationOutputTypeDef = TypedDict(
-    "GlueConfigurationOutputTypeDef",
-    {
-        "tableName": str,
-        "databaseName": str,
-    },
-)
-
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-_RequiredLambdaActivityOutputTypeDef = TypedDict(
-    "_RequiredLambdaActivityOutputTypeDef",
-    {
-        "name": str,
-        "lambdaName": str,
-        "batchSize": int,
-    },
-)
-_OptionalLambdaActivityOutputTypeDef = TypedDict(
-    "_OptionalLambdaActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class LambdaActivityOutputTypeDef(
-    _RequiredLambdaActivityOutputTypeDef, _OptionalLambdaActivityOutputTypeDef
-):
-    pass
-
 _RequiredLambdaActivityTypeDef = TypedDict(
     "_RequiredLambdaActivityTypeDef",
     {
         "name": str,
         "lambdaName": str,
         "batchSize": int,
     },
@@ -1111,53 +772,33 @@
     },
     total=False,
 )
 
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
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
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
-    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetContentsRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
@@ -1173,56 +814,32 @@
 
 class ListDatasetContentsRequestRequestTypeDef(
     _RequiredListDatasetContentsRequestRequestTypeDef,
     _OptionalListDatasetContentsRequestRequestTypeDef,
 ):
     pass
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1231,52 +848,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
-    {
-        "roleArn": str,
-        "level": Literal["ERROR"],
-        "enabled": bool,
-    },
-)
-
-_RequiredMathActivityOutputTypeDef = TypedDict(
-    "_RequiredMathActivityOutputTypeDef",
-    {
-        "name": str,
-        "attribute": str,
-        "math": str,
-    },
-)
-_OptionalMathActivityOutputTypeDef = TypedDict(
-    "_OptionalMathActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class MathActivityOutputTypeDef(
-    _RequiredMathActivityOutputTypeDef, _OptionalMathActivityOutputTypeDef
-):
-    pass
-
 _RequiredMathActivityTypeDef = TypedDict(
     "_RequiredMathActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "math": str,
     },
@@ -1288,38 +867,21 @@
     },
     total=False,
 )
 
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
-OutputFileUriValueOutputTypeDef = TypedDict(
-    "OutputFileUriValueOutputTypeDef",
-    {
-        "fileName": str,
-    },
-)
-
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
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
 _RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityOutputTypeDef",
     {
         "name": str,
         "attributes": List[str],
     },
 )
@@ -1402,34 +964,14 @@
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
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
-RunPipelineActivityResponseTypeDef = TypedDict(
-    "RunPipelineActivityResponseTypeDef",
-    {
-        "payloads": List[bytes],
-        "logResult": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
     "_RequiredSampleChannelDataRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
@@ -1443,51 +985,84 @@
 )
 
 class SampleChannelDataRequestRequestTypeDef(
     _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
 ):
     pass
 
-SampleChannelDataResponseTypeDef = TypedDict(
-    "SampleChannelDataResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "payloads": List[bytes],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-StartPipelineReprocessingResponseTypeDef = TypedDict(
-    "StartPipelineReprocessingResponseTypeDef",
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
     {
-        "reprocessingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "channelName": str,
+        "messages": Sequence[MessageTypeDef],
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+BatchPutMessageResponseTypeDef = TypedDict(
+    "BatchPutMessageResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageResponseTypeDef = TypedDict(
-    "BatchPutMessageResponseTypeDef",
+CreateDatasetContentResponseTypeDef = TypedDict(
+    "CreateDatasetContentResponseTypeDef",
     {
-        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "versionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
+CreatePipelineResponseTypeDef = TypedDict(
+    "CreatePipelineResponseTypeDef",
     {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
+        "pipelineName": str,
+        "pipelineArn": str,
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
+RunPipelineActivityResponseTypeDef = TypedDict(
+    "RunPipelineActivityResponseTypeDef",
+    {
+        "payloads": List[bytes],
+        "logResult": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SampleChannelDataResponseTypeDef = TypedDict(
+    "SampleChannelDataResponseTypeDef",
+    {
+        "payloads": List[bytes],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPipelineReprocessingResponseTypeDef = TypedDict(
+    "StartPipelineReprocessingResponseTypeDef",
+    {
+        "reprocessingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
@@ -1525,83 +1100,91 @@
     total=False,
 )
 
 ChannelStorageOutputTypeDef = TypedDict(
     "ChannelStorageOutputTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageOutputTypeDef,
+        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
-ChannelStorageSummaryTypeDef = TypedDict(
-    "ChannelStorageSummaryTypeDef",
+ChannelStorageTypeDef = TypedDict(
+    "ChannelStorageTypeDef",
     {
-        "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
+        "serviceManagedS3": Mapping[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
-ChannelStorageTypeDef = TypedDict(
-    "ChannelStorageTypeDef",
+ChannelStorageSummaryTypeDef = TypedDict(
+    "ChannelStorageSummaryTypeDef",
     {
-        "serviceManagedS3": Mapping[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
     },
     total=False,
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SchemaDefinitionOutputTypeDef = TypedDict(
     "SchemaDefinitionOutputTypeDef",
     {
-        "columns": List[ColumnOutputTypeDef],
+        "columns": List[ColumnTypeDef],
     },
     total=False,
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
     },
     total=False,
 )
 
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
@@ -1620,43 +1203,27 @@
 
 GetDatasetContentResponseTypeDef = TypedDict(
     "GetDatasetContentResponseTypeDef",
     {
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatasetTriggerOutputTypeDef = TypedDict(
-    "DatasetTriggerOutputTypeDef",
-    {
-        "schedule": ScheduleOutputTypeDef,
-        "dataset": TriggeringDatasetOutputTypeDef,
-    },
-    total=False,
-)
-
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
         "dataset": TriggeringDatasetTypeDef,
     },
     total=False,
 )
 
-DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef = TypedDict(
-    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
-    {
-        "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
-    },
-)
-
 DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     },
     total=False,
 )
@@ -1664,48 +1231,23 @@
 DatastoreIotSiteWiseMultiLayerStorageTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     },
 )
 
-DatastorePartitionOutputTypeDef = TypedDict(
-    "DatastorePartitionOutputTypeDef",
-    {
-        "attributePartition": PartitionOutputTypeDef,
-        "timestampPartition": TimestampPartitionOutputTypeDef,
-    },
-    total=False,
-)
-
 DatastorePartitionTypeDef = TypedDict(
     "DatastorePartitionTypeDef",
     {
         "attributePartition": PartitionTypeDef,
         "timestampPartition": TimestampPartitionTypeDef,
     },
     total=False,
 )
 
-QueryFilterOutputTypeDef = TypedDict(
-    "QueryFilterOutputTypeDef",
-    {
-        "deltaTime": DeltaTimeOutputTypeDef,
-    },
-    total=False,
-)
-
-LateDataRuleConfigurationOutputTypeDef = TypedDict(
-    "LateDataRuleConfigurationOutputTypeDef",
-    {
-        "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 LateDataRuleConfigurationTypeDef = TypedDict(
     "LateDataRuleConfigurationTypeDef",
     {
         "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationTypeDef,
     },
     total=False,
 )
@@ -1717,41 +1259,26 @@
     },
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "loggingOptions": LoggingOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredS3DestinationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3DestinationConfigurationOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "roleArn": str,
-    },
-)
-_OptionalS3DestinationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3DestinationConfigurationOutputTypeDef",
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
     {
-        "glueConfiguration": GlueConfigurationOutputTypeDef,
+        "loggingOptions": LoggingOptionsTypeDef,
     },
-    total=False,
 )
 
-class S3DestinationConfigurationOutputTypeDef(
-    _RequiredS3DestinationConfigurationOutputTypeDef,
-    _OptionalS3DestinationConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredS3DestinationConfigurationTypeDef = TypedDict(
     "_RequiredS3DestinationConfigurationTypeDef",
     {
         "bucket": str,
         "key": str,
         "roleArn": str,
     },
@@ -1765,48 +1292,67 @@
 )
 
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PutLoggingOptionsRequestRequestTypeDef = TypedDict(
-    "PutLoggingOptionsRequestRequestTypeDef",
+_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "datasetName": str,
     },
 )
+_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "scheduledOnOrAfter": Union[datetime, str],
+        "scheduledBefore": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
+    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+):
+    pass
 
-_RequiredVariableOutputTypeDef = TypedDict(
-    "_RequiredVariableOutputTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalVariableOutputTypeDef = TypedDict(
-    "_OptionalVariableOutputTypeDef",
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     {
-        "stringValue": str,
-        "doubleValue": float,
-        "datasetContentVersionValue": DatasetContentVersionValueOutputTypeDef,
-        "outputFileUriValue": OutputFileUriValueOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class VariableOutputTypeDef(_RequiredVariableOutputTypeDef, _OptionalVariableOutputTypeDef):
-    pass
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
@@ -1823,24 +1369,24 @@
 
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
 PipelineActivityOutputTypeDef = TypedDict(
     "PipelineActivityOutputTypeDef",
     {
-        "channel": ChannelActivityOutputTypeDef,
-        "lambda": LambdaActivityOutputTypeDef,
-        "datastore": DatastoreActivityOutputTypeDef,
+        "channel": ChannelActivityTypeDef,
+        "lambda": LambdaActivityTypeDef,
+        "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityOutputTypeDef,
         "removeAttributes": RemoveAttributesActivityOutputTypeDef,
         "selectAttributes": SelectAttributesActivityOutputTypeDef,
-        "filter": FilterActivityOutputTypeDef,
-        "math": MathActivityOutputTypeDef,
-        "deviceRegistryEnrich": DeviceRegistryEnrichActivityOutputTypeDef,
-        "deviceShadowEnrich": DeviceShadowEnrichActivityOutputTypeDef,
+        "filter": FilterActivityTypeDef,
+        "math": MathActivityTypeDef,
+        "deviceRegistryEnrich": DeviceRegistryEnrichActivityTypeDef,
+        "deviceShadowEnrich": DeviceShadowEnrichActivityTypeDef,
     },
     total=False,
 )
 
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
@@ -1872,28 +1418,15 @@
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
         "storage": ChannelStorageOutputTypeDef,
         "arn": str,
         "status": ChannelStatusType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
-    },
-    total=False,
-)
-
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
-    {
-        "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
-        "status": ChannelStatusType,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
@@ -1934,14 +1467,27 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
+    {
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
+        "status": ChannelStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+    },
+    total=False,
+)
+
 ParquetConfigurationOutputTypeDef = TypedDict(
     "ParquetConfigurationOutputTypeDef",
     {
         "schemaDefinition": SchemaDefinitionOutputTypeDef,
     },
     total=False,
 )
@@ -1955,47 +1501,47 @@
 )
 
 ListDatasetContentsResponseTypeDef = TypedDict(
     "ListDatasetContentsResponseTypeDef",
     {
         "datasetContentSummaries": List[DatasetContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
         "status": DatasetStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
-        "triggers": List[DatasetTriggerOutputTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
         "actions": List[DatasetActionSummaryTypeDef],
     },
     total=False,
 )
 
-DatastoreStorageOutputTypeDef = TypedDict(
-    "DatastoreStorageOutputTypeDef",
+DatastoreStorageSummaryTypeDef = TypedDict(
+    "DatastoreStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedDatastoreS3StorageOutputTypeDef,
-        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
+        "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
     total=False,
 )
 
-DatastoreStorageSummaryTypeDef = TypedDict(
-    "DatastoreStorageSummaryTypeDef",
+DatastoreStorageOutputTypeDef = TypedDict(
+    "DatastoreStorageOutputTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
-        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
+        "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
 DatastoreStorageTypeDef = TypedDict(
     "DatastoreStorageTypeDef",
     {
@@ -2005,80 +1551,61 @@
     },
     total=False,
 )
 
 DatastorePartitionsOutputTypeDef = TypedDict(
     "DatastorePartitionsOutputTypeDef",
     {
-        "partitions": List[DatastorePartitionOutputTypeDef],
+        "partitions": List[DatastorePartitionTypeDef],
     },
     total=False,
 )
 
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
 
-_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_RequiredSqlQueryDatasetActionOutputTypeDef",
-    {
-        "sqlQuery": str,
-    },
-)
-_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_OptionalSqlQueryDatasetActionOutputTypeDef",
-    {
-        "filters": List[QueryFilterOutputTypeDef],
-    },
-    total=False,
-)
-
-class SqlQueryDatasetActionOutputTypeDef(
-    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
-):
-    pass
-
-_RequiredLateDataRuleOutputTypeDef = TypedDict(
-    "_RequiredLateDataRuleOutputTypeDef",
+_RequiredLateDataRuleTypeDef = TypedDict(
+    "_RequiredLateDataRuleTypeDef",
     {
-        "ruleConfiguration": LateDataRuleConfigurationOutputTypeDef,
+        "ruleConfiguration": LateDataRuleConfigurationTypeDef,
     },
 )
-_OptionalLateDataRuleOutputTypeDef = TypedDict(
-    "_OptionalLateDataRuleOutputTypeDef",
+_OptionalLateDataRuleTypeDef = TypedDict(
+    "_OptionalLateDataRuleTypeDef",
     {
         "ruleName": str,
     },
     total=False,
 )
 
-class LateDataRuleOutputTypeDef(
-    _RequiredLateDataRuleOutputTypeDef, _OptionalLateDataRuleOutputTypeDef
-):
+class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
-_RequiredLateDataRuleTypeDef = TypedDict(
-    "_RequiredLateDataRuleTypeDef",
+_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredSqlQueryDatasetActionOutputTypeDef",
     {
-        "ruleConfiguration": LateDataRuleConfigurationTypeDef,
+        "sqlQuery": str,
     },
 )
-_OptionalLateDataRuleTypeDef = TypedDict(
-    "_OptionalLateDataRuleTypeDef",
+_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalSqlQueryDatasetActionOutputTypeDef",
     {
-        "ruleName": str,
+        "filters": List[QueryFilterTypeDef],
     },
     total=False,
 )
 
-class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
+class SqlQueryDatasetActionOutputTypeDef(
+    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
+):
     pass
 
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
@@ -2092,44 +1619,35 @@
 )
 
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
-DatasetContentDeliveryDestinationOutputTypeDef = TypedDict(
-    "DatasetContentDeliveryDestinationOutputTypeDef",
-    {
-        "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationOutputTypeDef,
-        "s3DestinationConfiguration": S3DestinationConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredContainerDatasetActionOutputTypeDef = TypedDict(
     "_RequiredContainerDatasetActionOutputTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
-        "resourceConfiguration": ResourceConfigurationOutputTypeDef,
+        "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
 _OptionalContainerDatasetActionOutputTypeDef = TypedDict(
     "_OptionalContainerDatasetActionOutputTypeDef",
     {
-        "variables": List[VariableOutputTypeDef],
+        "variables": List[VariableTypeDef],
     },
     total=False,
 )
 
 class ContainerDatasetActionOutputTypeDef(
     _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
 ):
@@ -2206,33 +1724,33 @@
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FileFormatConfigurationOutputTypeDef = TypedDict(
     "FileFormatConfigurationOutputTypeDef",
     {
         "jsonConfiguration": Dict[str, Any],
@@ -2251,15 +1769,15 @@
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
@@ -2270,34 +1788,14 @@
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
         "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
-    "_RequiredDatasetContentDeliveryRuleOutputTypeDef",
-    {
-        "destination": DatasetContentDeliveryDestinationOutputTypeDef,
-    },
-)
-_OptionalDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
-    "_OptionalDatasetContentDeliveryRuleOutputTypeDef",
-    {
-        "entryName": str,
-    },
-    total=False,
-)
-
-class DatasetContentDeliveryRuleOutputTypeDef(
-    _RequiredDatasetContentDeliveryRuleOutputTypeDef,
-    _OptionalDatasetContentDeliveryRuleOutputTypeDef,
-):
-    pass
-
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
@@ -2333,26 +1831,26 @@
     total=False,
 )
 
 DescribePipelineResponseTypeDef = TypedDict(
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
         "storage": DatastoreStorageOutputTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
         "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
@@ -2403,32 +1901,32 @@
     pass
 
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "name": str,
         "arn": str,
         "actions": List[DatasetActionOutputTypeDef],
-        "triggers": List[DatasetTriggerOutputTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleOutputTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
         "status": DatasetStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "versioningConfiguration": VersioningConfigurationOutputTypeDef,
-        "lateDataRules": List[LateDataRuleOutputTypeDef],
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "versioningConfiguration": VersioningConfigurationTypeDef,
+        "lateDataRules": List[LateDataRuleTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
@@ -2479,18 +1977,18 @@
     pass
 
 DescribeDatastoreResponseTypeDef = TypedDict(
     "DescribeDatastoreResponseTypeDef",
     {
         "datastore": DatastoreTypeDef,
         "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,182 +348,146 @@
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
+    ResponseMetadataTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
-    ChannelActivityOutputTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
-    CustomerManagedChannelS3StorageOutputTypeDef,
-    CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
-    RetentionPeriodOutputTypeDef,
-    ColumnOutputTypeDef,
+    CustomerManagedChannelS3StorageSummaryTypeDef,
+    RetentionPeriodTypeDef,
     ColumnTypeDef,
-    ResourceConfigurationOutputTypeDef,
     ResourceConfigurationTypeDef,
-    RetentionPeriodTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
-    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
-    CreatePipelineResponseTypeDef,
-    CustomerManagedDatastoreS3StorageOutputTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
-    IotEventsDestinationConfigurationOutputTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
-    DatasetContentVersionValueOutputTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
-    ScheduleOutputTypeDef,
-    TriggeringDatasetOutputTypeDef,
     ScheduleTypeDef,
     TriggeringDatasetTypeDef,
-    VersioningConfigurationOutputTypeDef,
-    DatastoreActivityOutputTypeDef,
     DatastoreActivityTypeDef,
-    IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
-    PartitionOutputTypeDef,
-    TimestampPartitionOutputTypeDef,
     PartitionTypeDef,
     TimestampPartitionTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteDatasetContentRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeletePipelineRequestRequestTypeDef,
-    DeltaTimeOutputTypeDef,
-    DeltaTimeSessionWindowConfigurationOutputTypeDef,
     DeltaTimeSessionWindowConfigurationTypeDef,
     DeltaTimeTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
-    LoggingOptionsOutputTypeDef,
+    LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
-    DeviceRegistryEnrichActivityOutputTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
-    DeviceShadowEnrichActivityOutputTypeDef,
     DeviceShadowEnrichActivityTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FilterActivityOutputTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
-    GlueConfigurationOutputTypeDef,
     GlueConfigurationTypeDef,
-    LambdaActivityOutputTypeDef,
     LambdaActivityTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    LoggingOptionsTypeDef,
-    MathActivityOutputTypeDef,
     MathActivityTypeDef,
-    OutputFileUriValueOutputTypeDef,
     OutputFileUriValueTypeDef,
-    PaginatorConfigTypeDef,
     RemoveAttributesActivityOutputTypeDef,
     SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RunPipelineActivityResponseTypeDef,
     SampleChannelDataRequestRequestTypeDef,
-    SampleChannelDataResponseTypeDef,
-    StartPipelineReprocessingResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
     BatchPutMessageRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    CreateDatasetContentResponseTypeDef,
+    CreatePipelineResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RunPipelineActivityResponseTypeDef,
+    SampleChannelDataResponseTypeDef,
+    StartPipelineReprocessingResponseTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageOutputTypeDef,
-    ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
+    ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
-    DatasetTriggerOutputTypeDef,
     DatasetTriggerTypeDef,
-    DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
-    DatastorePartitionOutputTypeDef,
     DatastorePartitionTypeDef,
-    QueryFilterOutputTypeDef,
-    LateDataRuleConfigurationOutputTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    S3DestinationConfigurationOutputTypeDef,
-    S3DestinationConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    VariableOutputTypeDef,
+    S3DestinationConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     VariableTypeDef,
     PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
     ChannelTypeDef,
-    ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ChannelSummaryTypeDef,
     ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
-    DatastoreStorageOutputTypeDef,
     DatastoreStorageSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
     DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
-    SqlQueryDatasetActionOutputTypeDef,
-    LateDataRuleOutputTypeDef,
     LateDataRuleTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
-    DatasetContentDeliveryDestinationOutputTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
     ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
     PipelineTypeDef,
     CreatePipelineRequestRequestTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ListChannelsResponseTypeDef,
     FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
     DatastoreSummaryTypeDef,
-    DatasetContentDeliveryRuleOutputTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
     DatastoreTypeDef,
     CreateDatastoreRequestRequestTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/SOURCES.txt` & `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.12/setup.py` & `mypy-boto3-iotanalytics-1.28.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotanalytics",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTAnalytics 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

