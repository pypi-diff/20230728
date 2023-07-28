# Comparing `tmp/mypy-boto3-kinesis-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesis-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-kinesis-1.28.12.tar` & `mypy-boto3-kinesis-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32120 2023-07-27 05:24:40.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32059 2023-07-27 05:24:40.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.453339 mypy-boto3-kinesis-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-07-28 20:43:05.449339 mypy-boto3-kinesis-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.449339 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31886 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31825 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-28 20:29:10.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.449339 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.453339 mypy-boto3-kinesis-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:29:09.000000 mypy-boto3-kinesis-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesis-1.28.12/LICENSE` & `mypy-boto3-kinesis-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/PKG-INFO` & `mypy-boto3-kinesis-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.28.12
-Summary: Type annotations for boto3.Kinesis 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Kinesis 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,86 +371,85 @@
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeStreamConsumerInputRequestTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeStreamInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
-    EnhancedMonitoringOutputTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
     ShardFilterTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamConsumersInputRequestTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutRecordInputRequestTypeDef,
-    PutRecordOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
-    StreamModeDetailsOutputTypeDef,
     UpdateShardCountInputRequestTypeDef,
-    UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
+    CreateStreamInputRequestTypeDef,
+    StreamSummaryTypeDef,
+    UpdateStreamModeInputRequestTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnhancedMonitoringOutputTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
+    PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
-    CreateStreamInputRequestTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
+    UpdateShardCountOutputTypeDef,
+    DescribeStreamInputDescribeStreamPaginateTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    ListStreamsInputListStreamsPaginateTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
+    StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
     SubscribeToShardInputRequestTypeDef,
-    StreamDescriptionSummaryTypeDef,
-    StreamSummaryTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
+    ListStreamsOutputTypeDef,
+    DescribeStreamSummaryOutputTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
-    ListStreamsOutputTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
 def get_structure() -> AddTagsToStreamInputRequestTypeDef:
```

### Comparing `mypy-boto3-kinesis-1.28.12/README.md` & `mypy-boto3-kinesis-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,86 +339,85 @@
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeStreamConsumerInputRequestTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeStreamInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
-    EnhancedMonitoringOutputTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
     ShardFilterTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamConsumersInputRequestTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutRecordInputRequestTypeDef,
-    PutRecordOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
-    StreamModeDetailsOutputTypeDef,
     UpdateShardCountInputRequestTypeDef,
-    UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
+    CreateStreamInputRequestTypeDef,
+    StreamSummaryTypeDef,
+    UpdateStreamModeInputRequestTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnhancedMonitoringOutputTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
+    PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
-    CreateStreamInputRequestTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
+    UpdateShardCountOutputTypeDef,
+    DescribeStreamInputDescribeStreamPaginateTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    ListStreamsInputListStreamsPaginateTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
+    StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
     SubscribeToShardInputRequestTypeDef,
-    StreamDescriptionSummaryTypeDef,
-    StreamSummaryTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
+    ListStreamsOutputTypeDef,
+    DescribeStreamSummaryOutputTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
-    ListStreamsOutputTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
 def get_structure() -> AddTagsToStreamInputRequestTypeDef:
```

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.pyi` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__main__.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kinesis 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Kinesis 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis\nOther"
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

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.pyi` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.pyi` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStreamOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#describestreampaginator)
         """
 
 
@@ -86,15 +86,15 @@
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
         StreamCreationTimestamp: Union[datetime, str] = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#listshardspaginator)
         """
 
 
@@ -105,31 +105,28 @@
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
         StreamCreationTimestamp: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
         """
 
 
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ExclusiveStartStreamName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExclusiveStartStreamName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.pyi` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStreamOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#describestreampaginator)
         """
 
 class ListShardsPaginator(Paginator):
@@ -82,15 +82,15 @@
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
         StreamCreationTimestamp: Union[datetime, str] = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#listshardspaginator)
         """
 
 class ListStreamConsumersPaginator(Paginator):
@@ -100,30 +100,27 @@
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
         StreamCreationTimestamp: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
         """
 
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ExclusiveStartStreamName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExclusiveStartStreamName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,86 +43,85 @@
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
     "DecreaseStreamRetentionPeriodInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "DeregisterStreamConsumerInputRequestTypeDef",
-    "DescribeLimitsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeStreamConsumerInputRequestTypeDef",
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeStreamSummaryInputRequestTypeDef",
     "DisableEnhancedMonitoringInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableEnhancedMonitoringInputRequestTypeDef",
     "EnhancedMetricsTypeDef",
