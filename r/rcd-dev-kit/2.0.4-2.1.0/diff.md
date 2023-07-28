# Comparing `tmp/rcd_dev_kit-2.0.4.tar.gz` & `tmp/rcd_dev_kit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcd_dev_kit-2.0.4.tar", max compression
+gzip compressed data, was "rcd_dev_kit-2.1.0.tar", max compression
```

## Comparing `rcd_dev_kit-2.0.4.tar` & `rcd_dev_kit-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rwxr-xr-x   0        0        0     1079 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/LICENSE
--rw-r--r--   0        0        0     3990 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/README.md
--rw-r--r--   0        0        0     3441 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      135 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/__init__.py
--rw-r--r--   0        0        0     7119 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/README.md
--rw-r--r--   0        0        0      702 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/__init__.py
--rw-r--r--   0        0        0    10194 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/directus_operator.py
--rw-r--r--   0        0        0     9590 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
--rw-r--r--   0        0        0     8970 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/gcloud_operator.py
--rw-r--r--   0        0        0      469 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/mysql_operator.py
--rw-r--r--   0        0        0    68724 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/redshift_operator.py
--rw-r--r--   0        0        0     7856 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/s3_operator.py
--rw-r--r--   0        0        0    32379 2023-04-12 12:21:54.760630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/snowflake_operator.py
--rw-r--r--   0        0        0     1567 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/README.md
--rw-r--r--   0        0        0       73 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/__init__.py
--rw-r--r--   0        0        0     4602 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/dictionary.py
--rw-r--r--   0        0        0     2253 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
--rw-r--r--   0        0        0      632 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/README.md
--rw-r--r--   0        0        0       75 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/__init__.py
--rw-r--r--   0        0        0      530 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/debug_decorator.py
--rw-r--r--   0        0        0      628 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/functional_decorator.py
--rw-r--r--   0        0        0     3567 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/README.md
--rw-r--r--   0        0        0      270 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/__init__.py
--rw-r--r--   0        0        0      334 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_as_bytes.py
--rw-r--r--   0        0        0     1493 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_detector.py
--rw-r--r--   0        0        0     8908 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_downloader.py
--rw-r--r--   0        0        0     2118 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_operator.py
--rw-r--r--   0        0        0     1390 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_writer.py
--rw-r--r--   0        0        0     1386 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/README.md
--rw-r--r--   0        0        0      206 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/__init__.py
--rw-r--r--   0        0        0     4115 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/checker.py
--rw-r--r--   0        0        0     3178 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/detector.py
--rw-r--r--   0        0        0     1127 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/io.py
--rw-r--r--   0        0        0      579 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/manipulator.py
--rw-r--r--   0        0        0     6151 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/normalizer.py
--rw-r--r--   0        0        0       85 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/sql_utils/__init__.py
--rw-r--r--   0        0        0    21107 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/sql_utils/sql2sf.py
--rw-r--r--   0        0        0     9032 2023-04-12 12:21:54.764630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
--rw-r--r--   0        0        0        0 2023-04-12 12:21:54.768630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/verification_utils/__init__.py
--rw-r--r--   0        0        0     1158 2023-04-12 12:21:54.768630 rcd_dev_kit-2.0.4/src/rcd_dev_kit/verification_utils/verifification.py
--rw-r--r--   0        0        0     6691 1970-01-01 00:00:00.000000 rcd_dev_kit-2.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1079 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6157 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/README.md
+-rw-r--r--   0        0        0     3298 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/__init__.py
+-rw-r--r--   0        0        0     7119 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/README.md
+-rw-r--r--   0        0        0      702 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/__init__.py
+-rw-r--r--   0        0        0    10194 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/directus_operator.py
+-rw-r--r--   0        0        0    12653 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
+-rw-r--r--   0        0        0     8970 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/gcloud_operator.py
+-rw-r--r--   0        0        0      469 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/mysql_operator.py
+-rw-r--r--   0        0        0    68724 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/redshift_operator.py
+-rw-r--r--   0        0        0     7856 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/s3_operator.py
+-rw-r--r--   0        0        0    32379 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/snowflake_operator.py
+-rw-r--r--   0        0        0     1567 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/README.md
+-rw-r--r--   0        0        0       73 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/__init__.py
+-rw-r--r--   0        0        0     4602 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/dictionary.py
+-rw-r--r--   0        0        0     2253 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
+-rw-r--r--   0        0        0      632 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/README.md
+-rw-r--r--   0        0        0       75 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/__init__.py
+-rw-r--r--   0        0        0      530 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/debug_decorator.py
+-rw-r--r--   0        0        0      628 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/functional_decorator.py
+-rw-r--r--   0        0        0     3567 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/README.md
+-rw-r--r--   0        0        0      270 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_as_bytes.py
+-rw-r--r--   0        0        0     1493 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_detector.py
+-rw-r--r--   0        0        0     8908 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_downloader.py
+-rw-r--r--   0        0        0     2118 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_operator.py
+-rw-r--r--   0        0        0     1390 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_writer.py
+-rw-r--r--   0        0        0     1386 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/README.md
+-rw-r--r--   0        0        0      206 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/__init__.py
+-rw-r--r--   0        0        0     4115 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/checker.py
+-rw-r--r--   0        0        0     3178 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/detector.py
+-rw-r--r--   0        0        0     1127 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/io.py
+-rw-r--r--   0        0        0      579 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/manipulator.py
+-rw-r--r--   0        0        0     6151 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/normalizer.py
+-rw-r--r--   0        0        0       85 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/__init__.py
+-rw-r--r--   0        0        0    21107 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/sql2sf.py
+-rw-r--r--   0        0        0     9032 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
+-rw-r--r--   0        0        0        0 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/verification_utils/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/verification_utils/verifification.py
+-rw-r--r--   0        0        0     8425 1970-01-01 00:00:00.000000 rcd_dev_kit-2.1.0/PKG-INFO
```

### Comparing `rcd_dev_kit-2.0.4/LICENSE` & `rcd_dev_kit-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/pyproject.toml` & `rcd_dev_kit-2.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 [tool.poetry]
 name = "rcd-dev-kit"
