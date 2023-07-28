# Comparing `tmp/serra-0.2.tar.gz` & `tmp/serra-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.2.tar", last modified: Fri Jul 28 19:51:57 2023, max compression
+gzip compressed data, was "serra-0.3.tar", last modified: Fri Jul 28 19:54:00 2023, max compression
```

## Comparing `serra-0.2.tar` & `serra-0.3.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.153263 serra-0.2/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-21 18:21:51.000000 serra-0.2/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-28 19:51:57.153128 serra-0.2/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     1618 2023-07-21 20:21:47.000000 serra-0.2/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.148530 serra-0.2/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.2/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      989 2023-07-28 01:15:14.000000 serra-0.2/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1501 2023-07-28 01:15:14.000000 serra-0.2/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      438 2023-07-28 01:15:14.000000 serra-0.2/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1887 2023-07-27 07:28:06.000000 serra-0.2/serra/config_parser.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2609 2023-07-28 01:15:14.000000 serra-0.2/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-27 07:28:06.000000 serra-0.2/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)      921 2023-07-28 01:15:14.000000 serra-0.2/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.150194 serra-0.2/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      185 2023-07-21 18:21:51.000000 serra-0.2/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1456 2023-07-28 01:15:14.000000 serra-0.2/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-27 07:28:06.000000 serra-0.2/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      487 2023-07-27 07:28:06.000000 serra-0.2/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-27 07:28:06.000000 serra-0.2/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-21 18:21:51.000000 serra-0.2/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2858 2023-07-28 06:09:36.000000 serra-0.2/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.150507 serra-0.2/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-21 18:21:51.000000 serra-0.2/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.2/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3262 2023-07-28 01:32:22.000000 serra-0.2/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      442 2023-07-28 01:15:14.000000 serra-0.2/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.152168 serra-0.2/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-25 20:52:34.000000 serra-0.2/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-27 07:28:06.000000 serra-0.2/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-21 18:21:51.000000 serra-0.2/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      462 2023-07-28 05:46:49.000000 serra-0.2/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-28 19:27:42.000000 serra-0.2/serra/transformers/conversion_to_usd_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-21 18:21:51.000000 serra-0.2/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-21 18:21:51.000000 serra-0.2/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1807 2023-07-28 06:02:24.000000 serra-0.2/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1820 2023-07-27 07:28:06.000000 serra-0.2/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-27 07:28:06.000000 serra-0.2/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-21 18:21:51.000000 serra-0.2/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1090 2023-07-27 07:28:06.000000 serra-0.2/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-21 18:21:51.000000 serra-0.2/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)    15497 2023-07-28 05:41:24.000000 serra-0.2/serra/translate.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1239 2023-07-28 01:15:14.000000 serra-0.2/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.152929 serra-0.2/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      186 2023-07-21 18:21:51.000000 serra-0.2/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-28 01:15:14.000000 serra-0.2/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      677 2023-07-21 18:21:51.000000 serra-0.2/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-27 07:28:06.000000 serra-0.2/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      568 2023-07-21 18:21:51.000000 serra-0.2/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-27 07:28:06.000000 serra-0.2/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:51:57.149422 serra-0.2/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-28 19:51:57.000000 serra-0.2/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     1419 2023-07-28 19:51:57.000000 serra-0.2/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-28 19:51:57.000000 serra-0.2/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-28 19:51:57.000000 serra-0.2/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-21 20:20:18.000000 serra-0.2/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       62 2023-07-28 19:51:57.000000 serra-0.2/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-28 19:51:57.000000 serra-0.2/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-28 19:51:57.153304 serra-0.2/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      649 2023-07-28 19:51:28.000000 serra-0.2/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.697853 serra-0.3/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-21 18:21:51.000000 serra-0.3/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-28 19:54:00.697715 serra-0.3/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     1511 2023-07-28 19:53:46.000000 serra-0.3/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.693059 serra-0.3/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.3/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1315 2023-07-28 19:53:46.000000 serra-0.3/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1501 2023-07-28 01:15:14.000000 serra-0.3/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-28 19:53:46.000000 serra-0.3/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1883 2023-07-28 19:53:46.000000 serra-0.3/serra/config_parser.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2963 2023-07-28 19:53:46.000000 serra-0.3/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-27 07:28:06.000000 serra-0.3/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1025 2023-07-28 19:53:46.000000 serra-0.3/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.695026 serra-0.3/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      185 2023-07-21 18:21:51.000000 serra-0.3/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1456 2023-07-28 01:15:14.000000 serra-0.3/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-27 07:28:06.000000 serra-0.3/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      487 2023-07-27 07:28:06.000000 serra-0.3/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-27 07:28:06.000000 serra-0.3/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-21 18:21:51.000000 serra-0.3/serra/readers/s3_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2975 2023-07-28 19:53:46.000000 serra-0.3/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.695325 serra-0.3/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-21 18:21:51.000000 serra-0.3/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.3/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3183 2023-07-28 19:53:46.000000 serra-0.3/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      442 2023-07-28 01:15:14.000000 serra-0.3/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.696839 serra-0.3/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-25 20:52:34.000000 serra-0.3/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-28 19:53:46.000000 serra-0.3/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1385 2023-07-28 19:53:46.000000 serra-0.3/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1820 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1090 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1189 2023-07-28 19:53:46.000000 serra-0.3/serra/translate_client.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1239 2023-07-28 01:15:14.000000 serra-0.3/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.697518 serra-0.3/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      186 2023-07-21 18:21:51.000000 serra-0.3/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-28 01:15:14.000000 serra-0.3/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      677 2023-07-21 18:21:51.000000 serra-0.3/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-27 07:28:06.000000 serra-0.3/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      568 2023-07-21 18:21:51.000000 serra-0.3/serra/writers/s3_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-27 07:28:06.000000 serra-0.3/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.694301 serra-0.3/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     1374 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-21 20:20:18.000000 serra-0.3/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       62 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-28 19:54:00.697895 serra-0.3/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      649 2023-07-28 19:53:57.000000 serra-0.3/setup.py
```

### Comparing `serra-0.2/LICENSE.md` & `serra-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.2/README.md` & `serra-0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Serra
-Object-Oriented Spark Framework for Data Transformations
+Translate SQL to Object-Oriented Spark
 
