# Comparing `tmp/mypy-boto3-timestream-write-1.28.12.tar.gz` & `tmp/mypy-boto3-timestream-write-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-write-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-write-1.28.15.tar", last modified: Fri Jul 28 20:43:53 2023, max compression
```

## Comparing `mypy-boto3-timestream-write-1.28.12.tar` & `mypy-boto3-timestream-write-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.685443 mypy-boto3-timestream-write-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-07-27 11:49:46.681443 mypy-boto3-timestream-write-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.681443 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29204 2023-07-27 11:48:02.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.681443 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.685443 mypy-boto3-timestream-write-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.249994 mypy-boto3-timestream-write-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-28 20:43:53.245994 mypy-boto3-timestream-write-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.229994 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-07-28 20:40:39.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-07-28 20:40:39.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.245994 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:53.249994 mypy-boto3-timestream-write-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/setup.py
```

### Comparing `mypy-boto3-timestream-write-1.28.12/LICENSE` & `mypy-boto3-timestream-write-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.12/PKG-INFO` & `mypy-boto3-timestream-write-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.12
-Summary: Type annotations for boto3.TimestreamWrite 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,80 +313,66 @@
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
-    CsvConfigurationOutputTypeDef,
     CsvConfigurationTypeDef,
-    DataModelS3ConfigurationOutputTypeDef,
     DataModelS3ConfigurationTypeDef,
-    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    DataSourceS3ConfigurationOutputTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
-    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
-    ReportS3ConfigurationOutputTypeDef,
     ReportS3ConfigurationTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
-    RetentionPropertiesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     CreateBatchLoadTaskResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
-    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MagneticStoreRejectedDataLocationOutputTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingOutputTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
-    ReportConfigurationOutputTypeDef,
     ReportConfigurationTypeDef,
-    MagneticStoreWritePropertiesOutputTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelOutputTypeDef,
     DataModelTypeDef,
-    TableTypeDef,
     CreateTableRequestRequestTypeDef,
+    TableTypeDef,
     UpdateTableRequestRequestTypeDef,
     DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
```

### Comparing `mypy-boto3-timestream-write-1.28.12/README.md` & `mypy-boto3-timestream-write-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,80 +281,66 @@
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
-    CsvConfigurationOutputTypeDef,
     CsvConfigurationTypeDef,
-    DataModelS3ConfigurationOutputTypeDef,
     DataModelS3ConfigurationTypeDef,
-    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    DataSourceS3ConfigurationOutputTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
-    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
-    ReportS3ConfigurationOutputTypeDef,
     ReportS3ConfigurationTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
-    RetentionPropertiesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     CreateBatchLoadTaskResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
-    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MagneticStoreRejectedDataLocationOutputTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingOutputTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
-    ReportConfigurationOutputTypeDef,
     ReportConfigurationTypeDef,
-    MagneticStoreWritePropertiesOutputTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelOutputTypeDef,
     DataModelTypeDef,
-    TableTypeDef,
     CreateTableRequestRequestTypeDef,
+    TableTypeDef,
     UpdateTableRequestRequestTypeDef,
     DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