-version = "2.0.4"
+version = "2.1.0"
 description = "Interact with OIP ecosystem."
 authors = ["Davi FACANHA", "Yu LE VERN"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python :: 3.8',
 ]
-homepage = "https://github.com/OpenInnovationProgram/rcd-dev-kit"
-repository = "https://github.com/OpenInnovationProgram/rcd-dev-kit"
-exclude = ["src/rcd_dev_kit/main.py",
+homepage = "https://github.com/Tekkare/rcd-dev-kit"
+repository = "https://github.com/Tekkare/rcd-dev-kit"
+exclude = [
+        "src/rcd_dev_kit/main.py",
         "src/rcd_dev_kit/migrate_sf_data.py",
         "src/rcd_dev_kit/Untitled.ipynb",
         "src/rcd_dev_kit/.ipynb_checkpoints",
         "src/rcd_dev_kit/migrate_big_data.py",
         "src/rcd_dev_kit/list_wrong_tables.py",
-        "src/rcd_dev_kit/datawarehouse_quality_report.txt"]
+        "src/rcd_dev_kit/datawarehouse_quality_report.txt"
+]
 
 [tool.poetry.dependencies] # requirements.txt
-python = "^3.8"
-boto3 = "^1.22.7"
-numpy = "^1.22.3"
-pandas = "^1.4.2"
-botocore = "^1.25.7"
-sqlalchemy-redshift = "^0.8.11"
-sqlalchemy = "^1.4"
-psycopg2-binary = "^2.9.3"
-snowflake-connector-python = {extras = ["pandas"], version = "2.7.9"}
-sqlparse = "^0.4.2"
-elasticsearch = ">=7.0.0,<8.0.0"
-python-dotenv = "^0.20.0"
-connectorx = "^0.3.0"
-py-markdown-table = "^0.3.3"
-tqdm = "^4.64.1"
-statsmodels = "^0.13.2"
-scikit-learn = "^1.1.2"
-pyspark = "^3.0.0"
-#snowflake-sqlalchemy = "^1.4.0"
+python = "^3.9"
+snowflake-connector-python = {extras = ["pandas"], version = "^3.0.4"}
+boto3 = "^1.28.12"
+numpy = "^1.25.1"
+pandas = "^2.0.3"
+botocore = "^1.31.12"
+psycopg2-binary = "^2.9.6"
+sqlparse = "^0.4.4"
+elasticsearch = "^8.8.2"
+python-dotenv = "^1.0.0"
+connectorx = "^0.3.1"
+py-markdown-table = "^0.4.0"
+tqdm = "^4.65.0"
+statsmodels = "^0.14.0"
+scikit-learn = "^1.3.0"
+sqlalchemy-redshift = "^0.8.14"
+
+# pyTest packages to be installed via extra package rcd-dev-kit[py_test]
+pytest = {version = "^7.4.0", optional = true}
+pytest-cov = {version = "^4.1.0", optional = true}
 