-# Setup for running
+# Setup
 
 ```bash
 python3.10 -m venv env
 source env/bin/activate
 pip install -r requirements.txt
 pip install -e .
 ```
 
-# May also need to follow these steps (Download and install spark)
-https://spark.apache.org/docs/latest/api/python/getting_started/install.html#manually-downloading
+# Getting Started
+Navigate to the workspace_example folder and try out a couple of jobs!
+
+```bash
+serra run LocalExample
+```
+Other jobs available can be found in the **workspace_example/jobs** folder.
 
 # Development Guide
 
 ## If you make changes to the package ( not just a new config)
 
 ### Step 1: Create wheel
 ```bash
@@ -44,32 +49,25 @@
 
 ### Step 2: Configure w/ DB cluster
 ```bash
 databricks-connect configure
 ```
 * Fill out the credentials as so:
 ```
-DB Workspace: https://dbc-b854a7df-4e5e.cloud.databricks.com
-DB Token: dapiaca3916d64c45c3b454fd6bb0e5a20c3
-cluster_id: 0630-194840-lj2a32jr
+DB Workspace: https://your-workspace.cloud.databricks.com
+DB Token: your_token
+cluster_id: your_cluster_id
 ```
 
 ### Step 3: Confirm connection
 * To test if your connection is setup
 ```bash
 databricks-connect test
 ```
 
 * All local spark sessions can now read from DB ie
 ```python
 from pyspark.sql.session import SparkSession
 
 spark = SparkSession.builder.getOrCreate()
 spark.sql("SELECT * FROM demo.sales_by_store")
-```
-
-
-# Run the flask server
-```bash
-source python3 -m venv env
-python3 app.py
 ```
```

