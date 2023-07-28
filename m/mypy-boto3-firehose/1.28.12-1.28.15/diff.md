# Comparing `tmp/mypy-boto3-firehose-1.28.12.tar.gz` & `tmp/mypy-boto3-firehose-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-firehose-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-firehose-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
```

## Comparing `mypy-boto3-firehose-1.28.12.tar` & `mypy-boto3-firehose-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.012509 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-07-27 05:22:19.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54181 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.445119 mypy-boto3-firehose-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-28 20:42:49.445119 mypy-boto3-firehose-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.441119 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-28 20:25:53.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48382 2023-07-28 20:25:55.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-07-28 20:25:54.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.445119 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-28 20:42:49.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 20:42:49.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:49.000000 mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.445119 mypy-boto3-firehose-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:25:52.000000 mypy-boto3-firehose-1.28.15/setup.py
```

### Comparing `mypy-boto3-firehose-1.28.12/LICENSE` & `mypy-boto3-firehose-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.12/PKG-INFO` & `mypy-boto3-firehose-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-firehose
-Version: 1.28.12
-Summary: Type annotations for boto3.Firehose 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 firehose type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,104 +287,82 @@
 ### Typed dictionaries
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
-    AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
-    AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
-    CloudWatchLoggingOptionsOutputTypeDef,
     VpcConfigurationDescriptionTypeDef,
-    AmazonopensearchserviceBufferingHintsOutputTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
-    AmazonopensearchserviceRetryOptionsOutputTypeDef,
-    BufferingHintsOutputTypeDef,
     BufferingHintsTypeDef,
-    CopyCommandOutputTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    SchemaConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
     HiveJsonSerDeOutputTypeDef,
     OpenXJsonSerDeOutputTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
-    RetryOptionsOutputTypeDef,
     RetryOptionsTypeDef,
-    ElasticsearchBufferingHintsOutputTypeDef,
     ElasticsearchBufferingHintsTypeDef,
     ElasticsearchRetryOptionsTypeDef,
-    ElasticsearchRetryOptionsOutputTypeDef,
-    KMSEncryptionConfigOutputTypeDef,
     KMSEncryptionConfigTypeDef,
-    HttpEndpointBufferingHintsOutputTypeDef,
     HttpEndpointBufferingHintsTypeDef,
-    HttpEndpointCommonAttributeOutputTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
-    HttpEndpointRetryOptionsOutputTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
-    TagOutputTypeDef,
     OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
-    ParquetSerDeOutputTypeDef,
     ParquetSerDeTypeDef,
-    ProcessorParameterOutputTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
-    PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
-    RedshiftRetryOptionsOutputTypeDef,
-    ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
-    SplunkRetryOptionsOutputTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    PutRecordOutputTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
     DeserializerOutputTypeDef,
     DeserializerTypeDef,
-    DynamicPartitioningConfigurationOutputTypeDef,
     DynamicPartitioningConfigurationTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
     SerializerOutputTypeDef,
     SerializerTypeDef,
     ProcessorOutputTypeDef,
     ProcessorTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
     PutRecordBatchOutputTypeDef,
     InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
-    S3DestinationDescriptionTypeDef,
     S3DestinationConfigurationTypeDef,
+    S3DestinationDescriptionTypeDef,
     S3DestinationUpdateTypeDef,
     OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
     ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     DataFormatConversionConfigurationOutputTypeDef,
     DataFormatConversionConfigurationTypeDef,
@@ -445,15 +391,15 @@
     CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsOutputTypeDef:
+def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.12/README.md` & `mypy-boto3-firehose-1.28.15/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-firehose
+Version: 1.28.15
+Summary: Type annotations for boto3.Firehose 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 firehose type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,104 +319,82 @@
 ### Typed dictionaries
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
-    AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
-    AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
-    CloudWatchLoggingOptionsOutputTypeDef,
     VpcConfigurationDescriptionTypeDef,
-    AmazonopensearchserviceBufferingHintsOutputTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
-    AmazonopensearchserviceRetryOptionsOutputTypeDef,
-    BufferingHintsOutputTypeDef,
     BufferingHintsTypeDef,
-    CopyCommandOutputTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    SchemaConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
     HiveJsonSerDeOutputTypeDef,
     OpenXJsonSerDeOutputTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
-    RetryOptionsOutputTypeDef,
     RetryOptionsTypeDef,
-    ElasticsearchBufferingHintsOutputTypeDef,
     ElasticsearchBufferingHintsTypeDef,
     ElasticsearchRetryOptionsTypeDef,
-    ElasticsearchRetryOptionsOutputTypeDef,
-    KMSEncryptionConfigOutputTypeDef,
     KMSEncryptionConfigTypeDef,
-    HttpEndpointBufferingHintsOutputTypeDef,
     HttpEndpointBufferingHintsTypeDef,
-    HttpEndpointCommonAttributeOutputTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
-    HttpEndpointRetryOptionsOutputTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
-    TagOutputTypeDef,
     OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
-    ParquetSerDeOutputTypeDef,
     ParquetSerDeTypeDef,
-    ProcessorParameterOutputTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
-    PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
-    RedshiftRetryOptionsOutputTypeDef,
-    ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
-    SplunkRetryOptionsOutputTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    PutRecordOutputTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
     DeserializerOutputTypeDef,
     DeserializerTypeDef,
-    DynamicPartitioningConfigurationOutputTypeDef,
     DynamicPartitioningConfigurationTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
     SerializerOutputTypeDef,
     SerializerTypeDef,
     ProcessorOutputTypeDef,
     ProcessorTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
     PutRecordBatchOutputTypeDef,
     InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
-    S3DestinationDescriptionTypeDef,
     S3DestinationConfigurationTypeDef,
+    S3DestinationDescriptionTypeDef,
     S3DestinationUpdateTypeDef,
     OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
     ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     DataFormatConversionConfigurationOutputTypeDef,
     DataFormatConversionConfigurationTypeDef,
@@ -413,15 +423,15 @@
     CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsOutputTypeDef:
+def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__main__.py` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Firehose 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Firehose 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.py` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.pyi` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.py` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.pyi` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.py` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for firehose service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsOutputTypeDef
+    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsTypeDef
 
-    data: AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = {...}
+    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -48,106 +48,83 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
-    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
-    "CloudWatchLoggingOptionsOutputTypeDef",
     "VpcConfigurationDescriptionTypeDef",
-    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
-    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
-    "BufferingHintsOutputTypeDef",
     "BufferingHintsTypeDef",
-    "CopyCommandOutputTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
-    "CreateDeliveryStreamOutputTypeDef",
-    "SchemaConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
     "HiveJsonSerDeOutputTypeDef",
     "OpenXJsonSerDeOutputTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
-    "RetryOptionsOutputTypeDef",
     "RetryOptionsTypeDef",
-    "ElasticsearchBufferingHintsOutputTypeDef",
     "ElasticsearchBufferingHintsTypeDef",
     "ElasticsearchRetryOptionsTypeDef",
-    "ElasticsearchRetryOptionsOutputTypeDef",
-    "KMSEncryptionConfigOutputTypeDef",
     "KMSEncryptionConfigTypeDef",
-    "HttpEndpointBufferingHintsOutputTypeDef",
     "HttpEndpointBufferingHintsTypeDef",
-    "HttpEndpointCommonAttributeOutputTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
-    "HttpEndpointRetryOptionsOutputTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
-    "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
-    "TagOutputTypeDef",
     "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
-    "ParquetSerDeOutputTypeDef",
     "ParquetSerDeTypeDef",
-    "ProcessorParameterOutputTypeDef",
     "ProcessorParameterTypeDef",
     "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
-    "PutRecordOutputTypeDef",
     "RedshiftRetryOptionsTypeDef",
-    "RedshiftRetryOptionsOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SplunkRetryOptionsTypeDef",
-    "SplunkRetryOptionsOutputTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
+    "CreateDeliveryStreamOutputTypeDef",
+    "ListDeliveryStreamsOutputTypeDef",
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    "PutRecordOutputTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
     "DeserializerOutputTypeDef",
     "DeserializerTypeDef",
-    "DynamicPartitioningConfigurationOutputTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
-    "ListTagsForDeliveryStreamOutputTypeDef",
     "SerializerOutputTypeDef",
     "SerializerTypeDef",
     "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
     "PutRecordBatchOutputTypeDef",
     "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
-    "S3DestinationDescriptionTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "S3DestinationDescriptionTypeDef",
     "S3DestinationUpdateTypeDef",
     "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
     "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
     "DataFormatConversionConfigurationOutputTypeDef",
     "DataFormatConversionConfigurationTypeDef",
@@ -175,23 +152,14 @@
     "DestinationDescriptionTypeDef",
     "CreateDeliveryStreamInputRequestTypeDef",
     "UpdateDestinationInputRequestTypeDef",
     "DeliveryStreamDescriptionTypeDef",
     "DescribeDeliveryStreamOutputTypeDef",
 )
 
-AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
-    {
-        "IntervalInSeconds": int,
-        "SizeInMBs": int,
-    },
-    total=False,
-)
-
 AmazonOpenSearchServerlessBufferingHintsTypeDef = TypedDict(
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -220,51 +188,24 @@
     {
         "SubnetIds": Sequence[str],
         "RoleARN": str,
         "SecurityGroupIds": Sequence[str],
     },
 )
 
-AmazonOpenSearchServerlessRetryOptionsOutputTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
-CloudWatchLoggingOptionsOutputTypeDef = TypedDict(
-    "CloudWatchLoggingOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "LogGroupName": str,
-        "LogStreamName": str,
-    },
-    total=False,
-)
-
 VpcConfigurationDescriptionTypeDef = TypedDict(
     "VpcConfigurationDescriptionTypeDef",
     {
         "SubnetIds": List[str],
         "RoleARN": str,
         "SecurityGroupIds": List[str],
         "VpcId": str,
     },
 )
 