+# Google packages to be installed via extra package rcd-dev-kit[google]
 google = { version = "^3.0.0", optional = true }
 google-api-python-client = { version = "^2.47.0", optional = true }
 google-cloud-storage = { version = "^2.3.0", optional = true }
 googletrans = { version = "3.0.0", optional = true }
-#google-cloud = { version = "^0.34.0", optional = true }
-
-dagster = { version = "^1.0.16", optional = true }
-dagit = { version = "^1.0.16", optional = true }
-dagster-postgres = { version = "0.16.16", optional = true }
-dagster-k8s =  { version = "0.16.16", optional = true }
-requests = { version = "^2.28.1", optional = true }
+google-cloud = { version = "^0.34.0", optional = true }
 
+# Sphinx packages to be installed via extra package rcd-dev-kit[docs]
+# Those packages are used mainly to generate automatically the doc html of the package.
 Sphinx = { version = "^5.2.3", optional = true }
 sphinx-rtd-theme = { version = "1.0.0", optional = true }
 sphinxcontrib-napoleon = { version = "0.7", optional = true }
 myst-nb = {version = "^0.17.1", python = "^3.8", optional = true }
 sphinx-autoapi = { version = "^2.0.0", optional = true }
 
-pytest = { version = "^7.1", optional = true }
-pytest-cov = { version = "^3.0.0", optional = true }
-
 [tool.poetry.extras]
-py-test = ["pytest", "pytest-cov"]
+py_test = ["pytest", "pytest-cov"]
 google = ["google", "google-api-python-client", "google-cloud-storage", "googletrans"]
-dagster = ["dagster", "dagit", "dagster-postgres", "dagster-k8s", "requests"]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon", "sphinx-autoapi", "myst-nb"]
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
```

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/README.md` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/__init__.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/directus_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/directus_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/elasticsearch_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/elasticsearch_operator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import os
 import json
 import certifi
 import pandas as pd
 from datetime import datetime
-from typing import Any, Generator
+from typing import Any, Generator, Optional
 from elasticsearch import Elasticsearch
 from elasticsearch.exceptions import ConnectionTimeout
 from elasticsearch.helpers import parallel_bulk, bulk
 from .. import decorator_manager
 
 
-def index_json_bulk_parallel(index: str, method: str, **kwargs: Any) -> None:
+def index_json_bulk_parallel(index: str, method: str, custom_mapping_json: Optional[dict] = None,  **kwargs: Any) -> None:
     """
     Function index_json_bulk_parallel.
     Use this function to send data to elasticsearch with bulk indexing and multi-threading.
 
     Args:
         index(str): The name of index in elasticsearch.
         method (str): "json" send to elasticsearch with local .json file, or "dataframe" send to elasticsearch with pandas dataframe.
+        custom_mapping_json (dict, None):
+            Json value containing the index custom mapping.
+            Obs: In Elasticsearch, mappings are used to define how documents and their fields are indexed and stored
+                 in the search engine. When you index data into Elasticsearch, it automatically tries to infer the data
+                 types of the fields based on the JSON documents you provide. However, you can also explicitly define
+                 custom mappings to have more control over how the data is indexed and analyzed.
     Kwargs:
         keyword(str): Only for method="json", the keyword to filter json file. By default it is an empty string.
         json_path(str): Only for method="json", the local directory which contains json file.
 
         df(pd.Dataframe): Only for method="dataframe", pandas dataframe object to index.
     Examples:
         >>> from rcd_dev_kit import database_manager
         >>> database_manager.index_json_bulk_parallel(index="my_index", method="json", json_path="my_json_path", keyword="")
         >>> database_manager.index_json_bulk_parallel(index="my_index", method="dataframe", df=pd.DataFrame())
     """
     eo = ElasticsearchOperator(index=index)
     request_timeout = kwargs.get("request_timeout", 1200)