### Comparing `serra-0.2/serra/cli.py` & `serra-0.3/serra/cli.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/config_parser.py` & `serra-0.3/serra/config_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # In case we ever want to change use of yaml file
 import yaml
-from serra.aws import retrieve_file_as_bytes_from_bucket
+from serra.aws import retrieve_file_from_config_bucket
 
 
 def convert_name_to_full(class_name):
     if "Reader" in class_name:
         return f"serra.readers.{class_name}"
     elif "Writer" in class_name:
         return f"serra.writers.{class_name}"
@@ -22,15 +22,15 @@
             config = yaml.safe_load(stream)
         return ConfigParser(config)
     
     @staticmethod
     def from_s3_config(config_name):
         # TODO: Make more generalizable
         # Currenltly 
-        config_bytes = retrieve_file_as_bytes_from_bucket(config_name)
+        config_bytes = retrieve_file_from_config_bucket(config_name)
         config = yaml.safe_load(config_bytes)
         return ConfigParser(config)
     
     def get_step(self, block_name):
         return self.config.get(block_name)
     
     def get_class_name_for_step(self, block_name):
```

### Comparing `serra-0.2/serra/databricks.py` & `serra-0.3/serra/databricks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,85 @@
 # Module to help connect to databricks
 from loguru import logger
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.service.jobs import Task, PythonWheelTask
 from databricks.sdk.service.compute import Library, State
-from serra.aws import upload_file_to_bucket
+from serra.aws import upload_file_to_config_bucket
 from serra.utils import get_path_to_user_configs_folder
 from serra.profile import get_serra_profile
 from serra.config import (
-    PATH_TO_WHEEL,
-    S3_WHEEL_PATH
+    WHEEL_FILE_NAME_IN_BUCKET,
+    LOCAL_PATH_TO_WHEEL
 )
 
+def get_remote_path_to_wheel():
+    serra_profile = get_serra_profile()
+    bucket = serra_profile.aws_config_bucket
+    s3_wheel_path = f"s3://{bucket}/{WHEEL_FILE_NAME_IN_BUCKET}"
+    return s3_wheel_path
+
 def create_databricks_workspace_client():
     serra_profile = get_serra_profile()
     w = WorkspaceClient(
         host  = serra_profile.databricks_host,
         token = serra_profile.databricks_token
     )
     return w
 
 def upload_wheel_to_bucket():
     # TODO: Add code to recreate wheel
-    logger.info(f"Uploading wheel from {PATH_TO_WHEEL} to AWS")
-    upload_file_to_bucket(PATH_TO_WHEEL)
+    logger.info(f"Uploading wheel from {LOCAL_PATH_TO_WHEEL} to AWS")
+    upload_file_to_config_bucket(LOCAL_PATH_TO_WHEEL)
 
 def create_job(config_name):
     """Use like this: submit_job("StripeExample")
     """
     serra_profile = get_serra_profile()
+    s3_wheel_path = get_remote_path_to_wheel()
+
     w = create_databricks_workspace_client()
 
     # Upload the config file to aws
     logger.info("Uploading config to AWS")
     config_path = f"{get_path_to_user_configs_folder()}/{config_name}.yml"
-    upload_file_to_bucket(config_path)
+    upload_file_to_config_bucket(config_path)
     
     # Create the job on databricks
     logger.info("Creating databricks job")
     job_name = config_name
 
     j = w.jobs.create(
         name=job_name,
         tasks = [
             Task(
                 description = "Basic new job",
                 existing_cluster_id = serra_profile.databricks_cluster_id,
                 python_wheel_task=PythonWheelTask(entry_point="serra_databricks",
                                                 package_name="serra",
                                                 parameters=[config_name]),
-                libraries=[Library(whl=S3_WHEEL_PATH)],
+                libraries=[Library(whl=s3_wheel_path)],
                 task_key="my-task"
             )
     ]
     )
     logger.info(f"View job at {w.config.host}/#job/{j.job_id}")
     return j
 
 def restart_server():
     w = create_databricks_workspace_client()
     serra_profile = get_serra_profile()
