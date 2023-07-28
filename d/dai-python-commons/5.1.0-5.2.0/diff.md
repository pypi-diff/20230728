# Comparing `tmp/dai_python_commons-5.1.0.tar.gz` & `tmp/dai_python_commons-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dai_python_commons-5.1.0.tar", max compression
+gzip compressed data, was "dai_python_commons-5.2.0.tar", max compression
```

## Comparing `dai_python_commons-5.1.0.tar` & `dai_python_commons-5.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      108 2023-07-20 09:05:56.938902 dai_python_commons-5.1.0/dai_python_commons/__init__.py
--rw-r--r--   0        0        0     1521 2023-07-20 09:05:56.938902 dai_python_commons-5.1.0/dai_python_commons/cdk_utils.py
--rw-r--r--   0        0        0     1372 2023-07-20 09:05:56.938902 dai_python_commons-5.1.0/dai_python_commons/cloudwatch_utils.py
--rw-r--r--   0        0        0     4421 2023-07-20 09:05:56.938902 dai_python_commons-5.1.0/dai_python_commons/dai_error.py
--rw-r--r--   0        0        0     2390 2023-07-20 09:05:56.938902 dai_python_commons-5.1.0/dai_python_commons/event_bridge.py
--rw-r--r--   0        0        0     5314 2023-07-20 09:05:56.938902 dai_python_commons-5.1.0/dai_python_commons/glue_utils.py
--rw-r--r--   0        0        0     1742 2023-07-20 09:05:56.942902 dai_python_commons-5.1.0/dai_python_commons/logging_utils.py
--rw-r--r--   0        0        0    10471 2023-07-20 09:05:56.942902 dai_python_commons-5.1.0/dai_python_commons/parquet_utils.py
--rw-r--r--   0        0        0    24224 2023-07-20 09:05:56.942902 dai_python_commons-5.1.0/dai_python_commons/s3_event_object_copy.py
--rw-r--r--   0        0        0     7973 2023-07-20 09:05:56.942902 dai_python_commons-5.1.0/dai_python_commons/s3_utils.py
--rw-r--r--   0        0        0     2391 2023-07-20 09:05:56.942902 dai_python_commons-5.1.0/dai_python_commons/time_utils.py
--rw-r--r--   0        0        0      995 2023-07-20 09:05:56.942902 dai_python_commons-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 dai_python_commons-5.1.0/setup.py
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 dai_python_commons-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/__init__.py
+-rw-r--r--   0        0        0     1521 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/cdk_utils.py
+-rw-r--r--   0        0        0     1372 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/cloudwatch_utils.py
+-rw-r--r--   0        0        0     4421 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/dai_error.py
+-rw-r--r--   0        0        0     2390 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/event_bridge.py
+-rw-r--r--   0        0        0     5314 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/glue_utils.py
+-rw-r--r--   0        0        0     1742 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/logging_utils.py
+-rw-r--r--   0        0        0    11212 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/parquet_utils.py
+-rw-r--r--   0        0        0    24224 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/s3_event_object_copy.py
+-rw-r--r--   0        0        0     7973 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/s3_utils.py
+-rw-r--r--   0        0        0     2391 2023-07-28 06:56:05.411933 dai_python_commons-5.2.0/dai_python_commons/time_utils.py
+-rw-r--r--   0        0        0      872 2023-07-28 06:56:05.415933 dai_python_commons-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 dai_python_commons-5.2.0/setup.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 dai_python_commons-5.2.0/PKG-INFO
```

### Comparing `dai_python_commons-5.1.0/dai_python_commons/cdk_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/cdk_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/cloudwatch_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/cloudwatch_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/dai_error.py` & `dai_python_commons-5.2.0/dai_python_commons/dai_error.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/event_bridge.py` & `dai_python_commons-5.2.0/dai_python_commons/event_bridge.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/glue_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/glue_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/logging_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/parquet_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/parquet_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Functionality to modify parquet files in an S3 bucket"""
 from __future__ import annotations
 
 import gc
+import io
+import os
 from dataclasses import dataclass
 from typing import Optional
-from aiobotocore.session import AioSession
 
 import boto3
 import loguru
-import pyarrow.parquet as pq
-import s3fs
+import polars as pl
 
 from dai_python_commons.s3_utils import S3Utils
 
 
 @dataclass
 class ParquetFileLocation:
     """