-AmazonopensearchserviceBufferingHintsOutputTypeDef = TypedDict(
-    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
-    {
-        "IntervalInSeconds": int,
-        "SizeInMBs": int,
-    },
-    total=False,
-)
-
 AmazonopensearchserviceBufferingHintsTypeDef = TypedDict(
     "AmazonopensearchserviceBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -274,62 +215,23 @@
     "AmazonopensearchserviceRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-AmazonopensearchserviceRetryOptionsOutputTypeDef = TypedDict(
-    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
-BufferingHintsOutputTypeDef = TypedDict(
-    "BufferingHintsOutputTypeDef",
-    {
-        "SizeInMBs": int,
-        "IntervalInSeconds": int,
-    },
-    total=False,
-)
-
 BufferingHintsTypeDef = TypedDict(
     "BufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
-_RequiredCopyCommandOutputTypeDef = TypedDict(
-    "_RequiredCopyCommandOutputTypeDef",
-    {
-        "DataTableName": str,
-    },
-)
-_OptionalCopyCommandOutputTypeDef = TypedDict(
-    "_OptionalCopyCommandOutputTypeDef",
-    {
-        "DataTableColumns": str,
-        "CopyOptions": str,
-    },
-    total=False,
-)
-
-
-class CopyCommandOutputTypeDef(
-    _RequiredCopyCommandOutputTypeDef, _OptionalCopyCommandOutputTypeDef
-):
-    pass
-
-
 _RequiredCopyCommandTypeDef = TypedDict(
     "_RequiredCopyCommandTypeDef",
     {
         "DataTableName": str,
     },
 )
 _OptionalCopyCommandTypeDef = TypedDict(
@@ -337,41 +239,37 @@
     {
         "DataTableColumns": str,
         "CopyOptions": str,
     },
     total=False,
 )
 
-
 class CopyCommandTypeDef(_RequiredCopyCommandTypeDef, _OptionalCopyCommandTypeDef):
     pass
 
-
 _RequiredDeliveryStreamEncryptionConfigurationInputTypeDef = TypedDict(
     "_RequiredDeliveryStreamEncryptionConfigurationInputTypeDef",
     {
         "KeyType": KeyTypeType,
     },
 )
 _OptionalDeliveryStreamEncryptionConfigurationInputTypeDef = TypedDict(
     "_OptionalDeliveryStreamEncryptionConfigurationInputTypeDef",
     {
         "KeyARN": str,
     },
     total=False,
 )
 
-
 class DeliveryStreamEncryptionConfigurationInputTypeDef(
     _RequiredDeliveryStreamEncryptionConfigurationInputTypeDef,
     _OptionalDeliveryStreamEncryptionConfigurationInputTypeDef,
 ):
     pass
 
-
 KinesisStreamSourceConfigurationTypeDef = TypedDict(
     "KinesisStreamSourceConfigurationTypeDef",
     {
         "KinesisStreamARN": str,
         "RoleARN": str,
     },
 )
@@ -386,38 +284,26 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
-CreateDeliveryStreamOutputTypeDef = TypedDict(
-    "CreateDeliveryStreamOutputTypeDef",
-    {
-        "DeliveryStreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SchemaConfigurationOutputTypeDef = TypedDict(
-    "SchemaConfigurationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RoleARN": str,
-        "CatalogId": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "Region": str,
-        "VersionId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 SchemaConfigurationTypeDef = TypedDict(
     "SchemaConfigurationTypeDef",
     {
         "RoleARN": str,
         "CatalogId": str,
@@ -439,22 +325,20 @@
     "_OptionalDeleteDeliveryStreamInputRequestTypeDef",
     {
         "AllowForceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteDeliveryStreamInputRequestTypeDef(
     _RequiredDeleteDeliveryStreamInputRequestTypeDef,
     _OptionalDeleteDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-
 FailureDescriptionTypeDef = TypedDict(
     "FailureDescriptionTypeDef",
     {
         "Type": DeliveryStreamFailureTypeType,
         "Details": str,
     },
 )
@@ -470,22 +354,20 @@
     {
         "Limit": int,
         "ExclusiveStartDestinationId": str,
     },
     total=False,
 )
 
-
 class DescribeDeliveryStreamInputRequestTypeDef(
     _RequiredDescribeDeliveryStreamInputRequestTypeDef,
     _OptionalDescribeDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-
 HiveJsonSerDeOutputTypeDef = TypedDict(
     "HiveJsonSerDeOutputTypeDef",
     {
         "TimestampFormats": List[str],
     },
     total=False,
 )
@@ -514,39 +396,22 @@
         "ConvertDotsInJsonKeysToUnderscores": bool,
         "CaseInsensitive": bool,
         "ColumnToJsonKeyMappings": Mapping[str, str],
     },
     total=False,
 )
 
-RetryOptionsOutputTypeDef = TypedDict(
-    "RetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
 RetryOptionsTypeDef = TypedDict(
     "RetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-ElasticsearchBufferingHintsOutputTypeDef = TypedDict(
-    "ElasticsearchBufferingHintsOutputTypeDef",
-    {
-        "IntervalInSeconds": int,
-        "SizeInMBs": int,
-    },
-    total=False,
-)
-
 ElasticsearchBufferingHintsTypeDef = TypedDict(
     "ElasticsearchBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -556,62 +421,30 @@
     "ElasticsearchRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-ElasticsearchRetryOptionsOutputTypeDef = TypedDict(
-    "ElasticsearchRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
-KMSEncryptionConfigOutputTypeDef = TypedDict(
-    "KMSEncryptionConfigOutputTypeDef",
-    {
-        "AWSKMSKeyARN": str,
-    },
-)
-
 KMSEncryptionConfigTypeDef = TypedDict(
     "KMSEncryptionConfigTypeDef",
     {
         "AWSKMSKeyARN": str,
     },
 )
 
-HttpEndpointBufferingHintsOutputTypeDef = TypedDict(
-    "HttpEndpointBufferingHintsOutputTypeDef",
-    {
-        "SizeInMBs": int,
-        "IntervalInSeconds": int,
-    },
-    total=False,
-)
-
 HttpEndpointBufferingHintsTypeDef = TypedDict(
     "HttpEndpointBufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
-HttpEndpointCommonAttributeOutputTypeDef = TypedDict(
-    "HttpEndpointCommonAttributeOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeValue": str,
-    },
-)
-
 HttpEndpointCommonAttributeTypeDef = TypedDict(
     "HttpEndpointCommonAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
 )
@@ -627,21 +460,19 @@
     {
         "Name": str,
         "AccessKey": str,
     },
     total=False,
 )
 
-
 class HttpEndpointConfigurationTypeDef(
     _RequiredHttpEndpointConfigurationTypeDef, _OptionalHttpEndpointConfigurationTypeDef
 ):
     pass
 
-
 HttpEndpointDescriptionTypeDef = TypedDict(
     "HttpEndpointDescriptionTypeDef",
     {
         "Url": str,
         "Name": str,
     },
     total=False,
@@ -651,22 +482,14 @@
     "HttpEndpointRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-HttpEndpointRetryOptionsOutputTypeDef = TypedDict(
-    "HttpEndpointRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
 KinesisStreamSourceDescriptionTypeDef = TypedDict(
     "KinesisStreamSourceDescriptionTypeDef",
     {
         "KinesisStreamARN": str,
         "RoleARN": str,
         "DeliveryStartTimestamp": datetime,
     },
@@ -679,23 +502,14 @@
         "Limit": int,
         "DeliveryStreamType": DeliveryStreamTypeType,
         "ExclusiveStartDeliveryStreamName": str,
     },
     total=False,
 )
 
-ListDeliveryStreamsOutputTypeDef = TypedDict(
-    "ListDeliveryStreamsOutputTypeDef",
-    {
-        "DeliveryStreamNames": List[str],
-        "HasMoreDeliveryStreams": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -703,41 +517,20 @@
     {
         "ExclusiveStartTagKey": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListTagsForDeliveryStreamInputRequestTypeDef(
     _RequiredListTagsForDeliveryStreamInputRequestTypeDef,
     _OptionalListTagsForDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-
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
 OrcSerDeOutputTypeDef = TypedDict(
     "OrcSerDeOutputTypeDef",
     {
         "StripeSizeBytes": int,
         "BlockSizeBytes": int,
         "RowIndexStride": int,
         "EnablePadding": bool,
@@ -764,48 +557,27 @@
         "BloomFilterFalsePositiveProbability": float,
         "DictionaryKeyThreshold": float,
         "FormatVersion": OrcFormatVersionType,
     },
     total=False,
 )
 
-ParquetSerDeOutputTypeDef = TypedDict(
-    "ParquetSerDeOutputTypeDef",
-    {
-        "BlockSizeBytes": int,
-        "PageSizeBytes": int,
-        "Compression": ParquetCompressionType,
-        "EnableDictionaryCompression": bool,
-        "MaxPaddingBytes": int,
-        "WriterVersion": ParquetWriterVersionType,
-    },
-    total=False,
-)
-
 ParquetSerDeTypeDef = TypedDict(
     "ParquetSerDeTypeDef",
     {
         "BlockSizeBytes": int,
         "PageSizeBytes": int,
         "Compression": ParquetCompressionType,
         "EnableDictionaryCompression": bool,
         "MaxPaddingBytes": int,
         "WriterVersion": ParquetWriterVersionType,
     },
     total=False,
 )
 
-ProcessorParameterOutputTypeDef = TypedDict(
-    "ProcessorParameterOutputTypeDef",
-    {
-        "ParameterName": ProcessorParameterNameType,
-        "ParameterValue": str,
-    },
-)
-
 ProcessorParameterTypeDef = TypedDict(
     "ProcessorParameterTypeDef",
     {
         "ParameterName": ProcessorParameterNameType,
         "ParameterValue": str,
     },
 )
@@ -823,66 +595,30 @@
         "RecordId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
-    {
-        "RecordId": str,
-        "Encrypted": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedshiftRetryOptionsTypeDef = TypedDict(
     "RedshiftRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-RedshiftRetryOptionsOutputTypeDef = TypedDict(
-    "RedshiftRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
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
 SplunkRetryOptionsTypeDef = TypedDict(
     "SplunkRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-SplunkRetryOptionsOutputTypeDef = TypedDict(
-    "SplunkRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
 StopDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 
@@ -906,30 +642,63 @@
         "DeliveryStreamEncryptionConfigurationInput": (
             DeliveryStreamEncryptionConfigurationInputTypeDef
         ),
     },
     total=False,
 )
 
-
 class StartDeliveryStreamEncryptionInputRequestTypeDef(
     _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef,
     _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
-
 TagDeliveryStreamInputRequestTypeDef = TypedDict(
     "TagDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateDeliveryStreamOutputTypeDef = TypedDict(
+    "CreateDeliveryStreamOutputTypeDef",
+    {
+        "DeliveryStreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeliveryStreamsOutputTypeDef = TypedDict(
+    "ListDeliveryStreamsOutputTypeDef",
+    {
+        "DeliveryStreamNames": List[str],
+        "HasMoreDeliveryStreams": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "HasMoreTags": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "RecordId": str,
+        "Encrypted": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeliveryStreamEncryptionConfigurationTypeDef = TypedDict(
     "DeliveryStreamEncryptionConfigurationTypeDef",
     {
         "KeyARN": str,
         "KeyType": KeyTypeType,
         "Status": DeliveryStreamEncryptionStatusType,
         "FailureDescription": FailureDescriptionTypeDef,
@@ -951,55 +720,37 @@
     {
         "OpenXJsonSerDe": OpenXJsonSerDeTypeDef,
         "HiveJsonSerDe": HiveJsonSerDeTypeDef,
     },
     total=False,
 )
 
-DynamicPartitioningConfigurationOutputTypeDef = TypedDict(
-    "DynamicPartitioningConfigurationOutputTypeDef",
-    {
-        "RetryOptions": RetryOptionsOutputTypeDef,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 DynamicPartitioningConfigurationTypeDef = TypedDict(
     "DynamicPartitioningConfigurationTypeDef",
     {
         "RetryOptions": RetryOptionsTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "NoEncryptionConfig": Literal["NoEncryption"],
-        "KMSEncryptionConfig": KMSEncryptionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "NoEncryptionConfig": Literal["NoEncryption"],
         "KMSEncryptionConfig": KMSEncryptionConfigTypeDef,
     },
     total=False,
 )
 
 HttpEndpointRequestConfigurationOutputTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationOutputTypeDef",
     {
         "ContentEncoding": ContentEncodingType,
-        "CommonAttributes": List[HttpEndpointCommonAttributeOutputTypeDef],
+        "CommonAttributes": List[HttpEndpointCommonAttributeTypeDef],
     },
     total=False,
 )
 
 HttpEndpointRequestConfigurationTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationTypeDef",
     {
@@ -1013,27 +764,18 @@
     "SourceDescriptionTypeDef",
     {
         "KinesisStreamSourceDescription": KinesisStreamSourceDescriptionTypeDef,
     },
     total=False,
 )
 
-ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
-    "ListTagsForDeliveryStreamOutputTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "HasMoreTags": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SerializerOutputTypeDef = TypedDict(
     "SerializerOutputTypeDef",
     {
-        "ParquetSerDe": ParquetSerDeOutputTypeDef,
+        "ParquetSerDe": ParquetSerDeTypeDef,
         "OrcSerDe": OrcSerDeOutputTypeDef,
     },
     total=False,
 )
 
 SerializerTypeDef = TypedDict(
     "SerializerTypeDef",
@@ -1049,43 +791,39 @@
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorOutputTypeDef = TypedDict(
     "_OptionalProcessorOutputTypeDef",
     {
-        "Parameters": List[ProcessorParameterOutputTypeDef],
+        "Parameters": List[ProcessorParameterTypeDef],
     },
     total=False,
 )
 
-
 class ProcessorOutputTypeDef(_RequiredProcessorOutputTypeDef, _OptionalProcessorOutputTypeDef):
     pass
 
-
 _RequiredProcessorTypeDef = TypedDict(
     "_RequiredProcessorTypeDef",
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorTypeDef = TypedDict(
     "_OptionalProcessorTypeDef",
     {
         "Parameters": Sequence[ProcessorParameterTypeDef],
     },
     total=False,
 )
 
-
 class ProcessorTypeDef(_RequiredProcessorTypeDef, _OptionalProcessorTypeDef):
     pass
 
-
 PutRecordBatchInputRequestTypeDef = TypedDict(
     "PutRecordBatchInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Records": Sequence[RecordTypeDef],
     },
 )
@@ -1100,15 +838,15 @@
 
 PutRecordBatchOutputTypeDef = TypedDict(
     "PutRecordBatchOutputTypeDef",
     {
         "FailedPutCount": int,
         "Encrypted": bool,
         "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputFormatConfigurationOutputTypeDef = TypedDict(
     "InputFormatConfigurationOutputTypeDef",
     {
         "Deserializer": DeserializerOutputTypeDef,
@@ -1120,68 +858,64 @@
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
     },
     total=False,
 )
 
-_RequiredS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredS3DestinationDescriptionTypeDef",
+_RequiredS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsOutputTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
-_OptionalS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalS3DestinationDescriptionTypeDef",
+_OptionalS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-
-class S3DestinationDescriptionTypeDef(
-    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
+class S3DestinationConfigurationTypeDef(
+    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
-
-_RequiredS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredS3DestinationConfigurationTypeDef",
+_RequiredS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalS3DestinationConfigurationTypeDef",
+_OptionalS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-
-class S3DestinationConfigurationTypeDef(
-    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
+class S3DestinationDescriptionTypeDef(
+    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
 ):
     pass
 
-
 S3DestinationUpdateTypeDef = TypedDict(
     "S3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
         "Prefix": str,
         "ErrorOutputPrefix": str,
@@ -1226,15 +960,15 @@
     },
     total=False,
 )
 
 DataFormatConversionConfigurationOutputTypeDef = TypedDict(
     "DataFormatConversionConfigurationOutputTypeDef",
     {
-        "SchemaConfiguration": SchemaConfigurationOutputTypeDef,
+        "SchemaConfiguration": SchemaConfigurationTypeDef,
         "InputFormatConfiguration": InputFormatConfigurationOutputTypeDef,
         "OutputFormatConfiguration": OutputFormatConfigurationOutputTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
@@ -1251,122 +985,120 @@
 
 AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
-        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
-        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
+        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
         "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
     },
     total=False,
 )
 
 AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
         "TypeName": str,
         "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
-        "BufferingHints": AmazonopensearchserviceBufferingHintsOutputTypeDef,
-        "RetryOptions": AmazonopensearchserviceRetryOptionsOutputTypeDef,
+        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
+        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
         "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
     },
     total=False,
 )
 
 ElasticsearchDestinationDescriptionTypeDef = TypedDict(
     "ElasticsearchDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
         "TypeName": str,
         "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
-        "BufferingHints": ElasticsearchBufferingHintsOutputTypeDef,
-        "RetryOptions": ElasticsearchRetryOptionsOutputTypeDef,
+        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
+        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
         "S3BackupMode": ElasticsearchS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
     },
     total=False,
 )
 
 HttpEndpointDestinationDescriptionTypeDef = TypedDict(
     "HttpEndpointDestinationDescriptionTypeDef",
     {
         "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
-        "BufferingHints": HttpEndpointBufferingHintsOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationOutputTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "RoleARN": str,
-        "RetryOptions": HttpEndpointRetryOptionsOutputTypeDef,
+        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
         "S3BackupMode": HttpEndpointS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
     },
     total=False,
 )
 
 _RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
     "_RequiredRedshiftDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
-        "CopyCommand": CopyCommandOutputTypeDef,
+        "CopyCommand": CopyCommandTypeDef,
         "Username": str,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
     },
 )
 _OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
     "_OptionalRedshiftDestinationDescriptionTypeDef",
     {
-        "RetryOptions": RedshiftRetryOptionsOutputTypeDef,
+        "RetryOptions": RedshiftRetryOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "S3BackupMode": RedshiftS3BackupModeType,
         "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftDestinationDescriptionTypeDef(
     _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
 ):
     pass
 
-
 SplunkDestinationDescriptionTypeDef = TypedDict(
     "SplunkDestinationDescriptionTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
-        "RetryOptions": SplunkRetryOptionsOutputTypeDef,
+        "RetryOptions": SplunkRetryOptionsTypeDef,
         "S3BackupMode": SplunkS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
 _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef = TypedDict(
     "_RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     {
@@ -1385,22 +1117,20 @@
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(
     _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     _OptionalAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
 ):
     pass
 
-
 AmazonOpenSearchServerlessDestinationUpdateTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
         "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
@@ -1433,22 +1163,20 @@
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class AmazonopensearchserviceDestinationConfigurationTypeDef(
     _RequiredAmazonopensearchserviceDestinationConfigurationTypeDef,
     _OptionalAmazonopensearchserviceDestinationConfigurationTypeDef,
 ):
     pass
 
-
 AmazonopensearchserviceDestinationUpdateTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1484,22 +1212,20 @@
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ElasticsearchDestinationConfigurationTypeDef(
     _RequiredElasticsearchDestinationConfigurationTypeDef,
     _OptionalElasticsearchDestinationConfigurationTypeDef,
 ):
     pass
 
-
 ElasticsearchDestinationUpdateTypeDef = TypedDict(
     "ElasticsearchDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1531,22 +1257,20 @@
         "RoleARN": str,
         "RetryOptions": HttpEndpointRetryOptionsTypeDef,
         "S3BackupMode": HttpEndpointS3BackupModeType,
     },
     total=False,
 )
 
-
 class HttpEndpointDestinationConfigurationTypeDef(
     _RequiredHttpEndpointDestinationConfigurationTypeDef,
     _OptionalHttpEndpointDestinationConfigurationTypeDef,
 ):
     pass
 
-
 HttpEndpointDestinationUpdateTypeDef = TypedDict(
     "HttpEndpointDestinationUpdateTypeDef",
     {
         "EndpointConfiguration": HttpEndpointConfigurationTypeDef,
         "BufferingHints": HttpEndpointBufferingHintsTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
@@ -1578,22 +1302,20 @@
         "S3BackupMode": RedshiftS3BackupModeType,
         "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftDestinationConfigurationTypeDef(
     _RequiredRedshiftDestinationConfigurationTypeDef,
     _OptionalRedshiftDestinationConfigurationTypeDef,
 ):
     pass
 
-
 RedshiftDestinationUpdateTypeDef = TypedDict(
     "RedshiftDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
         "CopyCommand": CopyCommandTypeDef,
         "Username": str,
@@ -1625,21 +1347,19 @@
         "S3BackupMode": SplunkS3BackupModeType,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class SplunkDestinationConfigurationTypeDef(
     _RequiredSplunkDestinationConfigurationTypeDef, _OptionalSplunkDestinationConfigurationTypeDef
 ):
     pass
 
-
 SplunkDestinationUpdateTypeDef = TypedDict(
     "SplunkDestinationUpdateTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
@@ -1653,42 +1373,40 @@
 )
 
 _RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
     "_RequiredExtendedS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsOutputTypeDef,
+        "BufferingHints": BufferingHintsTypeDef,
         "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
 _OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
     "_OptionalExtendedS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "S3BackupMode": S3BackupModeType,
         "S3BackupDescription": S3DestinationDescriptionTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationOutputTypeDef,
-        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationOutputTypeDef,
+        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ExtendedS3DestinationDescriptionTypeDef(
     _RequiredExtendedS3DestinationDescriptionTypeDef,
     _OptionalExtendedS3DestinationDescriptionTypeDef,
 ):
     pass
 
-
 _RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
     "_RequiredExtendedS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
     },
 )
@@ -1706,22 +1424,20 @@
         "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ExtendedS3DestinationConfigurationTypeDef(
     _RequiredExtendedS3DestinationConfigurationTypeDef,
     _OptionalExtendedS3DestinationConfigurationTypeDef,
 ):
     pass
 
-
 ExtendedS3DestinationUpdateTypeDef = TypedDict(
     "ExtendedS3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
         "Prefix": str,
         "ErrorOutputPrefix": str,
@@ -1759,21 +1475,19 @@
         "AmazonOpenSearchServerlessDestinationDescription": (
             AmazonOpenSearchServerlessDestinationDescriptionTypeDef
         ),
     },
     total=False,
 )
 
-
 class DestinationDescriptionTypeDef(
     _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
 ):
     pass
 
-
 _RequiredCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -1797,22 +1511,20 @@
         "AmazonOpenSearchServerlessDestinationConfiguration": (
             AmazonOpenSearchServerlessDestinationConfigurationTypeDef
         ),
     },
     total=False,
 )
 
-
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDestinationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "CurrentDeliveryStreamVersionId": str,
         "DestinationId": str,
     },
@@ -1830,21 +1542,19 @@
         "AmazonOpenSearchServerlessDestinationUpdate": (
             AmazonOpenSearchServerlessDestinationUpdateTypeDef
         ),
     },
     total=False,
 )
 
-
 class UpdateDestinationInputRequestTypeDef(
     _RequiredUpdateDestinationInputRequestTypeDef, _OptionalUpdateDestinationInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeliveryStreamDescriptionTypeDef = TypedDict(
     "_RequiredDeliveryStreamDescriptionTypeDef",
     {
         "DeliveryStreamName": str,
         "DeliveryStreamARN": str,
         "DeliveryStreamStatus": DeliveryStreamStatusType,
         "DeliveryStreamType": DeliveryStreamTypeType,
@@ -1861,21 +1571,19 @@
         "CreateTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Source": SourceDescriptionTypeDef,
     },
     total=False,
 )
 
-
 class DeliveryStreamDescriptionTypeDef(
     _RequiredDeliveryStreamDescriptionTypeDef, _OptionalDeliveryStreamDescriptionTypeDef
 ):
     pass
 
-
 DescribeDeliveryStreamOutputTypeDef = TypedDict(
     "DescribeDeliveryStreamOutputTypeDef",
     {
         "DeliveryStreamDescription": DeliveryStreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.pyi` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for firehose service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsOutputTypeDef
+    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsTypeDef
 
-    data: AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = {...}
+    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -48,105 +48,84 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
-    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
-    "CloudWatchLoggingOptionsOutputTypeDef",
     "VpcConfigurationDescriptionTypeDef",
-    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
-    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
-    "BufferingHintsOutputTypeDef",
     "BufferingHintsTypeDef",
-    "CopyCommandOutputTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
-    "CreateDeliveryStreamOutputTypeDef",
-    "SchemaConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
     "HiveJsonSerDeOutputTypeDef",
     "OpenXJsonSerDeOutputTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
-    "RetryOptionsOutputTypeDef",
     "RetryOptionsTypeDef",
-    "ElasticsearchBufferingHintsOutputTypeDef",
     "ElasticsearchBufferingHintsTypeDef",
     "ElasticsearchRetryOptionsTypeDef",
-    "ElasticsearchRetryOptionsOutputTypeDef",
-    "KMSEncryptionConfigOutputTypeDef",
     "KMSEncryptionConfigTypeDef",
-    "HttpEndpointBufferingHintsOutputTypeDef",
     "HttpEndpointBufferingHintsTypeDef",
-    "HttpEndpointCommonAttributeOutputTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
-    "HttpEndpointRetryOptionsOutputTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
-    "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
-    "TagOutputTypeDef",
     "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
-    "ParquetSerDeOutputTypeDef",
     "ParquetSerDeTypeDef",
-    "ProcessorParameterOutputTypeDef",
     "ProcessorParameterTypeDef",
     "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
-    "PutRecordOutputTypeDef",
     "RedshiftRetryOptionsTypeDef",
-    "RedshiftRetryOptionsOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SplunkRetryOptionsTypeDef",
-    "SplunkRetryOptionsOutputTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
+    "CreateDeliveryStreamOutputTypeDef",
+    "ListDeliveryStreamsOutputTypeDef",
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    "PutRecordOutputTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
     "DeserializerOutputTypeDef",
     "DeserializerTypeDef",
-    "DynamicPartitioningConfigurationOutputTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
-    "ListTagsForDeliveryStreamOutputTypeDef",
     "SerializerOutputTypeDef",
     "SerializerTypeDef",
     "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
     "PutRecordBatchOutputTypeDef",
     "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
-    "S3DestinationDescriptionTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "S3DestinationDescriptionTypeDef",
     "S3DestinationUpdateTypeDef",
     "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
     "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
     "DataFormatConversionConfigurationOutputTypeDef",
     "DataFormatConversionConfigurationTypeDef",
@@ -174,23 +153,14 @@
     "DestinationDescriptionTypeDef",
     "CreateDeliveryStreamInputRequestTypeDef",
     "UpdateDestinationInputRequestTypeDef",
     "DeliveryStreamDescriptionTypeDef",
     "DescribeDeliveryStreamOutputTypeDef",
 )
 
-AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
-    {
-        "IntervalInSeconds": int,
-        "SizeInMBs": int,
-    },
-    total=False,
-)
-
 AmazonOpenSearchServerlessBufferingHintsTypeDef = TypedDict(
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -219,51 +189,24 @@
     {
         "SubnetIds": Sequence[str],
         "RoleARN": str,
         "SecurityGroupIds": Sequence[str],
     },
 )
 
-AmazonOpenSearchServerlessRetryOptionsOutputTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
-CloudWatchLoggingOptionsOutputTypeDef = TypedDict(
-    "CloudWatchLoggingOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "LogGroupName": str,
-        "LogStreamName": str,
-    },
-    total=False,
-)
-
 VpcConfigurationDescriptionTypeDef = TypedDict(
     "VpcConfigurationDescriptionTypeDef",
     {
         "SubnetIds": List[str],
         "RoleARN": str,
         "SecurityGroupIds": List[str],
         "VpcId": str,
     },
 )
 
-AmazonopensearchserviceBufferingHintsOutputTypeDef = TypedDict(
-    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
-    {
-        "IntervalInSeconds": int,
-        "SizeInMBs": int,
-    },
-    total=False,
-)
-
 AmazonopensearchserviceBufferingHintsTypeDef = TypedDict(
     "AmazonopensearchserviceBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -273,60 +216,23 @@
     "AmazonopensearchserviceRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-AmazonopensearchserviceRetryOptionsOutputTypeDef = TypedDict(
-    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
-BufferingHintsOutputTypeDef = TypedDict(
-    "BufferingHintsOutputTypeDef",
-    {
-        "SizeInMBs": int,
-        "IntervalInSeconds": int,
-    },
-    total=False,
-)
-
 BufferingHintsTypeDef = TypedDict(
     "BufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
-_RequiredCopyCommandOutputTypeDef = TypedDict(
-    "_RequiredCopyCommandOutputTypeDef",
-    {
-        "DataTableName": str,
-    },
-)
-_OptionalCopyCommandOutputTypeDef = TypedDict(
-    "_OptionalCopyCommandOutputTypeDef",
-    {
-        "DataTableColumns": str,
-        "CopyOptions": str,
-    },
-    total=False,
-)
-
-class CopyCommandOutputTypeDef(
-    _RequiredCopyCommandOutputTypeDef, _OptionalCopyCommandOutputTypeDef
-):
-    pass
-
 _RequiredCopyCommandTypeDef = TypedDict(
     "_RequiredCopyCommandTypeDef",
     {
         "DataTableName": str,
     },
 )
 _OptionalCopyCommandTypeDef = TypedDict(
@@ -334,37 +240,41 @@
     {
         "DataTableColumns": str,
         "CopyOptions": str,
     },
     total=False,
 )
 
+
 class CopyCommandTypeDef(_RequiredCopyCommandTypeDef, _OptionalCopyCommandTypeDef):
     pass
 
+
 _RequiredDeliveryStreamEncryptionConfigurationInputTypeDef = TypedDict(
     "_RequiredDeliveryStreamEncryptionConfigurationInputTypeDef",
     {
         "KeyType": KeyTypeType,
     },
 )
 _OptionalDeliveryStreamEncryptionConfigurationInputTypeDef = TypedDict(
     "_OptionalDeliveryStreamEncryptionConfigurationInputTypeDef",
     {
         "KeyARN": str,
     },
     total=False,
 )
 
+
 class DeliveryStreamEncryptionConfigurationInputTypeDef(
     _RequiredDeliveryStreamEncryptionConfigurationInputTypeDef,
     _OptionalDeliveryStreamEncryptionConfigurationInputTypeDef,
 ):
     pass
 
+
 KinesisStreamSourceConfigurationTypeDef = TypedDict(
     "KinesisStreamSourceConfigurationTypeDef",
     {
         "KinesisStreamARN": str,
         "RoleARN": str,
     },
 )
@@ -379,36 +289,28 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CreateDeliveryStreamOutputTypeDef = TypedDict(
-    "CreateDeliveryStreamOutputTypeDef",
-    {
-        "DeliveryStreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-SchemaConfigurationOutputTypeDef = TypedDict(
-    "SchemaConfigurationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RoleARN": str,
-        "CatalogId": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "Region": str,
-        "VersionId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 SchemaConfigurationTypeDef = TypedDict(
     "SchemaConfigurationTypeDef",
     {
         "RoleARN": str,
         "CatalogId": str,
@@ -430,20 +332,22 @@
     "_OptionalDeleteDeliveryStreamInputRequestTypeDef",
     {
         "AllowForceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteDeliveryStreamInputRequestTypeDef(
     _RequiredDeleteDeliveryStreamInputRequestTypeDef,
     _OptionalDeleteDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
+
 FailureDescriptionTypeDef = TypedDict(
     "FailureDescriptionTypeDef",
     {
         "Type": DeliveryStreamFailureTypeType,
         "Details": str,
     },
 )
@@ -459,20 +363,22 @@
     {
         "Limit": int,
         "ExclusiveStartDestinationId": str,
     },
     total=False,
 )
 
+
 class DescribeDeliveryStreamInputRequestTypeDef(
     _RequiredDescribeDeliveryStreamInputRequestTypeDef,
     _OptionalDescribeDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
+
 HiveJsonSerDeOutputTypeDef = TypedDict(
     "HiveJsonSerDeOutputTypeDef",
     {
         "TimestampFormats": List[str],
     },
     total=False,
 )
@@ -501,39 +407,22 @@
         "ConvertDotsInJsonKeysToUnderscores": bool,
         "CaseInsensitive": bool,
         "ColumnToJsonKeyMappings": Mapping[str, str],
     },
     total=False,
 )
 
-RetryOptionsOutputTypeDef = TypedDict(
-    "RetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
 RetryOptionsTypeDef = TypedDict(
     "RetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-ElasticsearchBufferingHintsOutputTypeDef = TypedDict(
-    "ElasticsearchBufferingHintsOutputTypeDef",
-    {
-        "IntervalInSeconds": int,
-        "SizeInMBs": int,
-    },
-    total=False,
-)
-
 ElasticsearchBufferingHintsTypeDef = TypedDict(
     "ElasticsearchBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -543,62 +432,30 @@
     "ElasticsearchRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-ElasticsearchRetryOptionsOutputTypeDef = TypedDict(
-    "ElasticsearchRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
-KMSEncryptionConfigOutputTypeDef = TypedDict(
-    "KMSEncryptionConfigOutputTypeDef",
-    {
-        "AWSKMSKeyARN": str,
-    },
-)
-
 KMSEncryptionConfigTypeDef = TypedDict(
     "KMSEncryptionConfigTypeDef",
     {
         "AWSKMSKeyARN": str,
     },
 )
 
-HttpEndpointBufferingHintsOutputTypeDef = TypedDict(
-    "HttpEndpointBufferingHintsOutputTypeDef",
-    {
-        "SizeInMBs": int,
-        "IntervalInSeconds": int,
-    },
-    total=False,
-)
-
 HttpEndpointBufferingHintsTypeDef = TypedDict(
     "HttpEndpointBufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
-HttpEndpointCommonAttributeOutputTypeDef = TypedDict(
-    "HttpEndpointCommonAttributeOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeValue": str,
-    },
-)
-
 HttpEndpointCommonAttributeTypeDef = TypedDict(
     "HttpEndpointCommonAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
 )
@@ -614,19 +471,21 @@
     {
         "Name": str,
         "AccessKey": str,
     },
     total=False,
 )
 
+
 class HttpEndpointConfigurationTypeDef(
     _RequiredHttpEndpointConfigurationTypeDef, _OptionalHttpEndpointConfigurationTypeDef
 ):
     pass
 
+
 HttpEndpointDescriptionTypeDef = TypedDict(
     "HttpEndpointDescriptionTypeDef",
     {
         "Url": str,
         "Name": str,
     },
     total=False,
@@ -636,22 +495,14 @@
     "HttpEndpointRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-HttpEndpointRetryOptionsOutputTypeDef = TypedDict(
-    "HttpEndpointRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
 KinesisStreamSourceDescriptionTypeDef = TypedDict(
     "KinesisStreamSourceDescriptionTypeDef",
     {
         "KinesisStreamARN": str,
         "RoleARN": str,
         "DeliveryStartTimestamp": datetime,
     },
@@ -664,23 +515,14 @@
         "Limit": int,
         "DeliveryStreamType": DeliveryStreamTypeType,
         "ExclusiveStartDeliveryStreamName": str,
     },
     total=False,
 )
 
-ListDeliveryStreamsOutputTypeDef = TypedDict(
-    "ListDeliveryStreamsOutputTypeDef",
-    {
-        "DeliveryStreamNames": List[str],
-        "HasMoreDeliveryStreams": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -688,36 +530,21 @@
     {
         "ExclusiveStartTagKey": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListTagsForDeliveryStreamInputRequestTypeDef(
     _RequiredListTagsForDeliveryStreamInputRequestTypeDef,
     _OptionalListTagsForDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
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
 
 OrcSerDeOutputTypeDef = TypedDict(
     "OrcSerDeOutputTypeDef",
     {
         "StripeSizeBytes": int,
         "BlockSizeBytes": int,
         "RowIndexStride": int,
@@ -745,48 +572,27 @@
         "BloomFilterFalsePositiveProbability": float,
         "DictionaryKeyThreshold": float,
         "FormatVersion": OrcFormatVersionType,
     },
     total=False,
 )
 
-ParquetSerDeOutputTypeDef = TypedDict(
-    "ParquetSerDeOutputTypeDef",
-    {
-        "BlockSizeBytes": int,
-        "PageSizeBytes": int,
-        "Compression": ParquetCompressionType,
-        "EnableDictionaryCompression": bool,
-        "MaxPaddingBytes": int,
-        "WriterVersion": ParquetWriterVersionType,
-    },
-    total=False,
-)
-
 ParquetSerDeTypeDef = TypedDict(
     "ParquetSerDeTypeDef",
     {
         "BlockSizeBytes": int,
         "PageSizeBytes": int,
         "Compression": ParquetCompressionType,
         "EnableDictionaryCompression": bool,
         "MaxPaddingBytes": int,
         "WriterVersion": ParquetWriterVersionType,
     },
     total=False,
 )
 
-ProcessorParameterOutputTypeDef = TypedDict(
-    "ProcessorParameterOutputTypeDef",
-    {
-        "ParameterName": ProcessorParameterNameType,
-        "ParameterValue": str,
-    },
-)
-
 ProcessorParameterTypeDef = TypedDict(
     "ProcessorParameterTypeDef",
     {
         "ParameterName": ProcessorParameterNameType,
         "ParameterValue": str,
     },
 )
@@ -804,66 +610,30 @@
         "RecordId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
-    {
-        "RecordId": str,
-        "Encrypted": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedshiftRetryOptionsTypeDef = TypedDict(
     "RedshiftRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-RedshiftRetryOptionsOutputTypeDef = TypedDict(
-    "RedshiftRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
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
 SplunkRetryOptionsTypeDef = TypedDict(
     "SplunkRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
-SplunkRetryOptionsOutputTypeDef = TypedDict(
-    "SplunkRetryOptionsOutputTypeDef",
-    {
-        "DurationInSeconds": int,
-    },
-    total=False,
-)
-
 StopDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 
@@ -887,28 +657,65 @@
         "DeliveryStreamEncryptionConfigurationInput": (
             DeliveryStreamEncryptionConfigurationInputTypeDef
         ),
     },
     total=False,
 )
 
+
 class StartDeliveryStreamEncryptionInputRequestTypeDef(
     _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef,
     _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
+
 TagDeliveryStreamInputRequestTypeDef = TypedDict(
     "TagDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateDeliveryStreamOutputTypeDef = TypedDict(
+    "CreateDeliveryStreamOutputTypeDef",
+    {
+        "DeliveryStreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeliveryStreamsOutputTypeDef = TypedDict(
+    "ListDeliveryStreamsOutputTypeDef",
+    {
+        "DeliveryStreamNames": List[str],
+        "HasMoreDeliveryStreams": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "HasMoreTags": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "RecordId": str,
+        "Encrypted": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeliveryStreamEncryptionConfigurationTypeDef = TypedDict(
     "DeliveryStreamEncryptionConfigurationTypeDef",
     {
         "KeyARN": str,
         "KeyType": KeyTypeType,
         "Status": DeliveryStreamEncryptionStatusType,
         "FailureDescription": FailureDescriptionTypeDef,
@@ -930,55 +737,37 @@
     {
         "OpenXJsonSerDe": OpenXJsonSerDeTypeDef,
         "HiveJsonSerDe": HiveJsonSerDeTypeDef,
     },
     total=False,
 )
 
-DynamicPartitioningConfigurationOutputTypeDef = TypedDict(
-    "DynamicPartitioningConfigurationOutputTypeDef",
-    {
-        "RetryOptions": RetryOptionsOutputTypeDef,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 DynamicPartitioningConfigurationTypeDef = TypedDict(
     "DynamicPartitioningConfigurationTypeDef",
     {
         "RetryOptions": RetryOptionsTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "NoEncryptionConfig": Literal["NoEncryption"],
-        "KMSEncryptionConfig": KMSEncryptionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "NoEncryptionConfig": Literal["NoEncryption"],
         "KMSEncryptionConfig": KMSEncryptionConfigTypeDef,
     },
     total=False,
 )
 
 HttpEndpointRequestConfigurationOutputTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationOutputTypeDef",
     {
         "ContentEncoding": ContentEncodingType,
-        "CommonAttributes": List[HttpEndpointCommonAttributeOutputTypeDef],
+        "CommonAttributes": List[HttpEndpointCommonAttributeTypeDef],
     },
     total=False,
 )
 
 HttpEndpointRequestConfigurationTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationTypeDef",
     {
@@ -992,27 +781,18 @@
     "SourceDescriptionTypeDef",
     {
         "KinesisStreamSourceDescription": KinesisStreamSourceDescriptionTypeDef,
     },
     total=False,
 )
 
-ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
-    "ListTagsForDeliveryStreamOutputTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "HasMoreTags": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SerializerOutputTypeDef = TypedDict(
     "SerializerOutputTypeDef",
     {
-        "ParquetSerDe": ParquetSerDeOutputTypeDef,
+        "ParquetSerDe": ParquetSerDeTypeDef,
         "OrcSerDe": OrcSerDeOutputTypeDef,
     },
     total=False,
 )
 
 SerializerTypeDef = TypedDict(
     "SerializerTypeDef",
@@ -1028,39 +808,43 @@
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorOutputTypeDef = TypedDict(
     "_OptionalProcessorOutputTypeDef",
     {
-        "Parameters": List[ProcessorParameterOutputTypeDef],
+        "Parameters": List[ProcessorParameterTypeDef],
     },
     total=False,
 )
 
+
 class ProcessorOutputTypeDef(_RequiredProcessorOutputTypeDef, _OptionalProcessorOutputTypeDef):
     pass
 
+
 _RequiredProcessorTypeDef = TypedDict(
     "_RequiredProcessorTypeDef",
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorTypeDef = TypedDict(
     "_OptionalProcessorTypeDef",
     {
         "Parameters": Sequence[ProcessorParameterTypeDef],
     },
     total=False,
 )
 
+
 class ProcessorTypeDef(_RequiredProcessorTypeDef, _OptionalProcessorTypeDef):
     pass
 
+
 PutRecordBatchInputRequestTypeDef = TypedDict(
     "PutRecordBatchInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Records": Sequence[RecordTypeDef],
     },
 )
@@ -1075,15 +859,15 @@
 
 PutRecordBatchOutputTypeDef = TypedDict(
     "PutRecordBatchOutputTypeDef",
     {
         "FailedPutCount": int,
         "Encrypted": bool,
         "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputFormatConfigurationOutputTypeDef = TypedDict(
     "InputFormatConfigurationOutputTypeDef",
     {
         "Deserializer": DeserializerOutputTypeDef,
@@ -1095,64 +879,68 @@
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
     },
     total=False,
 )
 
-_RequiredS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredS3DestinationDescriptionTypeDef",
+_RequiredS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsOutputTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
-_OptionalS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalS3DestinationDescriptionTypeDef",
+_OptionalS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-class S3DestinationDescriptionTypeDef(
-    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
+
+class S3DestinationConfigurationTypeDef(
+    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
-_RequiredS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredS3DestinationConfigurationTypeDef",
+
+_RequiredS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalS3DestinationConfigurationTypeDef",
+_OptionalS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-class S3DestinationConfigurationTypeDef(
-    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
+
+class S3DestinationDescriptionTypeDef(
+    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
 ):
     pass
 
+
 S3DestinationUpdateTypeDef = TypedDict(
     "S3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
         "Prefix": str,
         "ErrorOutputPrefix": str,
@@ -1197,15 +985,15 @@
     },
     total=False,
 )
 
 DataFormatConversionConfigurationOutputTypeDef = TypedDict(
     "DataFormatConversionConfigurationOutputTypeDef",
     {
-        "SchemaConfiguration": SchemaConfigurationOutputTypeDef,
+        "SchemaConfiguration": SchemaConfigurationTypeDef,
         "InputFormatConfiguration": InputFormatConfigurationOutputTypeDef,
         "OutputFormatConfiguration": OutputFormatConfigurationOutputTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
@@ -1222,120 +1010,122 @@
 
 AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
-        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
-        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
+        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
         "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
     },
     total=False,
 )
 
 AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
         "TypeName": str,
         "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
-        "BufferingHints": AmazonopensearchserviceBufferingHintsOutputTypeDef,
-        "RetryOptions": AmazonopensearchserviceRetryOptionsOutputTypeDef,
+        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
+        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
         "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
     },
     total=False,
 )
 
 ElasticsearchDestinationDescriptionTypeDef = TypedDict(
     "ElasticsearchDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
         "TypeName": str,
         "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
-        "BufferingHints": ElasticsearchBufferingHintsOutputTypeDef,
-        "RetryOptions": ElasticsearchRetryOptionsOutputTypeDef,
+        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
+        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
         "S3BackupMode": ElasticsearchS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
     },
     total=False,
 )
 
 HttpEndpointDestinationDescriptionTypeDef = TypedDict(
     "HttpEndpointDestinationDescriptionTypeDef",
     {
         "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
-        "BufferingHints": HttpEndpointBufferingHintsOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationOutputTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "RoleARN": str,
-        "RetryOptions": HttpEndpointRetryOptionsOutputTypeDef,
+        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
         "S3BackupMode": HttpEndpointS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
     },
     total=False,
 )
 
 _RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
     "_RequiredRedshiftDestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
-        "CopyCommand": CopyCommandOutputTypeDef,
+        "CopyCommand": CopyCommandTypeDef,
         "Username": str,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
     },
 )
 _OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
     "_OptionalRedshiftDestinationDescriptionTypeDef",
     {
-        "RetryOptions": RedshiftRetryOptionsOutputTypeDef,
+        "RetryOptions": RedshiftRetryOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "S3BackupMode": RedshiftS3BackupModeType,
         "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftDestinationDescriptionTypeDef(
     _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
 ):
     pass
 
+
 SplunkDestinationDescriptionTypeDef = TypedDict(
     "SplunkDestinationDescriptionTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
-        "RetryOptions": SplunkRetryOptionsOutputTypeDef,
+        "RetryOptions": SplunkRetryOptionsTypeDef,
         "S3BackupMode": SplunkS3BackupModeType,
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
 _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef = TypedDict(
     "_RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     {
@@ -1354,20 +1144,22 @@
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(
     _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     _OptionalAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
 ):
     pass
 
+
 AmazonOpenSearchServerlessDestinationUpdateTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
         "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
@@ -1400,20 +1192,22 @@
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class AmazonopensearchserviceDestinationConfigurationTypeDef(
     _RequiredAmazonopensearchserviceDestinationConfigurationTypeDef,
     _OptionalAmazonopensearchserviceDestinationConfigurationTypeDef,
 ):
     pass
 
+
 AmazonopensearchserviceDestinationUpdateTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1449,20 +1243,22 @@
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ElasticsearchDestinationConfigurationTypeDef(
     _RequiredElasticsearchDestinationConfigurationTypeDef,
     _OptionalElasticsearchDestinationConfigurationTypeDef,
 ):
     pass
 
+
 ElasticsearchDestinationUpdateTypeDef = TypedDict(
     "ElasticsearchDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1494,20 +1290,22 @@
         "RoleARN": str,
         "RetryOptions": HttpEndpointRetryOptionsTypeDef,
         "S3BackupMode": HttpEndpointS3BackupModeType,
     },
     total=False,
 )
 
+
 class HttpEndpointDestinationConfigurationTypeDef(
     _RequiredHttpEndpointDestinationConfigurationTypeDef,
     _OptionalHttpEndpointDestinationConfigurationTypeDef,
 ):
     pass
 
+
 HttpEndpointDestinationUpdateTypeDef = TypedDict(
     "HttpEndpointDestinationUpdateTypeDef",
     {
         "EndpointConfiguration": HttpEndpointConfigurationTypeDef,
         "BufferingHints": HttpEndpointBufferingHintsTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
@@ -1539,20 +1337,22 @@
         "S3BackupMode": RedshiftS3BackupModeType,
         "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftDestinationConfigurationTypeDef(
     _RequiredRedshiftDestinationConfigurationTypeDef,
     _OptionalRedshiftDestinationConfigurationTypeDef,
 ):
     pass
 
+
 RedshiftDestinationUpdateTypeDef = TypedDict(
     "RedshiftDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
         "CopyCommand": CopyCommandTypeDef,
         "Username": str,
@@ -1584,19 +1384,21 @@
         "S3BackupMode": SplunkS3BackupModeType,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class SplunkDestinationConfigurationTypeDef(
     _RequiredSplunkDestinationConfigurationTypeDef, _OptionalSplunkDestinationConfigurationTypeDef
 ):
     pass
 
+
 SplunkDestinationUpdateTypeDef = TypedDict(
     "SplunkDestinationUpdateTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
@@ -1610,40 +1412,42 @@
 )
 
 _RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
     "_RequiredExtendedS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsOutputTypeDef,
+        "BufferingHints": BufferingHintsTypeDef,
         "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
 _OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
     "_OptionalExtendedS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "S3BackupMode": S3BackupModeType,
         "S3BackupDescription": S3DestinationDescriptionTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationOutputTypeDef,
-        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationOutputTypeDef,
+        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ExtendedS3DestinationDescriptionTypeDef(
     _RequiredExtendedS3DestinationDescriptionTypeDef,
     _OptionalExtendedS3DestinationDescriptionTypeDef,
 ):
     pass
 
+
 _RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
     "_RequiredExtendedS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
     },
 )
@@ -1661,20 +1465,22 @@
         "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ExtendedS3DestinationConfigurationTypeDef(
     _RequiredExtendedS3DestinationConfigurationTypeDef,
     _OptionalExtendedS3DestinationConfigurationTypeDef,
 ):
     pass
 
+
 ExtendedS3DestinationUpdateTypeDef = TypedDict(
     "ExtendedS3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
         "Prefix": str,
         "ErrorOutputPrefix": str,
@@ -1712,19 +1518,21 @@
         "AmazonOpenSearchServerlessDestinationDescription": (
             AmazonOpenSearchServerlessDestinationDescriptionTypeDef
         ),
     },
     total=False,
 )
 
+
 class DestinationDescriptionTypeDef(
     _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
 ):
     pass
 
+
 _RequiredCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -1748,20 +1556,22 @@
         "AmazonOpenSearchServerlessDestinationConfiguration": (
             AmazonOpenSearchServerlessDestinationConfigurationTypeDef
         ),
     },
     total=False,
 )
 
+
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDestinationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "CurrentDeliveryStreamVersionId": str,
         "DestinationId": str,
     },
@@ -1779,19 +1589,21 @@
         "AmazonOpenSearchServerlessDestinationUpdate": (
             AmazonOpenSearchServerlessDestinationUpdateTypeDef
         ),
     },
     total=False,
 )
 
+
 class UpdateDestinationInputRequestTypeDef(
     _RequiredUpdateDestinationInputRequestTypeDef, _OptionalUpdateDestinationInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeliveryStreamDescriptionTypeDef = TypedDict(
     "_RequiredDeliveryStreamDescriptionTypeDef",
     {
         "DeliveryStreamName": str,
         "DeliveryStreamARN": str,
         "DeliveryStreamStatus": DeliveryStreamStatusType,
         "DeliveryStreamType": DeliveryStreamTypeType,
@@ -1808,19 +1620,21 @@
         "CreateTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Source": SourceDescriptionTypeDef,
     },
     total=False,
 )
 
+
 class DeliveryStreamDescriptionTypeDef(
     _RequiredDeliveryStreamDescriptionTypeDef, _OptionalDeliveryStreamDescriptionTypeDef
 ):
     pass
 
+
 DescribeDeliveryStreamOutputTypeDef = TypedDict(
     "DescribeDeliveryStreamOutputTypeDef",
     {
         "DeliveryStreamDescription": DeliveryStreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/PKG-INFO` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.28.12
-Summary: Type annotations for boto3.Firehose 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Firehose 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,104 +319,82 @@
 ### Typed dictionaries
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
-    AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
-    AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
-    CloudWatchLoggingOptionsOutputTypeDef,
     VpcConfigurationDescriptionTypeDef,
-    AmazonopensearchserviceBufferingHintsOutputTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
-    AmazonopensearchserviceRetryOptionsOutputTypeDef,
-    BufferingHintsOutputTypeDef,
     BufferingHintsTypeDef,
-    CopyCommandOutputTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    SchemaConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
     HiveJsonSerDeOutputTypeDef,
     OpenXJsonSerDeOutputTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
-    RetryOptionsOutputTypeDef,
     RetryOptionsTypeDef,
-    ElasticsearchBufferingHintsOutputTypeDef,
     ElasticsearchBufferingHintsTypeDef,
     ElasticsearchRetryOptionsTypeDef,
-    ElasticsearchRetryOptionsOutputTypeDef,
-    KMSEncryptionConfigOutputTypeDef,
     KMSEncryptionConfigTypeDef,
-    HttpEndpointBufferingHintsOutputTypeDef,
     HttpEndpointBufferingHintsTypeDef,
-    HttpEndpointCommonAttributeOutputTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
-    HttpEndpointRetryOptionsOutputTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
-    TagOutputTypeDef,
     OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
-    ParquetSerDeOutputTypeDef,
     ParquetSerDeTypeDef,
-    ProcessorParameterOutputTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
-    PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
-    RedshiftRetryOptionsOutputTypeDef,
-    ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
-    SplunkRetryOptionsOutputTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    PutRecordOutputTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
     DeserializerOutputTypeDef,
     DeserializerTypeDef,
-    DynamicPartitioningConfigurationOutputTypeDef,
     DynamicPartitioningConfigurationTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
     SerializerOutputTypeDef,
     SerializerTypeDef,
     ProcessorOutputTypeDef,
     ProcessorTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
     PutRecordBatchOutputTypeDef,
     InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
-    S3DestinationDescriptionTypeDef,
     S3DestinationConfigurationTypeDef,
+    S3DestinationDescriptionTypeDef,
     S3DestinationUpdateTypeDef,
     OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
     ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     DataFormatConversionConfigurationOutputTypeDef,
     DataFormatConversionConfigurationTypeDef,
@@ -445,15 +423,15 @@
     CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsOutputTypeDef:
+def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/SOURCES.txt` & `mypy-boto3-firehose-1.28.15/mypy_boto3_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.12/setup.py` & `mypy-boto3-firehose-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-firehose",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Firehose 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Firehose 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