+    s3_wheel_path = get_remote_path_to_wheel()
     cluster_id = serra_profile.databricks_cluster_id
 
     logger.info("Restarting cluster")
     w.clusters.ensure_cluster_is_running(cluster_id)
 
     logger.info("Uninstalling packages")
     w.libraries.uninstall(cluster_id=cluster_id,
-                          libraries=[Library(whl=S3_WHEEL_PATH)])
+                          libraries=[Library(whl=s3_wheel_path)])
     
     current_cluster_state = w.clusters.get(cluster_id).state
 
     if current_cluster_state != State.TERMINATED:
         w.clusters.restart_and_wait(cluster_id)
     
     w.clusters.ensure_cluster_is_running(cluster_id)
```

### Comparing `serra-0.2/serra/profile.py` & `serra-0.3/serra/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         return self.config.get("AWS_ACCESS_KEY_ID")
     
     @property
     def aws_secret_access_key(self):
         return self.config.get("AWS_SECRET_ACCESS_KEY")
     
     @property
+    def aws_config_bucket(self):
+        return self.config.get("AWS_CONFIG_BUCKET")
+    
+    @property
     def databricks_host(self):
         return self.config.get("DATABRICKS_HOST")
     
     @property
     def databricks_token(self):
         return self.config.get("DATABRICKS_TOKEN")
```

### Comparing `serra-0.2/serra/readers/amazon_reader.py` & `serra-0.3/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/readers/databricks_reader.py` & `serra-0.3/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/run.py` & `serra-0.3/serra/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os
 from serra.config_parser import ConfigParser
 from serra.utils import get_path_to_user_configs_folder, write_to_file
 from os.path import exists
 from loguru import logger
 from serra.databricks import upload_wheel_to_bucket, restart_server
 from serra.runners.graph_runner import run_job_with_graph
-from serra.translate import Translator
 from serra.exceptions import SerraRunException
+from serra.translate_client import save_as_yaml, get_translated_yaml
 
 PACKAGE_PATH = os.path.dirname(os.path.dirname(__file__))
 
 # Setup logger
 logger.remove()  # Remove the default sink
 logger.add(sink=sys.stdout, format="<green>{time}</green> - <level>{level}</level> - <cyan>{message}</cyan>", colorize=True)
 
@@ -46,22 +46,24 @@
     yaml_path = os.path.splitext(sql_path)[0]
 
     # Translate job by getting root dir, sql folder, sql path, get response, package path is just serra/
     sql_folder_path = './sql'
 
     sql_path = f"{sql_folder_path}/{sql_path}"
 
-    tl = Translator(sql_path)
-    response = tl.prompt_gpt()
+    translated_yaml = get_translated_yaml(sql_path)
+    if not translated_yaml:
+        logger.error("Unable to translate file")
+        return
 
     # Save in new yaml file (config folder with same name as sql path)
     user_configs_folder = get_path_to_user_configs_folder()
     yaml_path = f"{user_configs_folder}/{yaml_path}.yml"
     logger.info(f"Translation complete. Yaml file can be found at {os.path.abspath(yaml_path)}")
-    tl.save_as_yaml(response, yaml_path)
+    save_as_yaml(translated_yaml, yaml_path)
 
     if is_run:
         logger.info("Running job...")
         cf = ConfigParser.from_local_config(yaml_path)
     # run_job_simple_linear(cf, True)
         try:
             run_job_with_graph(cf)
```

### Comparing `serra-0.2/serra/runners/ExecutionGraph.py` & `serra-0.3/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/runners/graph_runner.py` & `serra-0.3/serra/runners/graph_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from serra.config_parser import ConfigParser, convert_name_to_full
-from serra.utils import get_or_create_spark_session, import_class
+from serra.utils import import_class
 from serra.tests import duplicates_test, nulls_test
 from loguru import logger
 from serra.runners.ExecutionGraph import BlockGraph
 
 
 # Returns instatiated reader,writer,transformer class with config already passed in
 def get_configured_block_object(block_name, cf: ConfigParser):