```

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__main__.py` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamWrite 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.TimestreamWrite 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
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

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.py` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.pyi` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.py` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.pyi` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.py` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -31,88 +31,73 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
-    "CsvConfigurationOutputTypeDef",
     "CsvConfigurationTypeDef",
-    "DataModelS3ConfigurationOutputTypeDef",
     "DataModelS3ConfigurationTypeDef",
-    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
-    "DataSourceS3ConfigurationOutputTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
-    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
-    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
-    "ReportS3ConfigurationOutputTypeDef",
     "ReportS3ConfigurationTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
-    "RetentionPropertiesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "CreateBatchLoadTaskResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
-    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MagneticStoreRejectedDataLocationOutputTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
     "MixedMeasureMappingOutputTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
-    "ReportConfigurationOutputTypeDef",
     "ReportConfigurationTypeDef",
-    "MagneticStoreWritePropertiesOutputTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelOutputTypeDef",
     "DataModelTypeDef",
-    "TableTypeDef",
     "CreateTableRequestRequestTypeDef",
+    "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
@@ -184,116 +169,63 @@
     "RetentionPropertiesTypeDef",
     {
         "MemoryStoreRetentionPeriodInHours": int,
         "MagneticStoreRetentionPeriodInDays": int,
     },
 )
 
-CsvConfigurationOutputTypeDef = TypedDict(
-    "CsvConfigurationOutputTypeDef",
-    {
-        "ColumnSeparator": str,
-        "EscapeChar": str,
-        "QuoteChar": str,
-        "NullValue": str,
-        "TrimWhiteSpace": bool,
-    },
-    total=False,
-)
-
 CsvConfigurationTypeDef = TypedDict(
     "CsvConfigurationTypeDef",
     {
         "ColumnSeparator": str,
         "EscapeChar": str,
         "QuoteChar": str,
         "NullValue": str,
         "TrimWhiteSpace": bool,
     },
     total=False,
 )
 
-DataModelS3ConfigurationOutputTypeDef = TypedDict(
-    "DataModelS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKey": str,
-    },
-    total=False,
-)
-
 DataModelS3ConfigurationTypeDef = TypedDict(
     "DataModelS3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
-DimensionMappingOutputTypeDef = TypedDict(
-    "DimensionMappingOutputTypeDef",
-    {
-        "SourceColumn": str,
-        "DestinationColumn": str,
-    },
-    total=False,
-)
-
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "SourceColumn": str,
         "DestinationColumn": str,
     },
     total=False,
 )
 
-_RequiredDataSourceS3ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDataSourceS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalDataSourceS3ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDataSourceS3ConfigurationOutputTypeDef",
-    {
-        "ObjectKeyPrefix": str,
-    },
-    total=False,
-)
-
-
-class DataSourceS3ConfigurationOutputTypeDef(
-    _RequiredDataSourceS3ConfigurationOutputTypeDef, _OptionalDataSourceS3ConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredDataSourceS3ConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalDataSourceS3ConfigurationTypeDef = TypedDict(
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
-
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
-
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -346,19 +278,17 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
-
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
-
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -387,33 +317,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-S3ConfigurationOutputTypeDef = TypedDict(
-    "S3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKeyPrefix": str,
-        "EncryptionOption": S3EncryptionOptionType,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
 S3ConfigurationTypeDef = TypedDict(
     "S3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
@@ -426,37 +337,14 @@
     {
         "Name": str,
         "Value": str,
         "Type": MeasureValueTypeType,
     },
 )
 
-_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "SourceColumn": str,
-    },
-)
-_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "TargetMultiMeasureAttributeName": str,
-        "MeasureValueType": ScalarMeasureValueTypeType,
-    },
-    total=False,
-)
-
-
-class MultiMeasureAttributeMappingOutputTypeDef(
-    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
-    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
-):
-    pass
-
-
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
     },
 )
 _OptionalMultiMeasureAttributeMappingTypeDef = TypedDict(
@@ -464,43 +352,19 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-
-_RequiredPartitionKeyOutputTypeDef = TypedDict(
-    "_RequiredPartitionKeyOutputTypeDef",
-    {
-        "Type": PartitionKeyTypeType,
-    },
-)
-_OptionalPartitionKeyOutputTypeDef = TypedDict(
-    "_OptionalPartitionKeyOutputTypeDef",
-    {
-        "Name": str,
-        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
-    },
-    total=False,
-)
-
-
-class PartitionKeyOutputTypeDef(
-    _RequiredPartitionKeyOutputTypeDef, _OptionalPartitionKeyOutputTypeDef
-):
-    pass
-
-
 _RequiredPartitionKeyTypeDef = TypedDict(
     "_RequiredPartitionKeyTypeDef",
     {
         "Type": PartitionKeyTypeType,
     },
 )
 _OptionalPartitionKeyTypeDef = TypedDict(
@@ -508,52 +372,27 @@
     {
         "Name": str,
         "EnforcementInRecord": PartitionKeyEnforcementLevelType,
     },
     total=False,
 )
 
-
 class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
     pass
 
-
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
     total=False,
 )
 
-_RequiredReportS3ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredReportS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalReportS3ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalReportS3ConfigurationOutputTypeDef",
-    {
-        "ObjectKeyPrefix": str,
-        "EncryptionOption": S3EncryptionOptionType,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class ReportS3ConfigurationOutputTypeDef(
-    _RequiredReportS3ConfigurationOutputTypeDef, _OptionalReportS3ConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredReportS3ConfigurationTypeDef = TypedDict(
     "_RequiredReportS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalReportS3ConfigurationTypeDef = TypedDict(
@@ -562,36 +401,26 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
-
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
-RetentionPropertiesOutputTypeDef = TypedDict(
-    "RetentionPropertiesOutputTypeDef",
-    {
-        "MemoryStoreRetentionPeriodInHours": int,
-        "MagneticStoreRetentionPeriodInDays": int,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -639,20 +468,26 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -687,36 +522,14 @@
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDataSourceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigurationOutputTypeDef",
-    {
-        "DataSourceS3Configuration": DataSourceS3ConfigurationOutputTypeDef,
-        "DataFormat": Literal["CSV"],
-    },
-)
-_OptionalDataSourceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigurationOutputTypeDef",
-    {
-        "CsvConfiguration": CsvConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigurationOutputTypeDef(
-    _RequiredDataSourceConfigurationOutputTypeDef, _OptionalDataSourceConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
         "DataFormat": Literal["CSV"],
     },
 )
@@ -724,45 +537,27 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
-
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MagneticStoreRejectedDataLocationOutputTypeDef = TypedDict(
-    "MagneticStoreRejectedDataLocationOutputTypeDef",
-    {
-        "S3Configuration": S3ConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
@@ -790,47 +585,24 @@
 )
 _OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
     "_OptionalMixedMeasureMappingOutputTypeDef",
     {
         "MeasureName": str,
         "SourceColumn": str,
         "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingOutputTypeDef(
     _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
 ):
     pass
 
-
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
-
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -840,20 +612,37 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
 
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
@@ -861,25 +650,23 @@
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-
 SchemaOutputTypeDef = TypedDict(
     "SchemaOutputTypeDef",
     {
-        "CompositePartitionKey": List[PartitionKeyOutputTypeDef],
+        "CompositePartitionKey": List[PartitionKeyTypeDef],
     },
     total=False,
 )
 
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
@@ -892,73 +679,41 @@
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportConfigurationOutputTypeDef = TypedDict(
-    "ReportConfigurationOutputTypeDef",
-    {
-        "ReportS3Configuration": ReportS3ConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
-    "_RequiredMagneticStoreWritePropertiesOutputTypeDef",
-    {
-        "EnableMagneticStoreWrites": bool,
-    },
-)
-_OptionalMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
-    "_OptionalMagneticStoreWritePropertiesOutputTypeDef",
-    {
-        "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MagneticStoreWritePropertiesOutputTypeDef(
-    _RequiredMagneticStoreWritePropertiesOutputTypeDef,
-    _OptionalMagneticStoreWritePropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_RequiredMagneticStoreWritePropertiesTypeDef",
     {
         "EnableMagneticStoreWrites": bool,
     },
 )
 _OptionalMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
-
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
-
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -967,44 +722,40 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
-
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDataModelOutputTypeDef = TypedDict(
     "_RequiredDataModelOutputTypeDef",
     {
-        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+        "DimensionMappings": List[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelOutputTypeDef = TypedDict(
     "_OptionalDataModelOutputTypeDef",
     {
         "TimeColumn": str,
         "TimeUnit": TimeUnitType,
         "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
         "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
     pass
 
-
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -1015,35 +766,17 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
-
-TableTypeDef = TypedDict(
-    "TableTypeDef",
-    {
-        "Arn": str,
-        "TableName": str,
-        "DatabaseName": str,
-        "TableStatus": TableStatusType,
-        "RetentionProperties": RetentionPropertiesOutputTypeDef,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesOutputTypeDef,
-        "Schema": SchemaOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1054,20 +787,34 @@
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+TableTypeDef = TypedDict(
+    "TableTypeDef",
+    {
+        "Arn": str,
+        "TableName": str,
+        "DatabaseName": str,
+        "TableStatus": TableStatusType,
+        "RetentionProperties": RetentionPropertiesTypeDef,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+    total=False,
+)
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
@@ -1078,26 +825,24 @@
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-
 DataModelConfigurationOutputTypeDef = TypedDict(
     "DataModelConfigurationOutputTypeDef",
     {
         "DataModel": DataModelOutputTypeDef,
-        "DataModelS3Configuration": DataModelS3ConfigurationOutputTypeDef,
+        "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
 )
 
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
@@ -1141,17 +886,17 @@
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
-        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
+        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
-        "ReportConfiguration": ReportConfigurationOutputTypeDef,
+        "ReportConfiguration": ReportConfigurationTypeDef,
         "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
@@ -1175,22 +920,20 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
-
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.pyi` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,87 +31,74 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
-    "CsvConfigurationOutputTypeDef",
     "CsvConfigurationTypeDef",