+
+    if custom_mapping_json:
+        eo.mapping = custom_mapping_json
+        eo.set_custom_mapping()
+
     if method == "json":
         eo.json_path = kwargs.get("json_path")
         eo.detect_json(keyword=kwargs.get("keyword"))
     elif method == "dataframe":
         eo.pd_dataframe = kwargs.get("df")
     else:
         raise ValueError(f"Unrecognized method: {method}")
@@ -53,32 +64,43 @@
                 request_timeout = int(
                     input("Enter your request_timeout setting: (integer > 1200)")
                 )
             print(f"Restarting with time_out {request_timeout}.")
 
 
 def index_json_bulk(
-    json_path: str, index: str, keyword: str = "", **kwargs: Any
+        json_path: str, index: str, keyword: str = "", custom_mapping_json: Optional[dict] = None, **kwargs: Any
 ) -> None:
     """
     Function index_json_bulk.
     Use this function to send data to elasticsearch with bulk indexing.
 
     Args:
         json_path (str): The path of json directory.
         index(str): The name of index in elasticsearch.
         keyword(str): The keyword to filter json file. By default it is an empty string.
+        custom_mapping_json (dict, None):
+            Json value containing the index custom mapping.
+            Obs: In Elasticsearch, mappings are used to define how documents and their fields are indexed and stored
+                 in the search engine. When you index data into Elasticsearch, it automatically tries to infer the data
+                 types of the fields based on the JSON documents you provide. However, you can also explicitly define
+                 custom mappings to have more control over how the data is indexed and analyzed.
     Examples:
         >>> from rcd_dev_kit import database_manager
         >>> database_manager.index_json_bulk(index="my_index", json_path="my_json_path", keyword="")
     """
     eo = ElasticsearchOperator(index=index)
     eo.json_path = json_path
     eo.detect_json(keyword=keyword)
     request_timeout = kwargs.get("request_timeout", 1200)
