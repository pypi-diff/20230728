# Comparing `tmp/mypy-boto3-kafkaconnect-1.28.12.tar.gz` & `tmp/mypy-boto3-kafkaconnect-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafkaconnect-1.28.12.tar", last modified: Thu Jul 27 05:34:52 2023, max compression
+gzip compressed data, was "mypy-boto3-kafkaconnect-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-kafkaconnect-1.28.12.tar` & `mypy-boto3-kafkaconnect-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.144473 mypy-boto3-kafkaconnect-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-27 05:34:52.144473 mypy-boto3-kafkaconnect-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.144473 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25544 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25523 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.144473 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-27 05:34:51.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:52.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:51.000000 mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:52.144473 mypy-boto3-kafkaconnect-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:30.000000 mypy-boto3-kafkaconnect-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.753302 mypy-boto3-kafkaconnect-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-28 20:43:02.753302 mypy-boto3-kafkaconnect-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.737302 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-07-28 20:28:57.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-07-28 20:28:59.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25493 2023-07-28 20:28:59.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.753302 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-28 20:43:02.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:02.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:02.000000 mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.753302 mypy-boto3-kafkaconnect-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:56.000000 mypy-boto3-kafkaconnect-1.28.15/setup.py
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/LICENSE` & `mypy-boto3-kafkaconnect-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/PKG-INFO` & `mypy-boto3-kafkaconnect-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafkaconnect
-Version: 1.28.12
-Summary: Type annotations for boto3.KafkaConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KafkaConnect 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafkaconnect)](https://pepy.tech/project/mypy-boto3-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KafkaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[boto3.KafkaConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [mypy-boto3-kafkaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,57 +355,57 @@
     CloudWatchLogsLogDeliveryTypeDef,
     KafkaClusterClientAuthenticationDescriptionTypeDef,
     KafkaClusterEncryptionInTransitDescriptionTypeDef,
     WorkerConfigurationDescriptionTypeDef,
     KafkaClusterClientAuthenticationTypeDef,
     KafkaClusterEncryptionInTransitTypeDef,
     WorkerConfigurationTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionSummaryTypeDef,
     CustomPluginDescriptionTypeDef,
     CustomPluginFileDescriptionTypeDef,
     S3LocationDescriptionTypeDef,
     S3LocationTypeDef,
     CustomPluginTypeDef,
     DeleteConnectorRequestRequestTypeDef,
-    DeleteConnectorResponseTypeDef,
     DeleteCustomPluginRequestRequestTypeDef,
-    DeleteCustomPluginResponseTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     StateDescriptionTypeDef,
     DescribeCustomPluginRequestRequestTypeDef,
     DescribeWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionDescriptionTypeDef,
     FirehoseLogDeliveryDescriptionTypeDef,
     FirehoseLogDeliveryTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConnectorsRequestRequestTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
     ListCustomPluginsRequestRequestTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     ListWorkerConfigurationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     S3LogDeliveryDescriptionTypeDef,
     S3LogDeliveryTypeDef,
-    UpdateConnectorResponseTypeDef,
     ApacheKafkaClusterDescriptionTypeDef,
     ApacheKafkaClusterTypeDef,
     AutoScalingDescriptionTypeDef,
     AutoScalingTypeDef,
     AutoScalingUpdateTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateCustomPluginResponseTypeDef,
+    DeleteConnectorResponseTypeDef,
+    DeleteCustomPluginResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
     CreateWorkerConfigurationResponseTypeDef,
     WorkerConfigurationSummaryTypeDef,
     PluginDescriptionTypeDef,
     CustomPluginLocationDescriptionTypeDef,
     CustomPluginLocationTypeDef,
     PluginTypeDef,
     DescribeWorkerConfigurationResponseTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
+    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     WorkerLogDeliveryDescriptionTypeDef,
     WorkerLogDeliveryTypeDef,
     KafkaClusterDescriptionTypeDef,
     KafkaClusterTypeDef,
     CapacityDescriptionTypeDef,
     CapacityTypeDef,
     CapacityUpdateTypeDef,
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/README.md` & `mypy-boto3-kafkaconnect-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafkaconnect)](https://pepy.tech/project/mypy-boto3-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KafkaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[boto3.KafkaConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [mypy-boto3-kafkaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,57 +323,57 @@
     CloudWatchLogsLogDeliveryTypeDef,
     KafkaClusterClientAuthenticationDescriptionTypeDef,
     KafkaClusterEncryptionInTransitDescriptionTypeDef,
     WorkerConfigurationDescriptionTypeDef,
     KafkaClusterClientAuthenticationTypeDef,
     KafkaClusterEncryptionInTransitTypeDef,
     WorkerConfigurationTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionSummaryTypeDef,
     CustomPluginDescriptionTypeDef,
     CustomPluginFileDescriptionTypeDef,
     S3LocationDescriptionTypeDef,
     S3LocationTypeDef,
     CustomPluginTypeDef,
     DeleteConnectorRequestRequestTypeDef,
-    DeleteConnectorResponseTypeDef,
     DeleteCustomPluginRequestRequestTypeDef,
-    DeleteCustomPluginResponseTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     StateDescriptionTypeDef,
     DescribeCustomPluginRequestRequestTypeDef,
     DescribeWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionDescriptionTypeDef,
     FirehoseLogDeliveryDescriptionTypeDef,
     FirehoseLogDeliveryTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConnectorsRequestRequestTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
     ListCustomPluginsRequestRequestTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     ListWorkerConfigurationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     S3LogDeliveryDescriptionTypeDef,
     S3LogDeliveryTypeDef,
-    UpdateConnectorResponseTypeDef,
     ApacheKafkaClusterDescriptionTypeDef,
     ApacheKafkaClusterTypeDef,
     AutoScalingDescriptionTypeDef,
     AutoScalingTypeDef,
     AutoScalingUpdateTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateCustomPluginResponseTypeDef,
+    DeleteConnectorResponseTypeDef,
+    DeleteCustomPluginResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
     CreateWorkerConfigurationResponseTypeDef,
     WorkerConfigurationSummaryTypeDef,
     PluginDescriptionTypeDef,
     CustomPluginLocationDescriptionTypeDef,
     CustomPluginLocationTypeDef,
     PluginTypeDef,
     DescribeWorkerConfigurationResponseTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
+    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     WorkerLogDeliveryDescriptionTypeDef,
     WorkerLogDeliveryTypeDef,
     KafkaClusterDescriptionTypeDef,
     KafkaClusterTypeDef,
     CapacityDescriptionTypeDef,
     CapacityTypeDef,
     CapacityUpdateTypeDef,
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/__init__.py` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/__init__.pyi` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/__main__.py` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KafkaConnect 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KafkaConnect 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect\nOther"
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

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/client.py` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/client.pyi` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/literals.py` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/literals.pyi` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/paginator.py` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,43 +54,43 @@
 class ListConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, connectorNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, connectorNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
         """
 
 
 class ListCustomPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
         """
 
 
 class ListWorkerConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkerConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/paginator.pyi` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,41 +51,41 @@
 class ListConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, connectorNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, connectorNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
         """
 
 class ListCustomPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
         """
 
 class ListWorkerConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkerConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/type_defs.py` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "VpcDescriptionTypeDef",
     "VpcTypeDef",
     "ScaleInPolicyDescriptionTypeDef",
     "ScaleOutPolicyDescriptionTypeDef",
     "ScaleInPolicyTypeDef",
     "ScaleOutPolicyTypeDef",
@@ -45,57 +44,57 @@
     "CloudWatchLogsLogDeliveryTypeDef",
     "KafkaClusterClientAuthenticationDescriptionTypeDef",
     "KafkaClusterEncryptionInTransitDescriptionTypeDef",
     "WorkerConfigurationDescriptionTypeDef",
     "KafkaClusterClientAuthenticationTypeDef",
     "KafkaClusterEncryptionInTransitTypeDef",
     "WorkerConfigurationTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateCustomPluginResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionSummaryTypeDef",
     "CustomPluginDescriptionTypeDef",
     "CustomPluginFileDescriptionTypeDef",
     "S3LocationDescriptionTypeDef",
     "S3LocationTypeDef",
     "CustomPluginTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
-    "DeleteConnectorResponseTypeDef",
     "DeleteCustomPluginRequestRequestTypeDef",
-    "DeleteCustomPluginResponseTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "StateDescriptionTypeDef",
     "DescribeCustomPluginRequestRequestTypeDef",
     "DescribeWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionDescriptionTypeDef",
     "FirehoseLogDeliveryDescriptionTypeDef",
     "FirehoseLogDeliveryTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConnectorsRequestRequestTypeDef",
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
     "ListCustomPluginsRequestRequestTypeDef",
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "ListWorkerConfigurationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "S3LogDeliveryDescriptionTypeDef",
     "S3LogDeliveryTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "ApacheKafkaClusterDescriptionTypeDef",
     "ApacheKafkaClusterTypeDef",
     "AutoScalingDescriptionTypeDef",
     "AutoScalingTypeDef",
     "AutoScalingUpdateTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateCustomPluginResponseTypeDef",
+    "DeleteConnectorResponseTypeDef",
+    "DeleteCustomPluginResponseTypeDef",
+    "UpdateConnectorResponseTypeDef",
     "CreateWorkerConfigurationResponseTypeDef",
     "WorkerConfigurationSummaryTypeDef",
     "PluginDescriptionTypeDef",
     "CustomPluginLocationDescriptionTypeDef",
     "CustomPluginLocationTypeDef",
     "PluginTypeDef",
     "DescribeWorkerConfigurationResponseTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "WorkerLogDeliveryDescriptionTypeDef",
     "WorkerLogDeliveryTypeDef",
     "KafkaClusterDescriptionTypeDef",
     "KafkaClusterTypeDef",
     "CapacityDescriptionTypeDef",
     "CapacityTypeDef",
     "CapacityUpdateTypeDef",
@@ -133,19 +132,17 @@
     "_OptionalVpcTypeDef",
     {
         "securityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcTypeDef(_RequiredVpcTypeDef, _OptionalVpcTypeDef):
     pass
 
-
 ScaleInPolicyDescriptionTypeDef = TypedDict(
     "ScaleInPolicyDescriptionTypeDef",
     {
         "cpuUtilizationPercentage": int,
     },
     total=False,
 )
@@ -230,21 +227,19 @@
     "_OptionalCloudWatchLogsLogDeliveryTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
 
-
 class CloudWatchLogsLogDeliveryTypeDef(
     _RequiredCloudWatchLogsLogDeliveryTypeDef, _OptionalCloudWatchLogsLogDeliveryTypeDef
 ):
     pass
 
-
 KafkaClusterClientAuthenticationDescriptionTypeDef = TypedDict(
     "KafkaClusterClientAuthenticationDescriptionTypeDef",
     {
         "authenticationType": KafkaClusterClientAuthenticationTypeType,
     },
     total=False,
 )
@@ -284,32 +279,22 @@
     "WorkerConfigurationTypeDef",
     {
         "revision": int,
         "workerConfigurationArn": str,
     },
 )
 
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorName": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomPluginResponseTypeDef = TypedDict(
-    "CreateCustomPluginResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "name": str,
-        "revision": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateWorkerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerConfigurationRequestRequestTypeDef",
     {
         "name": str,
@@ -320,22 +305,20 @@
     "_OptionalCreateWorkerConfigurationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class CreateWorkerConfigurationRequestRequestTypeDef(
     _RequiredCreateWorkerConfigurationRequestRequestTypeDef,
     _OptionalCreateWorkerConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 WorkerConfigurationRevisionSummaryTypeDef = TypedDict(
     "WorkerConfigurationRevisionSummaryTypeDef",
     {
         "creationTime": datetime,
         "description": str,
         "revision": int,
     },
@@ -381,19 +364,17 @@
     "_OptionalS3LocationTypeDef",
     {
         "objectVersion": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 CustomPluginTypeDef = TypedDict(
     "CustomPluginTypeDef",
     {
         "customPluginArn": str,
         "revision": int,
     },
 )
@@ -408,46 +389,26 @@
     "_OptionalDeleteConnectorRequestRequestTypeDef",
     {
         "currentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteConnectorRequestRequestTypeDef(
     _RequiredDeleteConnectorRequestRequestTypeDef, _OptionalDeleteConnectorRequestRequestTypeDef
 ):
     pass
 
-
-DeleteConnectorResponseTypeDef = TypedDict(
-    "DeleteConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCustomPluginRequestRequestTypeDef = TypedDict(
     "DeleteCustomPluginRequestRequestTypeDef",
     {
         "customPluginArn": str,
     },
 )
 
-DeleteCustomPluginResponseTypeDef = TypedDict(
-    "DeleteCustomPluginResponseTypeDef",
-    {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConnectorRequestRequestTypeDef = TypedDict(
     "DescribeConnectorRequestRequestTypeDef",
     {
         "connectorArn": str,
     },
 )
 
@@ -504,95 +465,57 @@
     "_OptionalFirehoseLogDeliveryTypeDef",
     {
         "deliveryStream": str,
     },
     total=False,
 )
 
-
 class FirehoseLogDeliveryTypeDef(
     _RequiredFirehoseLogDeliveryTypeDef, _OptionalFirehoseLogDeliveryTypeDef
 ):
     pass
 
-
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "connectorNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "connectorNamePrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomPluginsRequestRequestTypeDef = TypedDict(
     "ListCustomPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkerConfigurationsRequestRequestTypeDef = TypedDict(
     "ListWorkerConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
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
 S3LogDeliveryDescriptionTypeDef = TypedDict(
     "S3LogDeliveryDescriptionTypeDef",
     {
         "bucket": str,
         "enabled": bool,
         "prefix": str,
     },
@@ -610,28 +533,17 @@
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3LogDeliveryTypeDef(_RequiredS3LogDeliveryTypeDef, _OptionalS3LogDeliveryTypeDef):
     pass
 
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApacheKafkaClusterDescriptionTypeDef = TypedDict(
     "ApacheKafkaClusterDescriptionTypeDef",
     {
         "bootstrapServers": str,
         "vpc": VpcDescriptionTypeDef,
     },
     total=False,
@@ -670,38 +582,84 @@
     {
         "scaleInPolicy": ScaleInPolicyTypeDef,
         "scaleOutPolicy": ScaleOutPolicyTypeDef,
     },
     total=False,
 )
 
-
 class AutoScalingTypeDef(_RequiredAutoScalingTypeDef, _OptionalAutoScalingTypeDef):
     pass
 
-
 AutoScalingUpdateTypeDef = TypedDict(
     "AutoScalingUpdateTypeDef",
     {
         "maxWorkerCount": int,
         "mcuCount": int,
         "minWorkerCount": int,
         "scaleInPolicy": ScaleInPolicyUpdateTypeDef,
         "scaleOutPolicy": ScaleOutPolicyUpdateTypeDef,
     },
 )
 
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorName": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomPluginResponseTypeDef = TypedDict(
+    "CreateCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "name": str,
+        "revision": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteConnectorResponseTypeDef = TypedDict(
+    "DeleteConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomPluginResponseTypeDef = TypedDict(
+    "DeleteCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkerConfigurationResponseTypeDef = TypedDict(
     "CreateWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "latestRevision": WorkerConfigurationRevisionSummaryTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkerConfigurationSummaryTypeDef = TypedDict(
     "WorkerConfigurationSummaryTypeDef",
     {
         "creationTime": datetime,
@@ -747,16 +705,41 @@
     "DescribeWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "description": str,
         "latestRevision": WorkerConfigurationRevisionDescriptionTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    {
+        "connectorNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 WorkerLogDeliveryDescriptionTypeDef = TypedDict(
     "WorkerLogDeliveryDescriptionTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsLogDeliveryDescriptionTypeDef,
         "firehose": FirehoseLogDeliveryDescriptionTypeDef,
@@ -818,15 +801,15 @@
 )
 
 ListWorkerConfigurationsResponseTypeDef = TypedDict(
     "ListWorkerConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "workerConfigurations": List[WorkerConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomPluginRevisionSummaryTypeDef = TypedDict(
     "CustomPluginRevisionSummaryTypeDef",
     {
         "contentType": CustomPluginContentTypeType,
@@ -851,22 +834,20 @@
     "_OptionalCreateCustomPluginRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class CreateCustomPluginRequestRequestTypeDef(
     _RequiredCreateCustomPluginRequestRequestTypeDef,
     _OptionalCreateCustomPluginRequestRequestTypeDef,
 ):
     pass
 
-
 LogDeliveryDescriptionTypeDef = TypedDict(
     "LogDeliveryDescriptionTypeDef",
     {
         "workerLogDelivery": WorkerLogDeliveryDescriptionTypeDef,
     },
     total=False,
 )
@@ -906,15 +887,15 @@
         "creationTime": datetime,
         "customPluginArn": str,
         "customPluginState": CustomPluginStateType,
         "description": str,
         "latestRevision": CustomPluginRevisionSummaryTypeDef,
         "name": str,
         "stateDescription": StateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorSummaryTypeDef = TypedDict(
     "ConnectorSummaryTypeDef",
     {
         "capacity": CapacityDescriptionTypeDef,
@@ -952,15 +933,15 @@
         "kafkaClusterEncryptionInTransit": KafkaClusterEncryptionInTransitDescriptionTypeDef,
         "kafkaConnectVersion": str,
         "logDelivery": LogDeliveryDescriptionTypeDef,
         "plugins": List[PluginDescriptionTypeDef],
         "serviceExecutionRoleArn": str,
         "stateDescription": StateDescriptionTypeDef,
         "workerConfiguration": WorkerConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorRequestRequestTypeDef",
     {
         "capacity": CapacityTypeDef,
@@ -980,31 +961,29 @@
         "connectorDescription": str,
         "logDelivery": LogDeliveryTypeDef,
         "workerConfiguration": WorkerConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateConnectorRequestRequestTypeDef(
     _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
 ):
     pass
 
-
 ListCustomPluginsResponseTypeDef = TypedDict(
     "ListCustomPluginsResponseTypeDef",
     {
         "customPlugins": List[CustomPluginSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect/type_defs.pyi` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "VpcDescriptionTypeDef",
     "VpcTypeDef",
     "ScaleInPolicyDescriptionTypeDef",
     "ScaleOutPolicyDescriptionTypeDef",
     "ScaleInPolicyTypeDef",
     "ScaleOutPolicyTypeDef",
@@ -44,57 +45,57 @@
     "CloudWatchLogsLogDeliveryTypeDef",
     "KafkaClusterClientAuthenticationDescriptionTypeDef",
     "KafkaClusterEncryptionInTransitDescriptionTypeDef",
     "WorkerConfigurationDescriptionTypeDef",
     "KafkaClusterClientAuthenticationTypeDef",
     "KafkaClusterEncryptionInTransitTypeDef",
     "WorkerConfigurationTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateCustomPluginResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionSummaryTypeDef",
     "CustomPluginDescriptionTypeDef",
     "CustomPluginFileDescriptionTypeDef",
     "S3LocationDescriptionTypeDef",
     "S3LocationTypeDef",
     "CustomPluginTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
-    "DeleteConnectorResponseTypeDef",
     "DeleteCustomPluginRequestRequestTypeDef",
-    "DeleteCustomPluginResponseTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "StateDescriptionTypeDef",
     "DescribeCustomPluginRequestRequestTypeDef",
     "DescribeWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionDescriptionTypeDef",
     "FirehoseLogDeliveryDescriptionTypeDef",
     "FirehoseLogDeliveryTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConnectorsRequestRequestTypeDef",
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
     "ListCustomPluginsRequestRequestTypeDef",
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "ListWorkerConfigurationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "S3LogDeliveryDescriptionTypeDef",
     "S3LogDeliveryTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "ApacheKafkaClusterDescriptionTypeDef",
     "ApacheKafkaClusterTypeDef",
     "AutoScalingDescriptionTypeDef",
     "AutoScalingTypeDef",
     "AutoScalingUpdateTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateCustomPluginResponseTypeDef",
+    "DeleteConnectorResponseTypeDef",
+    "DeleteCustomPluginResponseTypeDef",
+    "UpdateConnectorResponseTypeDef",
     "CreateWorkerConfigurationResponseTypeDef",
     "WorkerConfigurationSummaryTypeDef",
     "PluginDescriptionTypeDef",
     "CustomPluginLocationDescriptionTypeDef",
     "CustomPluginLocationTypeDef",
     "PluginTypeDef",
     "DescribeWorkerConfigurationResponseTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "WorkerLogDeliveryDescriptionTypeDef",
     "WorkerLogDeliveryTypeDef",
     "KafkaClusterDescriptionTypeDef",
     "KafkaClusterTypeDef",
     "CapacityDescriptionTypeDef",
     "CapacityTypeDef",
     "CapacityUpdateTypeDef",
@@ -132,17 +133,19 @@
     "_OptionalVpcTypeDef",
     {
         "securityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcTypeDef(_RequiredVpcTypeDef, _OptionalVpcTypeDef):
     pass
 
+
 ScaleInPolicyDescriptionTypeDef = TypedDict(
     "ScaleInPolicyDescriptionTypeDef",
     {
         "cpuUtilizationPercentage": int,
     },
     total=False,
 )
@@ -227,19 +230,21 @@
     "_OptionalCloudWatchLogsLogDeliveryTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
 
+
 class CloudWatchLogsLogDeliveryTypeDef(
     _RequiredCloudWatchLogsLogDeliveryTypeDef, _OptionalCloudWatchLogsLogDeliveryTypeDef
 ):
     pass
 
+
 KafkaClusterClientAuthenticationDescriptionTypeDef = TypedDict(
     "KafkaClusterClientAuthenticationDescriptionTypeDef",
     {
         "authenticationType": KafkaClusterClientAuthenticationTypeType,
     },
     total=False,
 )
@@ -279,32 +284,22 @@
     "WorkerConfigurationTypeDef",
     {
         "revision": int,
         "workerConfigurationArn": str,
     },
 )
 
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorName": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomPluginResponseTypeDef = TypedDict(
-    "CreateCustomPluginResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "name": str,
-        "revision": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateWorkerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerConfigurationRequestRequestTypeDef",
     {
         "name": str,
@@ -315,20 +310,22 @@
     "_OptionalCreateWorkerConfigurationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class CreateWorkerConfigurationRequestRequestTypeDef(
     _RequiredCreateWorkerConfigurationRequestRequestTypeDef,
     _OptionalCreateWorkerConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 WorkerConfigurationRevisionSummaryTypeDef = TypedDict(
     "WorkerConfigurationRevisionSummaryTypeDef",
     {
         "creationTime": datetime,
         "description": str,
         "revision": int,
     },
@@ -374,17 +371,19 @@
     "_OptionalS3LocationTypeDef",
     {
         "objectVersion": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 CustomPluginTypeDef = TypedDict(
     "CustomPluginTypeDef",
     {
         "customPluginArn": str,
         "revision": int,
     },
 )
@@ -399,44 +398,28 @@
     "_OptionalDeleteConnectorRequestRequestTypeDef",
     {
         "currentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteConnectorRequestRequestTypeDef(
     _RequiredDeleteConnectorRequestRequestTypeDef, _OptionalDeleteConnectorRequestRequestTypeDef
 ):
     pass
 
-DeleteConnectorResponseTypeDef = TypedDict(
-    "DeleteConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteCustomPluginRequestRequestTypeDef = TypedDict(
     "DeleteCustomPluginRequestRequestTypeDef",
     {
         "customPluginArn": str,
     },
 )
 
-DeleteCustomPluginResponseTypeDef = TypedDict(
-    "DeleteCustomPluginResponseTypeDef",
-    {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConnectorRequestRequestTypeDef = TypedDict(
     "DescribeConnectorRequestRequestTypeDef",
     {
         "connectorArn": str,
     },
 )
 
@@ -493,93 +476,59 @@
     "_OptionalFirehoseLogDeliveryTypeDef",
     {
         "deliveryStream": str,
     },
     total=False,
 )
 
+
 class FirehoseLogDeliveryTypeDef(
     _RequiredFirehoseLogDeliveryTypeDef, _OptionalFirehoseLogDeliveryTypeDef
 ):
     pass
 
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "connectorNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "connectorNamePrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomPluginsRequestRequestTypeDef = TypedDict(
     "ListCustomPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkerConfigurationsRequestRequestTypeDef = TypedDict(
     "ListWorkerConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
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
 S3LogDeliveryDescriptionTypeDef = TypedDict(
     "S3LogDeliveryDescriptionTypeDef",
     {
         "bucket": str,
         "enabled": bool,
         "prefix": str,
     },
@@ -597,25 +546,18 @@
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3LogDeliveryTypeDef(_RequiredS3LogDeliveryTypeDef, _OptionalS3LogDeliveryTypeDef):
     pass
 
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ApacheKafkaClusterDescriptionTypeDef = TypedDict(
     "ApacheKafkaClusterDescriptionTypeDef",
     {
         "bootstrapServers": str,
         "vpc": VpcDescriptionTypeDef,
     },
@@ -655,36 +597,86 @@
     {
         "scaleInPolicy": ScaleInPolicyTypeDef,
         "scaleOutPolicy": ScaleOutPolicyTypeDef,
     },
     total=False,
 )
 
+
 class AutoScalingTypeDef(_RequiredAutoScalingTypeDef, _OptionalAutoScalingTypeDef):
     pass
 
+
 AutoScalingUpdateTypeDef = TypedDict(
     "AutoScalingUpdateTypeDef",
     {
         "maxWorkerCount": int,
         "mcuCount": int,
         "minWorkerCount": int,
         "scaleInPolicy": ScaleInPolicyUpdateTypeDef,
         "scaleOutPolicy": ScaleOutPolicyUpdateTypeDef,
     },
 )
 
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorName": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomPluginResponseTypeDef = TypedDict(
+    "CreateCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "name": str,
+        "revision": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteConnectorResponseTypeDef = TypedDict(
+    "DeleteConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomPluginResponseTypeDef = TypedDict(
+    "DeleteCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkerConfigurationResponseTypeDef = TypedDict(
     "CreateWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "latestRevision": WorkerConfigurationRevisionSummaryTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkerConfigurationSummaryTypeDef = TypedDict(
     "WorkerConfigurationSummaryTypeDef",
     {
         "creationTime": datetime,
@@ -730,18 +722,43 @@
     "DescribeWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "description": str,
         "latestRevision": WorkerConfigurationRevisionDescriptionTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    {
+        "connectorNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 WorkerLogDeliveryDescriptionTypeDef = TypedDict(
     "WorkerLogDeliveryDescriptionTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsLogDeliveryDescriptionTypeDef,
         "firehose": FirehoseLogDeliveryDescriptionTypeDef,
         "s3": S3LogDeliveryDescriptionTypeDef,
     },
@@ -801,15 +818,15 @@
 )
 
 ListWorkerConfigurationsResponseTypeDef = TypedDict(
     "ListWorkerConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "workerConfigurations": List[WorkerConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomPluginRevisionSummaryTypeDef = TypedDict(
     "CustomPluginRevisionSummaryTypeDef",
     {
         "contentType": CustomPluginContentTypeType,
@@ -834,20 +851,22 @@
     "_OptionalCreateCustomPluginRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class CreateCustomPluginRequestRequestTypeDef(
     _RequiredCreateCustomPluginRequestRequestTypeDef,
     _OptionalCreateCustomPluginRequestRequestTypeDef,
 ):
     pass
 
+
 LogDeliveryDescriptionTypeDef = TypedDict(
     "LogDeliveryDescriptionTypeDef",
     {
         "workerLogDelivery": WorkerLogDeliveryDescriptionTypeDef,
     },
     total=False,
 )
@@ -887,15 +906,15 @@
         "creationTime": datetime,
         "customPluginArn": str,
         "customPluginState": CustomPluginStateType,
         "description": str,
         "latestRevision": CustomPluginRevisionSummaryTypeDef,
         "name": str,
         "stateDescription": StateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorSummaryTypeDef = TypedDict(
     "ConnectorSummaryTypeDef",
     {
         "capacity": CapacityDescriptionTypeDef,
@@ -933,15 +952,15 @@
         "kafkaClusterEncryptionInTransit": KafkaClusterEncryptionInTransitDescriptionTypeDef,
         "kafkaConnectVersion": str,
         "logDelivery": LogDeliveryDescriptionTypeDef,
         "plugins": List[PluginDescriptionTypeDef],
         "serviceExecutionRoleArn": str,
         "stateDescription": StateDescriptionTypeDef,
         "workerConfiguration": WorkerConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorRequestRequestTypeDef",
     {
         "capacity": CapacityTypeDef,
@@ -961,29 +980,31 @@
         "connectorDescription": str,
         "logDelivery": LogDeliveryTypeDef,
         "workerConfiguration": WorkerConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateConnectorRequestRequestTypeDef(
     _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
 ):
     pass
 
+
 ListCustomPluginsResponseTypeDef = TypedDict(
     "ListCustomPluginsResponseTypeDef",
     {
         "customPlugins": List[CustomPluginSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/PKG-INFO` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafkaconnect
-Version: 1.28.12
-Summary: Type annotations for boto3.KafkaConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KafkaConnect 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafkaconnect)](https://pepy.tech/project/mypy-boto3-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KafkaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[boto3.KafkaConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [mypy-boto3-kafkaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,57 +355,57 @@
     CloudWatchLogsLogDeliveryTypeDef,
     KafkaClusterClientAuthenticationDescriptionTypeDef,
     KafkaClusterEncryptionInTransitDescriptionTypeDef,
     WorkerConfigurationDescriptionTypeDef,
     KafkaClusterClientAuthenticationTypeDef,
     KafkaClusterEncryptionInTransitTypeDef,
     WorkerConfigurationTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionSummaryTypeDef,
     CustomPluginDescriptionTypeDef,
     CustomPluginFileDescriptionTypeDef,
     S3LocationDescriptionTypeDef,
     S3LocationTypeDef,
     CustomPluginTypeDef,
     DeleteConnectorRequestRequestTypeDef,
-    DeleteConnectorResponseTypeDef,
     DeleteCustomPluginRequestRequestTypeDef,
-    DeleteCustomPluginResponseTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     StateDescriptionTypeDef,
     DescribeCustomPluginRequestRequestTypeDef,
     DescribeWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionDescriptionTypeDef,
     FirehoseLogDeliveryDescriptionTypeDef,
     FirehoseLogDeliveryTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConnectorsRequestRequestTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
     ListCustomPluginsRequestRequestTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     ListWorkerConfigurationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     S3LogDeliveryDescriptionTypeDef,
     S3LogDeliveryTypeDef,
-    UpdateConnectorResponseTypeDef,
     ApacheKafkaClusterDescriptionTypeDef,
     ApacheKafkaClusterTypeDef,
     AutoScalingDescriptionTypeDef,
     AutoScalingTypeDef,
     AutoScalingUpdateTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateCustomPluginResponseTypeDef,
+    DeleteConnectorResponseTypeDef,
+    DeleteCustomPluginResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
     CreateWorkerConfigurationResponseTypeDef,
     WorkerConfigurationSummaryTypeDef,
     PluginDescriptionTypeDef,
     CustomPluginLocationDescriptionTypeDef,
     CustomPluginLocationTypeDef,
     PluginTypeDef,
     DescribeWorkerConfigurationResponseTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
+    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     WorkerLogDeliveryDescriptionTypeDef,
     WorkerLogDeliveryTypeDef,
     KafkaClusterDescriptionTypeDef,
     KafkaClusterTypeDef,
     CapacityDescriptionTypeDef,
     CapacityTypeDef,
     CapacityUpdateTypeDef,
```

### Comparing `mypy-boto3-kafkaconnect-1.28.12/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt` & `mypy-boto3-kafkaconnect-1.28.15/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.28.12/setup.py` & `mypy-boto3-kafkaconnect-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafkaconnect",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kafkaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KafkaConnect 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.KafkaConnect 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