-    "DataModelS3ConfigurationOutputTypeDef",
     "DataModelS3ConfigurationTypeDef",
-    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
-    "DataSourceS3ConfigurationOutputTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
-    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
-    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
-    "ReportS3ConfigurationOutputTypeDef",
     "ReportS3ConfigurationTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
-    "RetentionPropertiesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "CreateBatchLoadTaskResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
-    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MagneticStoreRejectedDataLocationOutputTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
     "MixedMeasureMappingOutputTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
-    "ReportConfigurationOutputTypeDef",
     "ReportConfigurationTypeDef",
-    "MagneticStoreWritePropertiesOutputTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelOutputTypeDef",
     "DataModelTypeDef",
-    "TableTypeDef",
     "CreateTableRequestRequestTypeDef",
+    "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
@@ -183,112 +170,65 @@
     "RetentionPropertiesTypeDef",
     {
         "MemoryStoreRetentionPeriodInHours": int,
         "MagneticStoreRetentionPeriodInDays": int,
     },
 )
 
-CsvConfigurationOutputTypeDef = TypedDict(
-    "CsvConfigurationOutputTypeDef",
-    {
-        "ColumnSeparator": str,
-        "EscapeChar": str,
-        "QuoteChar": str,
-        "NullValue": str,
-        "TrimWhiteSpace": bool,
-    },
-    total=False,
-)
-
 CsvConfigurationTypeDef = TypedDict(
     "CsvConfigurationTypeDef",
     {
         "ColumnSeparator": str,
         "EscapeChar": str,
         "QuoteChar": str,
         "NullValue": str,
         "TrimWhiteSpace": bool,
     },
     total=False,
 )
 