+
+    if custom_mapping_json:
+        eo.mapping = custom_mapping_json
+        eo.set_custom_mapping()
+
     while True:
         try:
             eo.request_timeout = request_timeout
             eo.bulk_index()
             break
         except ConnectionTimeout:
             is_again = input(
@@ -90,62 +112,89 @@
                 request_timeout = int(
                     input("Enter your request_timeout setting: (integer > 1200)")
                 )
             print(f"Restarting with time_out {request_timeout}.")
 
 
 def index_json(
-    json_path: str,
-    index: str,
-    keyword: str = "",
-    show_debug: bool = True,
-    **kwargs: Any,
+        json_path: str,
+        index: str,
+        keyword: str = "",
+        show_debug: bool = True,
+        custom_mapping_json: Optional[dict] = None,
+        **kwargs: Any,
 ):
     """
     Function index_json.
     Use this function to send data to elasticsearch with normal indexing.
 
     Parameters:
           json_path (str): The path of json directory.
           index(str): The name of index in elasticsearch.
           keyword(str): The keyword to filter json file. By default it is an empty string.
           show_debug(bool): Display debugging information or not.
+          custom_mapping_json (dict, None):
+            Json value containing the index custom mapping.
+            Obs: In Elasticsearch, mappings are used to define how documents and their fields are indexed and stored
+                 in the search engine. When you index data into Elasticsearch, it automatically tries to infer the data
+                 types of the fields based on the JSON documents you provide. However, you can also explicitly define
+                 custom mappings to have more control over how the data is indexed and analyzed.
     Examples:
         >>> from rcd_dev_kit import database_manager
         >>> database_manager.index_json(json_path="my_json_path", index="my_index", keyword="")
     """
     eo = ElasticsearchOperator(index=index)
     eo.json_path = json_path
     eo.detect_json(keyword=keyword)
     if kwargs.get("request_timeout"):
         eo.request_timeout = kwargs.get("request_timeout")
+
+    if custom_mapping_json:
+        eo.mapping = custom_mapping_json
+        eo.set_custom_mapping()
+
     eo.normal_index_json(show_debug=show_debug)
 
 
 class ElasticsearchOperator:
     """
     Class ElasticsearchOperator.
     Use this class to manipulate data with elasticsearch.
 
     Parameters:
           index (str): elasticsearch index name.
     """
 
     def __init__(self, index: str) -> None:
+        host = os.environ.get("ELASTICSEARCH_HOST")
+        user = os.environ.get("ELASTICSEARCH_USER")
+        password = os.environ.get("ELASTICSEARCH_PASSWORD")
+        scheme = os.environ.get("ELASTICSEARCH_SCHEME")
+        port = int(os.environ.get("ELASTICSEARCH_PORT"))
+
         self.connection = Elasticsearch(
-            hosts=os.environ.get("ELASTICSEARCH_HOST"),
-            http_auth=(
-                os.environ.get("ELASTICSEARCH_USER"),
-                os.environ.get("ELASTICSEARCH_PASSWORD"),
-            ),
-            scheme=os.environ.get("ELASTICSEARCH_SCHEME"),
-            port=os.environ.get("ELASTICSEARCH_PORT"),
-            use_ssl=True,
+            [
+                {'host': host, 'port': port, "scheme": scheme}
+            ],
+            http_auth=(user, password),
             ca_certs=certifi.where(),
         )
+
+        # self.connection = Elasticsearch(
+        #     hosts=os.environ.get("ELASTICSEARCH_HOST"),
+        #     http_auth=(
+        #         os.environ.get("ELASTICSEARCH_USER"),
+        #         os.environ.get("ELASTICSEARCH_PASSWORD"),
+        #     ),
+        #     scheme=os.environ.get("ELASTICSEARCH_SCHEME"),
+        #     port=os.environ.get("ELASTICSEARCH_PORT"),
+        #     use_ssl=True,
+        #     ca_certs=certifi.where(),
+        # )
+        self._mapping = None
         self._json_path = None
         self._pd_dataframe = None
         self._request_timeout = 1200
         self.index = index
         self.lst_json = list()
 
     @property
@@ -171,21 +220,33 @@
         return self._request_timeout
 
     @request_timeout.setter
     def request_timeout(self, value: int) -> None:
         print(f"Setting request_timeout to {value}")
         self._request_timeout = value
 
+    @property
+    def mapping(self) -> dict:
+        return self._mapping
+
+    @mapping.setter
+    def mapping(self, value: dict) -> None:
+        print(f"Setting custom mapping json. 🖇")
+        self._mapping = value
+
+    def set_custom_mapping(self):
+        self.connection.indices.create(index=self.index, body=self._mapping, ignore=400)
+
     def detect_json(self, keyword: str) -> None:
         self.lst_json = [
             file
             for file in os.listdir(self.json_path)
             if (file.endswith(".json"))
-            and (not file.startswith("."))
-            and (keyword in file)
+               and (not file.startswith("."))
+               and (keyword in file)
         ]
         print(f"{len(self.lst_json)} .json files with keyword '{keyword}' detected.")
 
     def index_json(self, json_file: str, show_debug: bool = True) -> None:
         document_id = json_file.rsplit(".json")[0]
         with open(os.path.join(self.json_path, json_file)) as f:
             reader = json.load(f)
@@ -249,13 +310,13 @@
             actions=self.get_generator(),
             request_timeout=self._request_timeout,
         )
 
     @decorator_manager.timeit(program_name="Parallel Bulk indexing")
     def parallel_bulk_index(self) -> None:
         for success, info in parallel_bulk(
-            client=self.connection,
-            actions=self.get_generator(),
-            request_timeout=self._request_timeout,
+                client=self.connection,
+                actions=self.get_generator(),
+                request_timeout=self._request_timeout,
         ):
             if not success:
                 print(info)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/gcloud_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/gcloud_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/redshift_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/redshift_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/s3_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/s3_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/database_manager/snowflake_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/snowflake_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/README.md` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/dictionary.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/dictionary.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/dataclass_manager/raw_data_file.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/raw_data_file.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/README.md` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/debug_decorator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/debug_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/decorator_manager/functional_decorator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/functional_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/README.md` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_detector.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_downloader.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_downloader.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_operator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/file_manager/file_writer.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_writer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/README.md` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/checker.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/checker.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/detector.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/io.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/io.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/manipulator.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/manipulator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/pandas_manager/normalizer.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/normalizer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/sql_utils/sql2sf.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/sql2sf.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.0.4/src/rcd_dev_kit/verification_utils/verifification.py` & `rcd_dev_kit-2.1.0/src/rcd_dev_kit/verification_utils/verifification.py`

 * *Files identical despite different names*