@@ -67,20 +67,18 @@
             input_dfs = [df_map[dep] for dep in block_obj.dependencies]
             df = block_obj.transform(*input_dfs)
             df_map[block_name] = df
 
         if cf.get_tests_for_block(block_name) is not None:
             tests = cf.get_tests_for_block(block_name)
             for test_name in tests:
-                print(test_name)
+                logger.info(f"\tRunning test {test_name}")
                 if test_name == 'nulls':
                     df = df_map[block_name]
-                    print('checking')
                     nulls_test(df)
                 if test_name == 'duplicates':
                     df = df_map[block_name]
-                    print('checking')
                     duplicates_test(df)
 
     if cf.get_test():
         logger.info("Debug is true—printing out rows.")
         df.show(500)
```

### Comparing `serra-0.2/serra/transformers/__init__.py` & `serra-0.3/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/add_column_transformer.py` & `serra-0.3/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/case_when_transformer.py` & `serra-0.3/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/drop_columns_transformer.py` & `serra-0.3/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/get_count_transformer.py` & `serra-0.3/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/join_transformer.py` & `serra-0.3/serra/transformers/join_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -36,16 +36,11 @@
 
         assert len(join_keys) == 2
 
         matching_col = join_keys
 
         df1 = df1.join(df2, df1[matching_col[0]] == df2[matching_col[1]], self.join_type).drop(df2[matching_col[1]])
         if df1.isEmpty():
-            raise SerraRunException(f"""Joiner - Join Key Error: sales.{matching_col[0]}, ratings.{matching_col[1]} columns do not match.
-                                    
-                                          Dataframes: restaurants & ratings. 
-                                          Suggestion: Look at the the type for {matching_col[0]}, {matching_col[1]}.
-                                          Upstream Job Dependencies: restaurants_load, ratings_load
-                                          Contact: Customer Sales Data Team""")
+            raise SerraRunException(f"""Joiner - Join Key Error: {matching_col[0]}, {matching_col[1]} columns do not match.""")
         return df1
```

### Comparing `serra-0.2/serra/transformers/map_transformer.py` & `serra-0.3/serra/transformers/map_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/pivot_transformer.py` & `serra-0.3/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/rename_column_transformer.py` & `serra-0.3/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/transformers/select_transformer.py` & `serra-0.3/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/utils.py` & `serra-0.3/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/writers/amazon_writer.py` & `serra-0.3/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/writers/databricks_writer.py` & `serra-0.3/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra/writers/s3_writer.py` & `serra-0.3/serra/writers/s3_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.2/serra.egg-info/SOURCES.txt` & `serra-0.3/serra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 serra/config.py
 serra/config_parser.py
 serra/databricks.py
 serra/exceptions.py
 serra/profile.py
 serra/run.py
 serra/tests.py
-serra/translate.py
+serra/translate_client.py
 serra/utils.py
 serra.egg-info/PKG-INFO
 serra.egg-info/SOURCES.txt
 serra.egg-info/dependency_links.txt
 serra.egg-info/entry_points.txt
 serra.egg-info/not-zip-safe
 serra.egg-info/requires.txt
@@ -29,15 +29,14 @@
 serra/runners/ExecutionGraph.py
 serra/runners/__init__.py
 serra/runners/graph_runner.py
 serra/transformers/__init__.py
 serra/transformers/add_column_transformer.py
 serra/transformers/case_when_transformer.py
 serra/transformers/cast_columns_transformer.py
-serra/transformers/conversion_to_usd_transformer.py
 serra/transformers/drop_columns_transformer.py
 serra/transformers/get_count_transformer.py
 serra/transformers/join_transformer.py
 serra/transformers/map_transformer.py
 serra/transformers/pivot_transformer.py
 serra/transformers/rename_column_transformer.py
 serra/transformers/select_transformer.py
```

### Comparing `serra-0.2/setup.py` & `serra-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.2',
+      version='0.3',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Alan Wang',
       author_email='alan@serra.io',
       license='tbd',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/*.yml"]},
```