-DataModelS3ConfigurationOutputTypeDef = TypedDict(
-    "DataModelS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKey": str,
-    },
-    total=False,
-)
-
 DataModelS3ConfigurationTypeDef = TypedDict(
     "DataModelS3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
-DimensionMappingOutputTypeDef = TypedDict(
-    "DimensionMappingOutputTypeDef",
-    {
-        "SourceColumn": str,
-        "DestinationColumn": str,
-    },
-    total=False,
-)
-
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "SourceColumn": str,
         "DestinationColumn": str,
     },
     total=False,
 )
 
-_RequiredDataSourceS3ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDataSourceS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalDataSourceS3ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDataSourceS3ConfigurationOutputTypeDef",
-    {
-        "ObjectKeyPrefix": str,
-    },
-    total=False,
-)
-
-class DataSourceS3ConfigurationOutputTypeDef(
-    _RequiredDataSourceS3ConfigurationOutputTypeDef, _OptionalDataSourceS3ConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredDataSourceS3ConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalDataSourceS3ConfigurationTypeDef = TypedDict(
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
+
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
+
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -341,17 +281,19 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
+
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
+
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -380,33 +322,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-S3ConfigurationOutputTypeDef = TypedDict(
-    "S3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKeyPrefix": str,
-        "EncryptionOption": S3EncryptionOptionType,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
 S3ConfigurationTypeDef = TypedDict(
     "S3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
@@ -419,35 +342,14 @@
     {
         "Name": str,
         "Value": str,
         "Type": MeasureValueTypeType,
     },
 )
 
-_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "SourceColumn": str,
-    },
-)
-_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "TargetMultiMeasureAttributeName": str,
-        "MeasureValueType": ScalarMeasureValueTypeType,
-    },
-    total=False,
-)
-
-class MultiMeasureAttributeMappingOutputTypeDef(
-    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
-    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
-):
-    pass
-
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
     },
 )
 _OptionalMultiMeasureAttributeMappingTypeDef = TypedDict(
@@ -455,38 +357,20 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-_RequiredPartitionKeyOutputTypeDef = TypedDict(
-    "_RequiredPartitionKeyOutputTypeDef",
-    {
-        "Type": PartitionKeyTypeType,
-    },
-)
-_OptionalPartitionKeyOutputTypeDef = TypedDict(
-    "_OptionalPartitionKeyOutputTypeDef",
-    {
-        "Name": str,
-        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
-    },
-    total=False,
-)
-
-class PartitionKeyOutputTypeDef(
-    _RequiredPartitionKeyOutputTypeDef, _OptionalPartitionKeyOutputTypeDef
-):
-    pass
 
 _RequiredPartitionKeyTypeDef = TypedDict(
     "_RequiredPartitionKeyTypeDef",
     {
         "Type": PartitionKeyTypeType,
     },
 )
@@ -495,48 +379,29 @@
     {
         "Name": str,
         "EnforcementInRecord": PartitionKeyEnforcementLevelType,
     },
     total=False,
 )
 