@@ -44,84 +44,92 @@
     total_files_size: int = 1024 * 1024 * 1024   # 1GB
 
 
 class ParquetUtils:
     """
     Class that provides functionality for manipulating parquet files
     """
-    # pylint: disable=no-member
-    VALID_COMPRESSION_TYPES = {'NONE', 'SNAPPY', 'GZIP', 'BROTLI', 'LZ4', 'ZSTD'}
+    # pylint: disable=no-member,too-many-locals
+    VALID_COMPRESSION_TYPES = {'none', 'snappy', 'gzip', 'lz4', 'zstd'}
 
     @staticmethod
     def s3_merge_files_in_place(boto3_session: boto3.Session,
                                 parquet_file_location: ParquetFileLocation,
                                 logger: loguru.Logger,
-                                compression: Optional[str] = "SNAPPY",
+                                compression: str = "snappy",
                                 keep_source_files: bool = False) -> int:
         """
          Merge many small parquet files into one larger parquet file. In place.
 
         :param boto3_session: Boto3 session
         :param parquet_file_location: s3 bucket and prefix location where parquet files will be merged
         :param logger: The logger
-        :param compression: Type of compression. Accepted values are 'NONE', 'SNAPPY', 'GZIP', 'BROTLI', 'LZ4', 'ZSTD'
+        :param compression: Type of compression. Accepted values are 'none', 'snappy', 'gzip', 'brotli', 'lz4', 'zstd'
         :param keep_source_files: True to keep the source files, False to delete them.
         :return:
         """
         data_path = f"s3://{parquet_file_location.source_bucket}/{parquet_file_location.source_prefix}"
         logger.info(f"Merging files from {data_path} to {data_path}, compression: {compression}")
 
-        # this is a bit of hack, one should probably find a better way to do this
-        botoc_session = boto3_session._session # pylint: disable=protected-access
-        aio_session = AioSession(session_vars=botoc_session.session_var_map)
-        f_s = s3fs.S3FileSystem(session=aio_session)
-
         boto_s3_client = boto3_session.client("s3")
         num_rows = 0
 
         file_paths_iter = S3Utils.iter_file_paths_in_prefix(boto_s3_client=boto_s3_client,
                                                   bucket_name=parquet_file_location.source_bucket,
                                                   prefix=parquet_file_location.source_prefix,
                                                   logger=logger,
                                                   max_size=parquet_file_location.total_files_size)
         for file_paths in file_paths_iter:
             if len(file_paths) <2:
                 logger.info(f"file paths is less than 2 files, no reason to merge: {file_paths}")
                 continue
             logger.info(f"Reading and merging {file_paths}")
 
-            full_s3_paths = [f's3://{parquet_file_location.source_bucket}/{file_path["Key"]}' for file_path in file_paths]
+            file_bytes = []
+            for file_path in file_paths:
+                file = S3Utils.read_s3_file(
+                    s3_client=boto_s3_client,
+                    bucket_name=parquet_file_location.source_bucket,
+                    key=file_path["Key"]
+                ).read()
+                file_bytes.append(io.BytesIO(file))
+
+            merged_data = pl.read_parquet(file_bytes.pop(0))
+            merged_data = merged_data.select(sorted(merged_data.columns))
+            for file in file_bytes:
+                new_frame = pl.read_parquet(file)
+                merged_data.vstack(new_frame.select(sorted(merged_data.columns)), in_place=True)
 
-            # partitioning=None ensures we do not add a column dt when parsing
-            # our parquet files that usually have a "hive-like" partitioned dt
-            # path, which we do not wish to add to the set when consolidating.
-            # The type in the interface is wrong, source code does handle the None
-            pq_table = pq.read_table(full_s3_paths, filesystem=f_s, partitioning=None)  # type: ignore
-            num_rows += pq_table.num_rows
-            logger.debug(f"Shape of the table {pq_table.shape}")
+            num_rows += merged_data.height
+            logger.debug(f"Shape of the table {merged_data.shape}")
 
             logger.debug(f"Writing to the destination {data_path}")
             try:
-                pq.write_to_dataset(pq_table, data_path, filesystem=f_s, compression=compression)
-                logger.info(f"Done merging, {pq_table.num_rows} rows were written at {data_path}")
+                with io.BytesIO() as con:
+                    merged_data.write_parquet(con, compression=compression.lower())
+
+                    key=os.path.join(parquet_file_location.source_prefix, f"consolidated_rows_{num_rows}.parquet")
+                    boto_s3_client.put_object(Body=con.getvalue(), Bucket=parquet_file_location.source_bucket,Key=key)
+
+                logger.info(f"Done merging, {merged_data.height} rows were written at prefix {data_path}")
                 if not keep_source_files:
                     logger.info('Removing source files')
                     logger.debug(f'Removing these files {file_paths}')
                     S3Utils.delete_objects(
                         boto_s3_client=boto_s3_client,
                         bucket_name=parquet_file_location.source_bucket,
                         to_delete=file_paths,
                         logger=logger
                     )
             except Exception:
                 logger.exception(f'Caught error when trying to merge parquet files: {file_paths}')
                 raise
 
             # Explicitly clear data from memory
-            del pq_table
+            del merged_data
             gc.collect()
 
         if num_rows == 0:
             logger.warning(f"No files found at {data_path}, nothing to merge")
 
         return num_rows
 
@@ -160,45 +168,66 @@
             logger.warning(f"No files found at {source_data_path}, nothing to merge")
             return 0
 
         if remove_files_at_destination:
             ParquetUtils._remove_files(parquet_file_location, destination_data_path, logger, s3_client)
 
         logger.debug(f"Reading data from {source_data_path}")
-        # this is a bit of hack, one should probably find a better way to do this
-        botoc_session = boto3_session._session  # pylint: disable=protected-access
-        aio_session = AioSession(session_vars=botoc_session.session_var_map) # type: ignore
-        f_s = s3fs.S3FileSystem(session=aio_session)
-        full_s3_paths = [f's3://{source_bucket}/{file_path["Key"]}' for file_path in file_paths]
-        pq_table = pq.read_table(full_s3_paths, filesystem=f_s, partitioning=None) # type: ignore
+
+        file_paths = S3Utils.file_paths_in_prefix(boto_s3_client=s3_client,
+                                                  bucket_name=parquet_file_location.source_bucket,
+                                                  prefix=parquet_file_location.source_prefix,
+                                                  logger=logger)
+
+        files = []
+        for file_path in file_paths:
+            file = S3Utils.read_s3_file(
+                s3_client=s3_client,
+                bucket_name=parquet_file_location.source_bucket,
+                key=file_path["Key"]
+            ).read()
+            files.append(io.BytesIO(file))
+
+        pq_table = pl.read_parquet(files.pop(0))
+        pq_table = pq_table.select(sorted(pq_table.columns))
+        for file in files:
+            new_frame = pl.read_parquet(file)
+            pq_table.vstack(new_frame.select(sorted(pq_table.columns)), in_place=True)
+
         logger.debug(f"Shape of the table {pq_table.shape}")
 
+        compression = parquet_file_location.compression
+        if compression:
+            compression = compression.lower()
+        else:
+            compression = "none"
+
         try:
             logger.debug(f"Writing to the destination {destination_data_path}")
-            pq.write_to_dataset(pq_table,
-                                destination_data_path,
-                                filesystem=f_s,
-                                compression=parquet_file_location.compression
-            )
+            with io.BytesIO() as con:
+                pq_table.write_parquet(con, compression=compression)
+
+                key=os.path.join(parquet_file_location.destination_prefix, f"consolidated_entries_{pq_table.height}.parquet")
+                s3_client.put_object(Body=con.getvalue(), Bucket=parquet_file_location.destination_bucket,Key=key)
 