-    "EnhancedMonitoringOutputTypeDef",
     "GetRecordsInputRequestTypeDef",
     "RecordTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IncreaseStreamRetentionPeriodInputRequestTypeDef",
     "InternalFailureExceptionTypeDef",
     "KMSAccessDeniedExceptionTypeDef",
     "KMSDisabledExceptionTypeDef",
     "KMSInvalidStateExceptionTypeDef",
     "KMSNotFoundExceptionTypeDef",
     "KMSOptInRequiredTypeDef",
     "KMSThrottlingExceptionTypeDef",
     "ShardFilterTypeDef",
-    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     "ListStreamConsumersInputRequestTypeDef",
-    "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "TagTypeDef",
     "MergeShardsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutRecordInputRequestTypeDef",
-    "PutRecordOutputTypeDef",
     "PutRecordsRequestEntryTypeDef",
     "PutRecordsResultEntryTypeDef",
     "RegisterStreamConsumerInputRequestTypeDef",
     "RemoveTagsFromStreamInputRequestTypeDef",
     "ResourceInUseExceptionTypeDef",
     "ResourceNotFoundExceptionTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
     "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
-    "StreamModeDetailsOutputTypeDef",
     "UpdateShardCountInputRequestTypeDef",
-    "UpdateShardCountOutputTypeDef",
     "ChildShardTypeDef",
+    "CreateStreamInputRequestTypeDef",
+    "StreamSummaryTypeDef",
+    "UpdateStreamModeInputRequestTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnhancedMonitoringOutputTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
+    "PutRecordOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
-    "CreateStreamInputRequestTypeDef",
-    "UpdateStreamModeInputRequestTypeDef",
+    "UpdateShardCountOutputTypeDef",
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
+    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    "ListStreamsInputListStreamsPaginateTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
+    "StreamDescriptionSummaryTypeDef",
     "ListShardsInputListShardsPaginateTypeDef",
     "ListShardsInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "PutRecordsInputRequestTypeDef",
     "PutRecordsOutputTypeDef",
     "ShardTypeDef",
     "SubscribeToShardInputRequestTypeDef",
-    "StreamDescriptionSummaryTypeDef",
-    "StreamSummaryTypeDef",
     "GetRecordsOutputTypeDef",
     "SubscribeToShardEventTypeDef",
+    "ListStreamsOutputTypeDef",
+    "DescribeStreamSummaryOutputTypeDef",
     "ListShardsOutputTypeDef",
     "StreamDescriptionTypeDef",
-    "DescribeStreamSummaryOutputTypeDef",
-    "ListStreamsOutputTypeDef",
     "SubscribeToShardEventStreamTypeDef",
     "DescribeStreamOutputTypeDef",
     "SubscribeToShardOutputTypeDef",
 )
 
 _RequiredAddTagsToStreamInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToStreamInputRequestTypeDef",
@@ -221,41 +220,41 @@
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ShardLimit": int,
-        "OpenShardCount": int,
-        "OnDemandStreamCount": int,
-        "OnDemandStreamCountLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeStreamConsumerInputRequestTypeDef = TypedDict(
     "DescribeStreamConsumerInputRequestTypeDef",
     {
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
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
 
 DescribeStreamInputRequestTypeDef = TypedDict(
     "DescribeStreamInputRequestTypeDef",
     {
@@ -304,21 +303,14 @@
 class DisableEnhancedMonitoringInputRequestTypeDef(
     _RequiredDisableEnhancedMonitoringInputRequestTypeDef,
     _OptionalDisableEnhancedMonitoringInputRequestTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
     "_RequiredEnableEnhancedMonitoringInputRequestTypeDef",
     {
         "ShardLevelMetrics": Sequence[MetricsNameType],
     },
 )
 _OptionalEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
@@ -342,25 +334,14 @@
     "EnhancedMetricsTypeDef",
     {
         "ShardLevelMetrics": List[MetricsNameType],
     },
     total=False,
 )
 
-EnhancedMonitoringOutputTypeDef = TypedDict(
-    "EnhancedMonitoringOutputTypeDef",
-    {
-        "StreamName": str,
-        "CurrentShardLevelMetrics": List[MetricsNameType],
-        "DesiredShardLevelMetrics": List[MetricsNameType],
-        "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -422,22 +403,14 @@
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
     "_RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef",
     {
         "RetentionPeriodHours": int,
     },
 )
 _OptionalIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
@@ -529,37 +502,14 @@
 )
 
 
 class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
     pass
 
 
-_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamCreationTimestamp": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
-    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
     "_RequiredListStreamConsumersInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
@@ -575,23 +525,14 @@
 
 class ListStreamConsumersInputRequestTypeDef(
     _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
 ):
     pass
 
 
-ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsInputListStreamsPaginateTypeDef",
-    {
-        "ExclusiveStartStreamName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "Limit": int,
         "ExclusiveStartStreamName": str,
         "NextToken": str,
     },
@@ -647,24 +588,14 @@
 
 class MergeShardsInputRequestTypeDef(
     _RequiredMergeShardsInputRequestTypeDef, _OptionalMergeShardsInputRequestTypeDef
 ):
     pass
 
 
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
 _RequiredPutRecordInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordInputRequestTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -682,24 +613,14 @@
 
 class PutRecordInputRequestTypeDef(
     _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
 ):
     pass
 
 
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
-    {
-        "ShardId": str,
-        "SequenceNumber": str,
-        "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutRecordsRequestEntryTypeDef = TypedDict(
     "_RequiredPutRecordsRequestEntryTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -772,25 +693,14 @@
     "ResourceNotFoundExceptionTypeDef",
     {
         "message": str,
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
 _RequiredSequenceNumberRangeTypeDef = TypedDict(
     "_RequiredSequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
     },
 )
 _OptionalSequenceNumberRangeTypeDef = TypedDict(
@@ -895,21 +805,14 @@
 class StopStreamEncryptionInputRequestTypeDef(
     _RequiredStopStreamEncryptionInputRequestTypeDef,
     _OptionalStopStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
 
-StreamModeDetailsOutputTypeDef = TypedDict(
-    "StreamModeDetailsOutputTypeDef",
-    {
-        "StreamMode": StreamModeType,
-    },
-)
-
 _RequiredUpdateShardCountInputRequestTypeDef = TypedDict(
     "_RequiredUpdateShardCountInputRequestTypeDef",
     {
         "TargetShardCount": int,
         "ScalingType": Literal["UNIFORM_SCALING"],
     },
 )
@@ -925,87 +828,198 @@
 
 class UpdateShardCountInputRequestTypeDef(
     _RequiredUpdateShardCountInputRequestTypeDef, _OptionalUpdateShardCountInputRequestTypeDef
 ):
     pass
 
 
-UpdateShardCountOutputTypeDef = TypedDict(
-    "UpdateShardCountOutputTypeDef",
+ChildShardTypeDef = TypedDict(
+    "ChildShardTypeDef",
+    {
+        "ShardId": str,
+        "ParentShards": List[str],
+        "HashKeyRange": HashKeyRangeTypeDef,
+    },
+)
+
+_RequiredCreateStreamInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamInputRequestTypeDef",
+    {
+        "StreamName": str,
+    },
+)
+_OptionalCreateStreamInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamInputRequestTypeDef",
+    {
+        "ShardCount": int,
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateStreamInputRequestTypeDef(
+    _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
+):
+    pass
+
+
+_RequiredStreamSummaryTypeDef = TypedDict(
+    "_RequiredStreamSummaryTypeDef",
     {
         "StreamName": str,
-        "CurrentShardCount": int,
-        "TargetShardCount": int,
         "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamStatus": StreamStatusType,
     },
 )
+_OptionalStreamSummaryTypeDef = TypedDict(
+    "_OptionalStreamSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "StreamCreationTimestamp": datetime,
+    },
+    total=False,
+)
 
-ChildShardTypeDef = TypedDict(
-    "ChildShardTypeDef",
+
+class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
+    pass
+
+
+UpdateStreamModeInputRequestTypeDef = TypedDict(
+    "UpdateStreamModeInputRequestTypeDef",
     {
-        "ShardId": str,
-        "ParentShards": List[str],
-        "HashKeyRange": HashKeyRangeTypeDef,
+        "StreamARN": str,
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+    },
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "ShardLimit": int,
+        "OpenShardCount": int,
+        "OnDemandStreamCount": int,
+        "OnDemandStreamCountLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStreamConsumerOutputTypeDef = TypedDict(
     "DescribeStreamConsumerOutputTypeDef",
     {
         "ConsumerDescription": ConsumerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+EnhancedMonitoringOutputTypeDef = TypedDict(
+    "EnhancedMonitoringOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardLevelMetrics": List[MetricsNameType],
+        "DesiredShardLevelMetrics": List[MetricsNameType],
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamConsumersOutputTypeDef = TypedDict(
     "ListStreamConsumersOutputTypeDef",
     {
         "Consumers": List[ConsumerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "ShardId": str,
+        "SequenceNumber": str,
+        "EncryptionType": EncryptionTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterStreamConsumerOutputTypeDef = TypedDict(
     "RegisterStreamConsumerOutputTypeDef",
     {
         "Consumer": ConsumerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStreamInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamInputRequestTypeDef",
+UpdateShardCountOutputTypeDef = TypedDict(
+    "UpdateShardCountOutputTypeDef",
     {
         "StreamName": str,
+        "CurrentShardCount": int,
+        "TargetShardCount": int,
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateStreamInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamInputRequestTypeDef",
+
+DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
     {
-        "ShardCount": int,
-        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamCreationTimestamp": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class CreateStreamInputRequestTypeDef(
-    _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
+
+class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
+    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
 ):
     pass
 
 
-UpdateStreamModeInputRequestTypeDef = TypedDict(
-    "UpdateStreamModeInputRequestTypeDef",
+ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsInputListStreamsPaginateTypeDef",
     {
-        "StreamARN": str,
-        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "ExclusiveStartStreamName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeStreamInputStreamExistsWaitTypeDef = TypedDict(
     "DescribeStreamInputStreamExistsWaitTypeDef",
     {
         "StreamName": str,
         "Limit": int,
@@ -1024,23 +1038,53 @@
         "ExclusiveStartShardId": str,
         "StreamARN": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
+    "_RequiredStreamDescriptionSummaryTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "StreamStatus": StreamStatusType,
+        "RetentionPeriodHours": int,
+        "StreamCreationTimestamp": datetime,
+        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
+        "OpenShardCount": int,
+    },
+)
+_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
+    "_OptionalStreamDescriptionSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "EncryptionType": EncryptionTypeType,
+        "KeyId": str,
+        "ConsumerCount": int,
+    },
+    total=False,
+)
+
+
+class StreamDescriptionSummaryTypeDef(
+    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
+):
+    pass
+
+
 ListShardsInputListShardsPaginateTypeDef = TypedDict(
     "ListShardsInputListShardsPaginateTypeDef",
     {
         "StreamName": str,
         "ExclusiveStartShardId": str,
         "StreamCreationTimestamp": Union[datetime, str],
         "ShardFilter": ShardFilterTypeDef,
         "StreamARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListShardsInputRequestTypeDef = TypedDict(
     "ListShardsInputRequestTypeDef",
     {
@@ -1056,15 +1100,15 @@
 )
 
 ListTagsForStreamOutputTypeDef = TypedDict(
     "ListTagsForStreamOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "HasMoreTags": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordsInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordsInputRequestTypeDef",
     {
         "Records": Sequence[PutRecordsRequestEntryTypeDef],
@@ -1088,15 +1132,15 @@
 
 PutRecordsOutputTypeDef = TypedDict(
     "PutRecordsOutputTypeDef",
     {
         "FailedRecordCount": int,
         "Records": List[PutRecordsResultEntryTypeDef],
         "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredShardTypeDef = TypedDict(
     "_RequiredShardTypeDef",
     {
         "ShardId": str,
@@ -1123,74 +1167,22 @@
     {
         "ConsumerARN": str,
         "ShardId": str,
         "StartingPosition": StartingPositionTypeDef,
     },
 )
 
-_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
-    "_RequiredStreamDescriptionSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-        "RetentionPeriodHours": int,
-        "StreamCreationTimestamp": datetime,
-        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
-        "OpenShardCount": int,
-    },
-)
-_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
-    "_OptionalStreamDescriptionSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
-        "EncryptionType": EncryptionTypeType,
-        "KeyId": str,
-        "ConsumerCount": int,
-    },
-    total=False,
-)
-
-
-class StreamDescriptionSummaryTypeDef(
-    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
-):
-    pass
-
-
-_RequiredStreamSummaryTypeDef = TypedDict(
-    "_RequiredStreamSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-    },
-)
-_OptionalStreamSummaryTypeDef = TypedDict(
-    "_OptionalStreamSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
-        "StreamCreationTimestamp": datetime,
-    },
-    total=False,
-)
-
-
-class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
-    pass
-
-
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubscribeToShardEventTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -1209,20 +1201,39 @@
 
 class SubscribeToShardEventTypeDef(
     _RequiredSubscribeToShardEventTypeDef, _OptionalSubscribeToShardEventTypeDef
 ):
     pass
 
 
+ListStreamsOutputTypeDef = TypedDict(
+    "ListStreamsOutputTypeDef",
+    {
+        "StreamNames": List[str],
+        "HasMoreStreams": bool,
+        "NextToken": str,
+        "StreamSummaries": List[StreamSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStreamSummaryOutputTypeDef = TypedDict(
+    "DescribeStreamSummaryOutputTypeDef",
+    {
+        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStreamDescriptionTypeDef = TypedDict(
     "_RequiredStreamDescriptionTypeDef",
     {
         "StreamName": str,
@@ -1234,47 +1245,28 @@
         "StreamCreationTimestamp": datetime,
         "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
     },
 )
 _OptionalStreamDescriptionTypeDef = TypedDict(
     "_OptionalStreamDescriptionTypeDef",
     {
-        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
+        "StreamModeDetails": StreamModeDetailsTypeDef,
         "EncryptionType": EncryptionTypeType,
         "KeyId": str,
     },
     total=False,
 )
 
 
 class StreamDescriptionTypeDef(
     _RequiredStreamDescriptionTypeDef, _OptionalStreamDescriptionTypeDef
 ):
     pass
 
 
-DescribeStreamSummaryOutputTypeDef = TypedDict(
-    "DescribeStreamSummaryOutputTypeDef",
-    {
-        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListStreamsOutputTypeDef = TypedDict(
-    "ListStreamsOutputTypeDef",
-    {
-        "StreamNames": List[str],
-        "HasMoreStreams": bool,
-        "NextToken": str,
-        "StreamSummaries": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSubscribeToShardEventStreamTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventStreamTypeDef",
     {
         "SubscribeToShardEvent": SubscribeToShardEventTypeDef,
     },
 )
 _OptionalSubscribeToShardEventStreamTypeDef = TypedDict(
@@ -1300,18 +1292,18 @@
     pass
 
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscribeToShardOutputTypeDef = TypedDict(
     "SubscribeToShardOutputTypeDef",
     {
         "EventStream": "EventStream[SubscribeToShardEventStreamTypeDef]",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.pyi` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -42,86 +42,85 @@
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
     "DecreaseStreamRetentionPeriodInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "DeregisterStreamConsumerInputRequestTypeDef",
-    "DescribeLimitsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeStreamConsumerInputRequestTypeDef",
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeStreamSummaryInputRequestTypeDef",
     "DisableEnhancedMonitoringInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableEnhancedMonitoringInputRequestTypeDef",
     "EnhancedMetricsTypeDef",
-    "EnhancedMonitoringOutputTypeDef",
     "GetRecordsInputRequestTypeDef",
     "RecordTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IncreaseStreamRetentionPeriodInputRequestTypeDef",
     "InternalFailureExceptionTypeDef",
     "KMSAccessDeniedExceptionTypeDef",
     "KMSDisabledExceptionTypeDef",
     "KMSInvalidStateExceptionTypeDef",
     "KMSNotFoundExceptionTypeDef",
     "KMSOptInRequiredTypeDef",
     "KMSThrottlingExceptionTypeDef",
     "ShardFilterTypeDef",
-    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     "ListStreamConsumersInputRequestTypeDef",
-    "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "TagTypeDef",
     "MergeShardsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutRecordInputRequestTypeDef",
-    "PutRecordOutputTypeDef",
     "PutRecordsRequestEntryTypeDef",
     "PutRecordsResultEntryTypeDef",
     "RegisterStreamConsumerInputRequestTypeDef",
     "RemoveTagsFromStreamInputRequestTypeDef",
     "ResourceInUseExceptionTypeDef",
     "ResourceNotFoundExceptionTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
     "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
-    "StreamModeDetailsOutputTypeDef",
     "UpdateShardCountInputRequestTypeDef",
-    "UpdateShardCountOutputTypeDef",
     "ChildShardTypeDef",
+    "CreateStreamInputRequestTypeDef",
+    "StreamSummaryTypeDef",
+    "UpdateStreamModeInputRequestTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnhancedMonitoringOutputTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
+    "PutRecordOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
-    "CreateStreamInputRequestTypeDef",
-    "UpdateStreamModeInputRequestTypeDef",
+    "UpdateShardCountOutputTypeDef",
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
+    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    "ListStreamsInputListStreamsPaginateTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
+    "StreamDescriptionSummaryTypeDef",
     "ListShardsInputListShardsPaginateTypeDef",
     "ListShardsInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "PutRecordsInputRequestTypeDef",
     "PutRecordsOutputTypeDef",
     "ShardTypeDef",
     "SubscribeToShardInputRequestTypeDef",
-    "StreamDescriptionSummaryTypeDef",
-    "StreamSummaryTypeDef",
     "GetRecordsOutputTypeDef",
     "SubscribeToShardEventTypeDef",
+    "ListStreamsOutputTypeDef",
+    "DescribeStreamSummaryOutputTypeDef",
     "ListShardsOutputTypeDef",
     "StreamDescriptionTypeDef",
-    "DescribeStreamSummaryOutputTypeDef",
-    "ListStreamsOutputTypeDef",
     "SubscribeToShardEventStreamTypeDef",
     "DescribeStreamOutputTypeDef",
     "SubscribeToShardOutputTypeDef",
 )
 
 _RequiredAddTagsToStreamInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToStreamInputRequestTypeDef",
@@ -216,41 +215,41 @@
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ShardLimit": int,
-        "OpenShardCount": int,
-        "OnDemandStreamCount": int,
-        "OnDemandStreamCountLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeStreamConsumerInputRequestTypeDef = TypedDict(
     "DescribeStreamConsumerInputRequestTypeDef",
     {
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
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
 
 DescribeStreamInputRequestTypeDef = TypedDict(
     "DescribeStreamInputRequestTypeDef",
     {
@@ -297,21 +296,14 @@
 
 class DisableEnhancedMonitoringInputRequestTypeDef(
     _RequiredDisableEnhancedMonitoringInputRequestTypeDef,
     _OptionalDisableEnhancedMonitoringInputRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
     "_RequiredEnableEnhancedMonitoringInputRequestTypeDef",
     {
         "ShardLevelMetrics": Sequence[MetricsNameType],
     },
 )
 _OptionalEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
@@ -333,25 +325,14 @@
     "EnhancedMetricsTypeDef",
     {
         "ShardLevelMetrics": List[MetricsNameType],
     },
     total=False,
 )
 
-EnhancedMonitoringOutputTypeDef = TypedDict(
-    "EnhancedMonitoringOutputTypeDef",
-    {
-        "StreamName": str,
-        "CurrentShardLevelMetrics": List[MetricsNameType],
-        "DesiredShardLevelMetrics": List[MetricsNameType],
-        "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -407,22 +388,14 @@
 )
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
     "_RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef",
     {
         "RetentionPeriodHours": int,
     },
 )
 _OptionalIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
@@ -510,35 +483,14 @@
     },
     total=False,
 )
 
 class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
     pass
 
-_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamCreationTimestamp": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
-    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-):
-    pass
-
 _RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
     "_RequiredListStreamConsumersInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
@@ -552,23 +504,14 @@
 )
 
 class ListStreamConsumersInputRequestTypeDef(
     _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
 ):
     pass
 
-ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsInputListStreamsPaginateTypeDef",
-    {
-        "ExclusiveStartStreamName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "Limit": int,
         "ExclusiveStartStreamName": str,
         "NextToken": str,
     },
@@ -620,24 +563,14 @@
 )
 
 class MergeShardsInputRequestTypeDef(
     _RequiredMergeShardsInputRequestTypeDef, _OptionalMergeShardsInputRequestTypeDef
 ):
     pass
 
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
 _RequiredPutRecordInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordInputRequestTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -653,24 +586,14 @@
 )
 
 class PutRecordInputRequestTypeDef(
     _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
 ):
     pass
 
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
-    {
-        "ShardId": str,
-        "SequenceNumber": str,
-        "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutRecordsRequestEntryTypeDef = TypedDict(
     "_RequiredPutRecordsRequestEntryTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -739,25 +662,14 @@
     "ResourceNotFoundExceptionTypeDef",
     {
         "message": str,
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
 _RequiredSequenceNumberRangeTypeDef = TypedDict(
     "_RequiredSequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
     },
 )
 _OptionalSequenceNumberRangeTypeDef = TypedDict(
@@ -852,21 +764,14 @@
 
 class StopStreamEncryptionInputRequestTypeDef(
     _RequiredStopStreamEncryptionInputRequestTypeDef,
     _OptionalStopStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
-StreamModeDetailsOutputTypeDef = TypedDict(
-    "StreamModeDetailsOutputTypeDef",
-    {
-        "StreamMode": StreamModeType,
-    },
-)
-
 _RequiredUpdateShardCountInputRequestTypeDef = TypedDict(
     "_RequiredUpdateShardCountInputRequestTypeDef",
     {
         "TargetShardCount": int,
         "ScalingType": Literal["UNIFORM_SCALING"],
     },
 )
@@ -880,85 +785,192 @@
 )
 
 class UpdateShardCountInputRequestTypeDef(
     _RequiredUpdateShardCountInputRequestTypeDef, _OptionalUpdateShardCountInputRequestTypeDef
 ):
     pass
 
-UpdateShardCountOutputTypeDef = TypedDict(
-    "UpdateShardCountOutputTypeDef",
+ChildShardTypeDef = TypedDict(
+    "ChildShardTypeDef",
+    {
+        "ShardId": str,
+        "ParentShards": List[str],
+        "HashKeyRange": HashKeyRangeTypeDef,
+    },
+)
+
+_RequiredCreateStreamInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamInputRequestTypeDef",
+    {
+        "StreamName": str,
+    },
+)
+_OptionalCreateStreamInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamInputRequestTypeDef",
+    {
+        "ShardCount": int,
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+    },
+    total=False,
+)
+
+class CreateStreamInputRequestTypeDef(
+    _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
+):
+    pass
+
+_RequiredStreamSummaryTypeDef = TypedDict(
+    "_RequiredStreamSummaryTypeDef",
     {
         "StreamName": str,
-        "CurrentShardCount": int,
-        "TargetShardCount": int,
         "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamStatus": StreamStatusType,
+    },
+)
+_OptionalStreamSummaryTypeDef = TypedDict(
+    "_OptionalStreamSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "StreamCreationTimestamp": datetime,
     },
+    total=False,
 )
 
-ChildShardTypeDef = TypedDict(
-    "ChildShardTypeDef",
+class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
+    pass
+
+UpdateStreamModeInputRequestTypeDef = TypedDict(
+    "UpdateStreamModeInputRequestTypeDef",
     {
-        "ShardId": str,
-        "ParentShards": List[str],
-        "HashKeyRange": HashKeyRangeTypeDef,
+        "StreamARN": str,
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+    },
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "ShardLimit": int,
+        "OpenShardCount": int,
+        "OnDemandStreamCount": int,
+        "OnDemandStreamCountLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStreamConsumerOutputTypeDef = TypedDict(
     "DescribeStreamConsumerOutputTypeDef",
     {
         "ConsumerDescription": ConsumerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+EnhancedMonitoringOutputTypeDef = TypedDict(
+    "EnhancedMonitoringOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardLevelMetrics": List[MetricsNameType],
+        "DesiredShardLevelMetrics": List[MetricsNameType],
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamConsumersOutputTypeDef = TypedDict(
     "ListStreamConsumersOutputTypeDef",
     {
         "Consumers": List[ConsumerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "ShardId": str,
+        "SequenceNumber": str,
+        "EncryptionType": EncryptionTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterStreamConsumerOutputTypeDef = TypedDict(
     "RegisterStreamConsumerOutputTypeDef",
     {
         "Consumer": ConsumerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStreamInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamInputRequestTypeDef",
+UpdateShardCountOutputTypeDef = TypedDict(
+    "UpdateShardCountOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardCount": int,
+        "TargetShardCount": int,
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
     {
         "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateStreamInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamInputRequestTypeDef",
+
+_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     {
-        "ShardCount": int,
-        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamCreationTimestamp": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateStreamInputRequestTypeDef(
-    _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
+class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
+    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
 ):
     pass
 
-UpdateStreamModeInputRequestTypeDef = TypedDict(
-    "UpdateStreamModeInputRequestTypeDef",
+ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsInputListStreamsPaginateTypeDef",
     {
-        "StreamARN": str,
-        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "ExclusiveStartStreamName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeStreamInputStreamExistsWaitTypeDef = TypedDict(
     "DescribeStreamInputStreamExistsWaitTypeDef",
     {
         "StreamName": str,
         "Limit": int,
@@ -977,23 +989,51 @@
         "ExclusiveStartShardId": str,
         "StreamARN": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
+    "_RequiredStreamDescriptionSummaryTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "StreamStatus": StreamStatusType,
+        "RetentionPeriodHours": int,
+        "StreamCreationTimestamp": datetime,
+        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
+        "OpenShardCount": int,
+    },
+)
+_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
+    "_OptionalStreamDescriptionSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "EncryptionType": EncryptionTypeType,
+        "KeyId": str,
+        "ConsumerCount": int,
+    },
+    total=False,
+)
+
+class StreamDescriptionSummaryTypeDef(
+    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
+):
+    pass
+
 ListShardsInputListShardsPaginateTypeDef = TypedDict(
     "ListShardsInputListShardsPaginateTypeDef",
     {
         "StreamName": str,
         "ExclusiveStartShardId": str,
         "StreamCreationTimestamp": Union[datetime, str],
         "ShardFilter": ShardFilterTypeDef,
         "StreamARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListShardsInputRequestTypeDef = TypedDict(
     "ListShardsInputRequestTypeDef",
     {
@@ -1009,15 +1049,15 @@
 )
 
 ListTagsForStreamOutputTypeDef = TypedDict(
     "ListTagsForStreamOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "HasMoreTags": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordsInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordsInputRequestTypeDef",
     {
         "Records": Sequence[PutRecordsRequestEntryTypeDef],
@@ -1039,15 +1079,15 @@
 
 PutRecordsOutputTypeDef = TypedDict(
     "PutRecordsOutputTypeDef",
     {
         "FailedRecordCount": int,
         "Records": List[PutRecordsResultEntryTypeDef],
         "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredShardTypeDef = TypedDict(
     "_RequiredShardTypeDef",
     {
         "ShardId": str,
@@ -1072,70 +1112,22 @@
     {
         "ConsumerARN": str,
         "ShardId": str,
         "StartingPosition": StartingPositionTypeDef,
     },
 )
 
-_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
-    "_RequiredStreamDescriptionSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-        "RetentionPeriodHours": int,
-        "StreamCreationTimestamp": datetime,
-        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
-        "OpenShardCount": int,
-    },
-)
-_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
-    "_OptionalStreamDescriptionSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
-        "EncryptionType": EncryptionTypeType,
-        "KeyId": str,
-        "ConsumerCount": int,
-    },
-    total=False,
-)
-
-class StreamDescriptionSummaryTypeDef(
-    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
-):
-    pass
-
-_RequiredStreamSummaryTypeDef = TypedDict(
-    "_RequiredStreamSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-    },
-)
-_OptionalStreamSummaryTypeDef = TypedDict(
-    "_OptionalStreamSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
-        "StreamCreationTimestamp": datetime,
-    },
-    total=False,
-)
-
-class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
-    pass
-
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubscribeToShardEventTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -1152,20 +1144,39 @@
 )
 
 class SubscribeToShardEventTypeDef(
     _RequiredSubscribeToShardEventTypeDef, _OptionalSubscribeToShardEventTypeDef
 ):
     pass
 
+ListStreamsOutputTypeDef = TypedDict(
+    "ListStreamsOutputTypeDef",
+    {
+        "StreamNames": List[str],
+        "HasMoreStreams": bool,
+        "NextToken": str,
+        "StreamSummaries": List[StreamSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStreamSummaryOutputTypeDef = TypedDict(
+    "DescribeStreamSummaryOutputTypeDef",
+    {
+        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStreamDescriptionTypeDef = TypedDict(
     "_RequiredStreamDescriptionTypeDef",
     {
         "StreamName": str,
@@ -1177,45 +1188,26 @@
         "StreamCreationTimestamp": datetime,
         "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
     },
 )
 _OptionalStreamDescriptionTypeDef = TypedDict(
     "_OptionalStreamDescriptionTypeDef",
     {
-        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
+        "StreamModeDetails": StreamModeDetailsTypeDef,
         "EncryptionType": EncryptionTypeType,
         "KeyId": str,
     },
     total=False,
 )
 
 class StreamDescriptionTypeDef(
     _RequiredStreamDescriptionTypeDef, _OptionalStreamDescriptionTypeDef
 ):
     pass
 
-DescribeStreamSummaryOutputTypeDef = TypedDict(
-    "DescribeStreamSummaryOutputTypeDef",
-    {
-        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListStreamsOutputTypeDef = TypedDict(
-    "ListStreamsOutputTypeDef",
-    {
-        "StreamNames": List[str],
-        "HasMoreStreams": bool,
-        "NextToken": str,
-        "StreamSummaries": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSubscribeToShardEventStreamTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventStreamTypeDef",
     {
         "SubscribeToShardEvent": SubscribeToShardEventTypeDef,
     },
 )
 _OptionalSubscribeToShardEventStreamTypeDef = TypedDict(
@@ -1239,18 +1231,18 @@
 ):
     pass
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscribeToShardOutputTypeDef = TypedDict(
     "SubscribeToShardOutputTypeDef",
     {
         "EventStream": "EventStream[SubscribeToShardEventStreamTypeDef]",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.py` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.pyi` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/PKG-INFO` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.28.12
-Summary: Type annotations for boto3.Kinesis 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Kinesis 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,86 +371,85 @@
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeStreamConsumerInputRequestTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeStreamInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
-    EnhancedMonitoringOutputTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
     ShardFilterTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamConsumersInputRequestTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutRecordInputRequestTypeDef,
-    PutRecordOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
-    StreamModeDetailsOutputTypeDef,
     UpdateShardCountInputRequestTypeDef,
-    UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
+    CreateStreamInputRequestTypeDef,
+    StreamSummaryTypeDef,
+    UpdateStreamModeInputRequestTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnhancedMonitoringOutputTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
+    PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
-    CreateStreamInputRequestTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
+    UpdateShardCountOutputTypeDef,
+    DescribeStreamInputDescribeStreamPaginateTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    ListStreamsInputListStreamsPaginateTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
+    StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
     SubscribeToShardInputRequestTypeDef,
-    StreamDescriptionSummaryTypeDef,
-    StreamSummaryTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
+    ListStreamsOutputTypeDef,
+    DescribeStreamSummaryOutputTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
-    ListStreamsOutputTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
 def get_structure() -> AddTagsToStreamInputRequestTypeDef:
```

### Comparing `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-1.28.15/mypy_boto3_kinesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.12/setup.py` & `mypy-boto3-kinesis-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kinesis 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Kinesis 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