+
 class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
     pass
 
+
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
     total=False,
 )
 
-_RequiredReportS3ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredReportS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalReportS3ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalReportS3ConfigurationOutputTypeDef",
-    {
-        "ObjectKeyPrefix": str,
-        "EncryptionOption": S3EncryptionOptionType,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class ReportS3ConfigurationOutputTypeDef(
-    _RequiredReportS3ConfigurationOutputTypeDef, _OptionalReportS3ConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredReportS3ConfigurationTypeDef = TypedDict(
     "_RequiredReportS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalReportS3ConfigurationTypeDef = TypedDict(
@@ -545,34 +410,28 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
+
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
-RetentionPropertiesOutputTypeDef = TypedDict(
-    "RetentionPropertiesOutputTypeDef",
-    {
-        "MemoryStoreRetentionPeriodInHours": int,
-        "MagneticStoreRetentionPeriodInDays": int,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -620,19 +479,29 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
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
@@ -666,34 +535,14 @@
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDataSourceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigurationOutputTypeDef",
-    {
-        "DataSourceS3Configuration": DataSourceS3ConfigurationOutputTypeDef,
-        "DataFormat": Literal["CSV"],
-    },
-)
-_OptionalDataSourceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigurationOutputTypeDef",
-    {
-        "CsvConfiguration": CsvConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class DataSourceConfigurationOutputTypeDef(
-    _RequiredDataSourceConfigurationOutputTypeDef, _OptionalDataSourceConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
         "DataFormat": Literal["CSV"],
     },
 )
@@ -701,43 +550,29 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MagneticStoreRejectedDataLocationOutputTypeDef = TypedDict(
-    "MagneticStoreRejectedDataLocationOutputTypeDef",
-    {
-        "S3Configuration": S3ConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
@@ -765,42 +600,25 @@
 )
 _OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
     "_OptionalMixedMeasureMappingOutputTypeDef",
     {
         "MeasureName": str,
         "SourceColumn": str,
         "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingOutputTypeDef(
     _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
 ):
     pass
 
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
 
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
@@ -811,42 +629,67 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+
 SchemaOutputTypeDef = TypedDict(
     "SchemaOutputTypeDef",
     {
-        "CompositePartitionKey": List[PartitionKeyOutputTypeDef],
+        "CompositePartitionKey": List[PartitionKeyTypeDef],
     },
     total=False,
 )
 
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
@@ -859,69 +702,43 @@
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportConfigurationOutputTypeDef = TypedDict(
-    "ReportConfigurationOutputTypeDef",
-    {
-        "ReportS3Configuration": ReportS3ConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
-    "_RequiredMagneticStoreWritePropertiesOutputTypeDef",
-    {
-        "EnableMagneticStoreWrites": bool,
-    },
-)
-_OptionalMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
-    "_OptionalMagneticStoreWritePropertiesOutputTypeDef",
-    {
-        "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationOutputTypeDef,
-    },
-    total=False,
-)
-
-class MagneticStoreWritePropertiesOutputTypeDef(
-    _RequiredMagneticStoreWritePropertiesOutputTypeDef,
-    _OptionalMagneticStoreWritePropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_RequiredMagneticStoreWritePropertiesTypeDef",
     {
         "EnableMagneticStoreWrites": bool,
     },
 )
 _OptionalMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
+
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
+
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -930,40 +747,44 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
+
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDataModelOutputTypeDef = TypedDict(
     "_RequiredDataModelOutputTypeDef",
     {
-        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+        "DimensionMappings": List[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelOutputTypeDef = TypedDict(
     "_OptionalDataModelOutputTypeDef",
     {
         "TimeColumn": str,
         "TimeUnit": TimeUnitType,
         "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
         "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
     pass
 
+
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -974,32 +795,18 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
-TableTypeDef = TypedDict(
-    "TableTypeDef",
-    {
-        "Arn": str,
-        "TableName": str,
-        "DatabaseName": str,
-        "TableStatus": TableStatusType,
-        "RetentionProperties": RetentionPropertiesOutputTypeDef,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesOutputTypeDef,
-        "Schema": SchemaOutputTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
@@ -1011,19 +818,37 @@
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+
+TableTypeDef = TypedDict(
+    "TableTypeDef",
+    {
+        "Arn": str,
+        "TableName": str,
+        "DatabaseName": str,
+        "TableStatus": TableStatusType,
+        "RetentionProperties": RetentionPropertiesTypeDef,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1033,24 +858,26 @@
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+
 DataModelConfigurationOutputTypeDef = TypedDict(
     "DataModelConfigurationOutputTypeDef",
     {
         "DataModel": DataModelOutputTypeDef,
-        "DataModelS3Configuration": DataModelS3ConfigurationOutputTypeDef,
+        "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
 )
 
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
@@ -1094,17 +921,17 @@
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
-        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
+        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
-        "ReportConfiguration": ReportConfigurationOutputTypeDef,
+        "ReportConfiguration": ReportConfigurationTypeDef,
         "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
@@ -1128,20 +955,22 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
+
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/PKG-INFO` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.12
-Summary: Type annotations for boto3.TimestreamWrite 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,80 +313,66 @@
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
-    CsvConfigurationOutputTypeDef,
     CsvConfigurationTypeDef,
-    DataModelS3ConfigurationOutputTypeDef,
     DataModelS3ConfigurationTypeDef,
-    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    DataSourceS3ConfigurationOutputTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
-    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
-    ReportS3ConfigurationOutputTypeDef,
     ReportS3ConfigurationTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
-    RetentionPropertiesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     CreateBatchLoadTaskResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
-    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MagneticStoreRejectedDataLocationOutputTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingOutputTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
-    ReportConfigurationOutputTypeDef,
     ReportConfigurationTypeDef,
-    MagneticStoreWritePropertiesOutputTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelOutputTypeDef,
     DataModelTypeDef,
-    TableTypeDef,
     CreateTableRequestRequestTypeDef,
+    TableTypeDef,
     UpdateTableRequestRequestTypeDef,
     DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
```

### Comparing `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/SOURCES.txt` & `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.12/setup.py` & `mypy-boto3-timestream-write-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-write",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamWrite 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.TimestreamWrite 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