-            logger.info(f"Done merging, {pq_table.num_rows} rows were written at {destination_data_path}")
+            logger.info(f"Done merging, {pq_table.height} rows were written at {destination_data_path}")
             if not parquet_file_location.keep_source_files:
                 logger.info('Removing source files')
                 logger.debug(f'Removing these files {file_paths}')
                 S3Utils.delete_objects(
                     boto_s3_client=s3_client,
                     bucket_name=source_bucket,
                     to_delete=file_paths,
                     logger=logger
                 )
         except Exception:
             logger.exception(f'Caught error when trying to merge parquet files: {file_paths}')
             raise
 
-        return pq_table.num_rows
+        return pq_table.height
 
     @staticmethod
     def _remove_files(parquet_file_location, destination_data_path, logger, s3_client):
         """removes files at the destination bucket, assigned in the parquet_file_location"""
         logger.debug(f"Removing all files at {destination_data_path}")
         S3Utils.delete_objects_by_prefix(boto_s3_client=s3_client, bucket_name=parquet_file_location.destination_bucket,
                                          prefix=parquet_file_location.destination_prefix, logger=logger)
```

### Comparing `dai_python_commons-5.1.0/dai_python_commons/s3_event_object_copy.py` & `dai_python_commons-5.2.0/dai_python_commons/s3_event_object_copy.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/s3_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/dai_python_commons/time_utils.py` & `dai_python_commons-5.2.0/dai_python_commons/time_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.1.0/pyproject.toml` & `dai_python_commons-5.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "dai-python-commons"
-version = "5.1.0"
+version = "5.2.0"
 description = "Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration."
 authors = []
 
 [tool.poetry.dependencies]
 python = "~3.10"
 loguru = "^0.7.0"
 boto3 = "^1.26.0"
-pyarrow = { version = "12.0.0", optional = true }
-s3fs = { version = "2023.6.0", optional = true }
+polars = { version = "0.18.8", optional = true }
 awswrangler = { version = "3.2.1", optional = true }
 boto3-stubs = { version = "^1.26.0", extras = ["s3", "glue"] }
 cryptography = { version = "41.0.2", optional = true }
-aiobotocore = { version="2.5.2", optional=true }
 
 [tool.poetry.dev-dependencies]
 pytest = "7.4"
 moto = { version = "4.1.13", extras = ["s3", "glue"] }
 pylint = "2.17.4"
 
 
 [tool.poetry.extras]
-data-consolidation = ["s3fs", "pyarrow", "aiobotocore"]
+data-consolidation = ["polars"]
 glue = ["awswrangler", "cryptography"]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dai_python_commons-5.1.0/setup.py` & `dai_python_commons-5.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 
 install_requires = \
 ['boto3-stubs[glue,s3]>=1.26.0,<2.0.0',
  'boto3>=1.26.0,<2.0.0',
  'loguru>=0.7.0,<0.8.0']
 
 extras_require = \
-{'data-consolidation': ['pyarrow==12.0.0',
-                        's3fs==2023.6.0',
-                        'aiobotocore==2.5.2'],
+{'data-consolidation': ['polars==0.18.8'],
  'glue': ['awswrangler==3.2.1', 'cryptography==41.0.2']}
 
 setup_kwargs = {
     'name': 'dai-python-commons',
-    'version': '5.1.0',
+    'version': '5.2.0',
     'description': 'Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.',
     'long_description': 'None',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dai_python_commons-5.1.0/PKG-INFO` & `dai_python_commons-5.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dai-python-commons
-Version: 5.1.0
+Version: 5.2.0
 Summary: Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: data-consolidation
 Provides-Extra: glue
-Requires-Dist: aiobotocore (==2.5.2); extra == "data-consolidation"
 Requires-Dist: awswrangler (==3.2.1); extra == "glue"
 Requires-Dist: boto3 (>=1.26.0,<2.0.0)
 Requires-Dist: boto3-stubs[glue,s3] (>=1.26.0,<2.0.0)
 Requires-Dist: cryptography (==41.0.2); extra == "glue"
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pyarrow (==12.0.0); extra == "data-consolidation"
-Requires-Dist: s3fs (==2023.6.0); extra == "data-consolidation"
+Requires-Dist: polars (==0.18.8); extra == "data-consolidation"
```

