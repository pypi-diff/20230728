# Comparing `tmp/oddrn-generator-0.1.9.tar.gz` & `tmp/oddrn_generator-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddrn-generator-0.1.9.tar", max compression
+gzip compressed data, was "oddrn_generator-0.1.90.tar", max compression
```

## Comparing `oddrn-generator-0.1.9.tar` & `oddrn_generator-0.1.90.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    11356 2021-10-08 14:14:06.775943 oddrn-generator-0.1.9/LICENSE
--rw-r--r--   0        0        0     4970 2021-10-18 10:25:57.387497 oddrn-generator-0.1.9/README.md
--rw-r--r--   0        0        0      842 2021-10-18 12:18:05.407813 oddrn-generator-0.1.9/oddrn_generator/__init__.py
--rw-r--r--   0        0        0      157 2021-10-08 14:14:06.777038 oddrn-generator-0.1.9/oddrn_generator/exceptions.py
--rw-r--r--   0        0        0     5346 2021-10-18 10:28:14.410979 oddrn-generator-0.1.9/oddrn_generator/generators.py
--rw-r--r--   0        0        0    10224 2021-10-18 12:18:05.411939 oddrn-generator-0.1.9/oddrn_generator/path_models.py
--rw-r--r--   0        0        0      529 2021-10-08 14:14:06.777467 oddrn-generator-0.1.9/oddrn_generator/server_models.py
--rw-r--r--   0        0        0      627 2021-10-18 12:18:05.403660 oddrn-generator-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5904 2021-10-18 12:18:39.384833 oddrn-generator-0.1.9/setup.py
--rw-r--r--   0        0        0     5719 2021-10-18 12:18:39.385238 oddrn-generator-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/LICENSE
+-rw-r--r--   0        0        0     6337 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/README.md
+-rw-r--r--   0        0        0     2722 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/exceptions.py
+-rw-r--r--   0        0        0    12718 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/generators.py
+-rw-r--r--   0        0        0    24577 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/path_models.py
+-rw-r--r--   0        0        0     3652 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/server_models.py
+-rw-r--r--   0        0        0      287 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/utils/__init__.py
+-rw-r--r--   0        0        0     7327 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/utils/external_generators.py
+-rw-r--r--   0        0        0      734 2023-07-28 12:41:43.000000 oddrn_generator-0.1.90/pyproject.toml
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 oddrn_generator-0.1.90/setup.py
+-rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 oddrn_generator-0.1.90/PKG-INFO
```

### Comparing `oddrn-generator-0.1.9/LICENSE` & `oddrn_generator-0.1.90/LICENSE`

 * *Files identical despite different names*

### Comparing `oddrn-generator-0.1.9/README.md` & `oddrn_generator-0.1.90/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,102 @@
+[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)
+
 # Open Data Discovery Resource Name Generator
+
+Helps generate oddrn for data sources.
+
+* [Requirements](#requirements)
+* [Installation](#installation)
+* [Available generators](#available-generators)
+* [Generator properties](#generator-properties)
+* [Generator methods](#generator-methods)
+* [Generator properties](#generator-properties)
+* [Example usage](#example-usage)
+* [Exceptions](#example-usage)
+* [Development](#development)
+
 ## Requirements
-Python >= 3.7
+
+* __Python >= 3.7__
+
 ## Installation
+
+```bash
+poetry add oddrn-generator
+# or
+pip install oddrn-generator
 ```
-poetry install
-```
+
 ## Usage and configuration
+
 ### Available generators
-* postgresql - PostgresqlGenerator
-* mysql - MysqlGenerator
-* glue - GlueGenerator
-* kafka - KafkaGenerator
-* kafkaconnect - KafkaConnectGenerator
-* snowflake - SnowflakeGenerator
-* airflow - AirflowGenerator
-* hive - HiveGenerator
-* dynamodb - DynamodbGenerator
-* odbc - OdbcGenerator
-* mssql - MssqlGenerator
-* oracle - OracleGenerator
-* redshift - RedshiftGenerator
-* clickhouse - ClickHouseGenerator
-* athena - AthenaGenerator
-* quicksight - QuicksightGenerator
-* dbt - DbtGenerator
-* tableau - TableauGenerator
-### Work in progress generators
-* kubeflow - KubeflowGenerator
-* dvc - DVCGenerator
-* great_expectations - GreatExpectationsGenerator
+| DataSource   | Generator class name  |
+|--------------|-----------------------|
+| cassandra    | CassandraGenerator    |
+| postgresql   | PostgresqlGenerator   |
+| mysql        | MysqlGenerator        |
+| glue         | GlueGenerator         |
+| s3           | S3Generator           |
+| kafka        | KafkaGenerator        |
+| kafkaconnect | KafkaConnectGenerator |
+| snowflake    | SnowflakeGenerator    |
+| airflow      | AirflowGenerator      |
+| hive         | HiveGenerator         |
+| dynamodb     | DynamodbGenerator     |
+| odbc         | OdbcGenerator         |
+| mssql        | MssqlGenerator        |
+| oracle       | OracleGenerator       |
+| redshift     | RedshiftGenerator     |
+| clickhouse   | ClickHouseGenerator   |
+| athena       | AthenaGenerator       |
+| quicksight   | QuicksightGenerator   |
+| dbt          | DbtGenerator          |
+| prefect      | PrefectGenerator      |
+| tableau      | TableauGenerator      |
+| neo4j        | Neo4jGenerator        |
+| mongodb      | MongoGenerator        |
+| vertica      | VerticaGenerator      |
+| CubeJs       | CubeJsGenerator       |
+| superset     | SupersetGenerator     |
+| Presto       | PrestoGenerator       |
+| Trino        | TrinoGenerator        |
+| dms          | DmsGenerator          |
+| powerbi      | PowerBiGenerator      |
 
 ### Generator properties
+
 * base_oddrn - Get base oddrn (without path)
-* available_paths - Get all available path of generator 
+* available_paths - Get all available path of generator
 
 ### Generator methods
-* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using 'new_value' param
+
+* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using '
+  new_value' param
 * set_oddrn_paths(**kwargs) - Set or update values of oddrn path
-* get_data_source_oddrn() - Get datasouce oddrn 
+* get_data_source_oddrn() - Get data source oddrn
 
 ### Generator parameters:
+
 * host_settings: str - optional. Hostname configuration
-* cloud_settings: dict - optional.  Cloud configuration
+* cloud_settings: dict - optional. Cloud configuration
 * **kwargs - path's name and values
 
 ### Example usage
+
 ```python
 # postgresql
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
-  host_settings='my.host.com:5432', 
-  schemas='schema_name', databases='database_name', tables='table_name'
+    host_settings='my.host.com:5432',
+    schemas='schema_name', databases='database_name', tables='table_name'
 )
 
 oddrn_gen.base_oddrn
-# //postgresql/host/my.host.com:5432/
+# //postgresql/host/my.host.com:5432
 oddrn_gen.available_paths
 # ('schemas', 'databases', 'tables', 'columns')
 
 oddrn_gen.get_data_source_oddrn()
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("schemas")
@@ -78,18 +116,19 @@
 # you can get path wih new values:
 oddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name
 
 
 # glue
 from oddrn_generator import GlueGenerator
+
 oddrn_gen = GlueGenerator(
-  cloud_settings={'account': 'acc_id', 'region':'reg_id'}, 
-  databases='database_name', tables='table_name', columns='column_name', 
-  jobs='job_name', runs='run_name', owners='owner_name'
+    cloud_settings={'account': 'acc_id', 'region': 'reg_id'},
+    databases='database_name', tables='table_name', columns='column_name',
+    jobs='job_name', runs='run_name', owners='owner_name'
 )
 
 oddrn_gen.available_paths
 # ('databases', 'tables', 'columns', 'owners', 'jobs', 'runs')
 
 oddrn_gen.get_oddrn_by_path("databases")
 # //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name
@@ -108,37 +147,59 @@
 
 oddrn_gen.get_oddrn_by_path("owners")
 # //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name
 
 ```
 
 ### Exceptions
+
 * WrongPathOrderException - raises when trying set path that depends on another path
+
 ```python
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
-    host_settings='my.host.com:5432', 
+    host_settings='my.host.com:5432',
     schemas='schema_name', databases='database_name',
     columns='column_without_table'
 )
 # WrongPathOrderException: 'columns' can not be without 'tables' attribute
 ```
+
 * EmptyPathValueException - raises when trying to get a path that is not set up
+
 ```python
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("tables")
 
 # EmptyPathValueException: Path 'tables' is not set up
 ```
+
 * PathDoestExistException - raises when trying to get not existing oddrn path
+
 ```python
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("jobs")
 
 # PathDoestExistException: Path 'jobs' doesn't exist in generator
-```
+```
+
+## Development
+
+```bash
+#Install dependencies
+poetry install
+
+#Activate shell
+poetry shell
+
+# Run tests
+python run pytest
+```
```

### Comparing `oddrn-generator-0.1.9/pyproject.toml` & `oddrn_generator-0.1.90/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [tool.poetry]
 name = "oddrn-generator"
-version = "0.1.9"
+version = "0.1.90"
 description = "Open Data Discovery Resource Name Generator"
 authors = ["Open Data Discovery <pypi@opendatadiscovery.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opendatadiscovery/oddrn-generator"
 repository = "https://github.com/opendatadiscovery/oddrn-generator"
 keywords = ["oddrn", "opendatadiscovery"]
 include = ["LICENSE"]
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pydantic = "^1.8.2"
+python = "^3.9"
+pydantic = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
+black = "^22.8.0"
+
+[tool.poetry.group.dev.dependencies]
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
```

### Comparing `oddrn-generator-0.1.9/setup.py` & `oddrn_generator-0.1.90/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['oddrn_generator']
+['oddrn_generator', 'oddrn_generator.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pydantic>=1.8.2,<2.0.0']
+['pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'oddrn-generator',
-    'version': '0.1.9',
+    'version': '0.1.90',
     'description': 'Open Data Discovery Resource Name Generator',
-    'long_description': '# Open Data Discovery Resource Name Generator\n## Requirements\nPython >= 3.7\n## Installation\n```\npoetry install\n```\n## Usage and configuration\n### Available generators\n* postgresql - PostgresqlGenerator\n* mysql - MysqlGenerator\n* glue - GlueGenerator\n* kafka - KafkaGenerator\n* kafkaconnect - KafkaConnectGenerator\n* snowflake - SnowflakeGenerator\n* airflow - AirflowGenerator\n* hive - HiveGenerator\n* dynamodb - DynamodbGenerator\n* odbc - OdbcGenerator\n* mssql - MssqlGenerator\n* oracle - OracleGenerator\n* redshift - RedshiftGenerator\n* clickhouse - ClickHouseGenerator\n* athena - AthenaGenerator\n* quicksight - QuicksightGenerator\n* dbt - DbtGenerator\n* tableau - TableauGenerator\n### Work in progress generators\n* kubeflow - KubeflowGenerator\n* dvc - DVCGenerator\n* great_expectations - GreatExpectationsGenerator\n\n### Generator properties\n* base_oddrn - Get base oddrn (without path)\n* available_paths - Get all available path of generator \n\n### Generator methods\n* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using \'new_value\' param\n* set_oddrn_paths(**kwargs) - Set or update values of oddrn path\n* get_data_source_oddrn() - Get datasouce oddrn \n\n### Generator parameters:\n* host_settings: str - optional. Hostname configuration\n* cloud_settings: dict - optional.  Cloud configuration\n* **kwargs - path\'s name and values\n\n### Example usage\n```python\n# postgresql\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n  host_settings=\'my.host.com:5432\', \n  schemas=\'schema_name\', databases=\'database_name\', tables=\'table_name\'\n)\n\noddrn_gen.base_oddrn\n# //postgresql/host/my.host.com:5432/\noddrn_gen.available_paths\n# (\'schemas\', \'databases\', \'tables\', \'columns\')\n\noddrn_gen.get_data_source_oddrn()\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("schemas")\n# //postgresql/host/my.host.com:5432/schemas/schema_name\n\noddrn_gen.get_oddrn_by_path("databases")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name\n\n# you can set or change path:\noddrn_gen.set_oddrn_paths(tables=\'another_table_name\', columns=\'new_column_name\')\noddrn_gen.get_oddrn_by_path("columns")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name\n\n# you can get path wih new values:\noddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name\n\n\n# glue\nfrom oddrn_generator import GlueGenerator\noddrn_gen = GlueGenerator(\n  cloud_settings={\'account\': \'acc_id\', \'region\':\'reg_id\'}, \n  databases=\'database_name\', tables=\'table_name\', columns=\'column_name\', \n  jobs=\'job_name\', runs=\'run_name\', owners=\'owner_name\'\n)\n\noddrn_gen.available_paths\n# (\'databases\', \'tables\', \'columns\', \'owners\', \'jobs\', \'runs\')\n\noddrn_gen.get_oddrn_by_path("databases")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name\'\n\noddrn_gen.get_oddrn_by_path("columns")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name/columns/column_name\n\noddrn_gen.get_oddrn_by_path("jobs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name\n\noddrn_gen.get_oddrn_by_path("runs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name/runs/run_name\n\noddrn_gen.get_oddrn_by_path("owners")\n# //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name\n\n```\n\n### Exceptions\n* WrongPathOrderException - raises when trying set path that depends on another path\n```python\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', \n    schemas=\'schema_name\', databases=\'database_name\',\n    columns=\'column_without_table\'\n)\n# WrongPathOrderException: \'columns\' can not be without \'tables\' attribute\n```\n* EmptyPathValueException - raises when trying to get a path that is not set up\n```python\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("tables")\n\n# EmptyPathValueException: Path \'tables\' is not set up\n```\n* PathDoestExistException - raises when trying to get not existing oddrn path\n```python\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("jobs")\n\n# PathDoestExistException: Path \'jobs\' doesn\'t exist in generator\n```',
+    'long_description': '[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)\n\n# Open Data Discovery Resource Name Generator\n\nHelps generate oddrn for data sources.\n\n* [Requirements](#requirements)\n* [Installation](#installation)\n* [Available generators](#available-generators)\n* [Generator properties](#generator-properties)\n* [Generator methods](#generator-methods)\n* [Generator properties](#generator-properties)\n* [Example usage](#example-usage)\n* [Exceptions](#example-usage)\n* [Development](#development)\n\n## Requirements\n\n* __Python >= 3.7__\n\n## Installation\n\n```bash\npoetry add oddrn-generator\n# or\npip install oddrn-generator\n```\n\n## Usage and configuration\n\n### Available generators\n| DataSource   | Generator class name  |\n|--------------|-----------------------|\n| cassandra    | CassandraGenerator    |\n| postgresql   | PostgresqlGenerator   |\n| mysql        | MysqlGenerator        |\n| glue         | GlueGenerator         |\n| s3           | S3Generator           |\n| kafka        | KafkaGenerator        |\n| kafkaconnect | KafkaConnectGenerator |\n| snowflake    | SnowflakeGenerator    |\n| airflow      | AirflowGenerator      |\n| hive         | HiveGenerator         |\n| dynamodb     | DynamodbGenerator     |\n| odbc         | OdbcGenerator         |\n| mssql        | MssqlGenerator        |\n| oracle       | OracleGenerator       |\n| redshift     | RedshiftGenerator     |\n| clickhouse   | ClickHouseGenerator   |\n| athena       | AthenaGenerator       |\n| quicksight   | QuicksightGenerator   |\n| dbt          | DbtGenerator          |\n| prefect      | PrefectGenerator      |\n| tableau      | TableauGenerator      |\n| neo4j        | Neo4jGenerator        |\n| mongodb      | MongoGenerator        |\n| vertica      | VerticaGenerator      |\n| CubeJs       | CubeJsGenerator       |\n| superset     | SupersetGenerator     |\n| Presto       | PrestoGenerator       |\n| Trino        | TrinoGenerator        |\n| dms          | DmsGenerator          |\n| powerbi      | PowerBiGenerator      |\n\n### Generator properties\n\n* base_oddrn - Get base oddrn (without path)\n* available_paths - Get all available path of generator\n\n### Generator methods\n\n* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using \'\n  new_value\' param\n* set_oddrn_paths(**kwargs) - Set or update values of oddrn path\n* get_data_source_oddrn() - Get data source oddrn\n\n### Generator parameters:\n\n* host_settings: str - optional. Hostname configuration\n* cloud_settings: dict - optional. Cloud configuration\n* **kwargs - path\'s name and values\n\n### Example usage\n\n```python\n# postgresql\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\', tables=\'table_name\'\n)\n\noddrn_gen.base_oddrn\n# //postgresql/host/my.host.com:5432\noddrn_gen.available_paths\n# (\'schemas\', \'databases\', \'tables\', \'columns\')\n\noddrn_gen.get_data_source_oddrn()\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("schemas")\n# //postgresql/host/my.host.com:5432/schemas/schema_name\n\noddrn_gen.get_oddrn_by_path("databases")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name\n\n# you can set or change path:\noddrn_gen.set_oddrn_paths(tables=\'another_table_name\', columns=\'new_column_name\')\noddrn_gen.get_oddrn_by_path("columns")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name\n\n# you can get path wih new values:\noddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name\n\n\n# glue\nfrom oddrn_generator import GlueGenerator\n\noddrn_gen = GlueGenerator(\n    cloud_settings={\'account\': \'acc_id\', \'region\': \'reg_id\'},\n    databases=\'database_name\', tables=\'table_name\', columns=\'column_name\',\n    jobs=\'job_name\', runs=\'run_name\', owners=\'owner_name\'\n)\n\noddrn_gen.available_paths\n# (\'databases\', \'tables\', \'columns\', \'owners\', \'jobs\', \'runs\')\n\noddrn_gen.get_oddrn_by_path("databases")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name\'\n\noddrn_gen.get_oddrn_by_path("columns")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name/columns/column_name\n\noddrn_gen.get_oddrn_by_path("jobs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name\n\noddrn_gen.get_oddrn_by_path("runs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name/runs/run_name\n\noddrn_gen.get_oddrn_by_path("owners")\n# //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name\n\n```\n\n### Exceptions\n\n* WrongPathOrderException - raises when trying set path that depends on another path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\',\n    columns=\'column_without_table\'\n)\n# WrongPathOrderException: \'columns\' can not be without \'tables\' attribute\n```\n\n* EmptyPathValueException - raises when trying to get a path that is not set up\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("tables")\n\n# EmptyPathValueException: Path \'tables\' is not set up\n```\n\n* PathDoestExistException - raises when trying to get not existing oddrn path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("jobs")\n\n# PathDoestExistException: Path \'jobs\' doesn\'t exist in generator\n```\n\n## Development\n\n```bash\n#Install dependencies\npoetry install\n\n#Activate shell\npoetry shell\n\n# Run tests\npython run pytest\n```\n',
     'author': 'Open Data Discovery',
     'author_email': 'pypi@opendatadiscovery.org',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/opendatadiscovery/oddrn-generator',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `oddrn-generator-0.1.9/PKG-INFO` & `oddrn_generator-0.1.90/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,121 @@
 Metadata-Version: 2.1
 Name: oddrn-generator
-Version: 0.1.9
+Version: 0.1.90
 Summary: Open Data Discovery Resource Name Generator
 Home-page: https://github.com/opendatadiscovery/oddrn-generator
 License: Apache-2.0
 Keywords: oddrn,opendatadiscovery
 Author: Open Data Discovery
 Author-email: pypi@opendatadiscovery.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Repository, https://github.com/opendatadiscovery/oddrn-generator
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)
+
 # Open Data Discovery Resource Name Generator
+
+Helps generate oddrn for data sources.
+
+* [Requirements](#requirements)
+* [Installation](#installation)
+* [Available generators](#available-generators)
+* [Generator properties](#generator-properties)
+* [Generator methods](#generator-methods)
+* [Generator properties](#generator-properties)
+* [Example usage](#example-usage)
+* [Exceptions](#example-usage)
+* [Development](#development)
+
 ## Requirements
-Python >= 3.7
+
+* __Python >= 3.7__
+
 ## Installation
+
+```bash
+poetry add oddrn-generator
+# or
+pip install oddrn-generator
 ```
-poetry install
-```
+
 ## Usage and configuration
+
 ### Available generators
-* postgresql - PostgresqlGenerator
-* mysql - MysqlGenerator
-* glue - GlueGenerator
-* kafka - KafkaGenerator
-* kafkaconnect - KafkaConnectGenerator
-* snowflake - SnowflakeGenerator
-* airflow - AirflowGenerator
-* hive - HiveGenerator
-* dynamodb - DynamodbGenerator
-* odbc - OdbcGenerator
-* mssql - MssqlGenerator
-* oracle - OracleGenerator
-* redshift - RedshiftGenerator
-* clickhouse - ClickHouseGenerator
-* athena - AthenaGenerator
-* quicksight - QuicksightGenerator
-* dbt - DbtGenerator
-* tableau - TableauGenerator
-### Work in progress generators
-* kubeflow - KubeflowGenerator
-* dvc - DVCGenerator
-* great_expectations - GreatExpectationsGenerator
+| DataSource   | Generator class name  |
+|--------------|-----------------------|
+| cassandra    | CassandraGenerator    |
+| postgresql   | PostgresqlGenerator   |
+| mysql        | MysqlGenerator        |
+| glue         | GlueGenerator         |
+| s3           | S3Generator           |
+| kafka        | KafkaGenerator        |
+| kafkaconnect | KafkaConnectGenerator |
+| snowflake    | SnowflakeGenerator    |
+| airflow      | AirflowGenerator      |
+| hive         | HiveGenerator         |
+| dynamodb     | DynamodbGenerator     |
+| odbc         | OdbcGenerator         |
+| mssql        | MssqlGenerator        |
+| oracle       | OracleGenerator       |
+| redshift     | RedshiftGenerator     |
+| clickhouse   | ClickHouseGenerator   |
+| athena       | AthenaGenerator       |
+| quicksight   | QuicksightGenerator   |
+| dbt          | DbtGenerator          |
+| prefect      | PrefectGenerator      |
+| tableau      | TableauGenerator      |
+| neo4j        | Neo4jGenerator        |
+| mongodb      | MongoGenerator        |
+| vertica      | VerticaGenerator      |
+| CubeJs       | CubeJsGenerator       |
+| superset     | SupersetGenerator     |
+| Presto       | PrestoGenerator       |
+| Trino        | TrinoGenerator        |
+| dms          | DmsGenerator          |
+| powerbi      | PowerBiGenerator      |
 
 ### Generator properties
+
 * base_oddrn - Get base oddrn (without path)
-* available_paths - Get all available path of generator 
+* available_paths - Get all available path of generator
 
 ### Generator methods
-* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using 'new_value' param
+
+* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using '
+  new_value' param
 * set_oddrn_paths(**kwargs) - Set or update values of oddrn path
-* get_data_source_oddrn() - Get datasouce oddrn 
+* get_data_source_oddrn() - Get data source oddrn
 
 ### Generator parameters:
+
 * host_settings: str - optional. Hostname configuration
-* cloud_settings: dict - optional.  Cloud configuration
+* cloud_settings: dict - optional. Cloud configuration
 * **kwargs - path's name and values
 
 ### Example usage
+
 ```python
 # postgresql
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
-  host_settings='my.host.com:5432', 
-  schemas='schema_name', databases='database_name', tables='table_name'
+    host_settings='my.host.com:5432',
+    schemas='schema_name', databases='database_name', tables='table_name'
 )
 
 oddrn_gen.base_oddrn
-# //postgresql/host/my.host.com:5432/
+# //postgresql/host/my.host.com:5432
 oddrn_gen.available_paths
 # ('schemas', 'databases', 'tables', 'columns')
 
 oddrn_gen.get_data_source_oddrn()
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("schemas")
@@ -97,18 +135,19 @@
 # you can get path wih new values:
 oddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name
 
 
 # glue
 from oddrn_generator import GlueGenerator
+
 oddrn_gen = GlueGenerator(
-  cloud_settings={'account': 'acc_id', 'region':'reg_id'}, 
-  databases='database_name', tables='table_name', columns='column_name', 
-  jobs='job_name', runs='run_name', owners='owner_name'
+    cloud_settings={'account': 'acc_id', 'region': 'reg_id'},
+    databases='database_name', tables='table_name', columns='column_name',
+    jobs='job_name', runs='run_name', owners='owner_name'
 )
 
 oddrn_gen.available_paths
 # ('databases', 'tables', 'columns', 'owners', 'jobs', 'runs')
 
 oddrn_gen.get_oddrn_by_path("databases")
 # //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name
@@ -127,37 +166,60 @@
 
 oddrn_gen.get_oddrn_by_path("owners")
 # //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name
 
 ```
 
 ### Exceptions
+
 * WrongPathOrderException - raises when trying set path that depends on another path
+
 ```python
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
-    host_settings='my.host.com:5432', 
+    host_settings='my.host.com:5432',
     schemas='schema_name', databases='database_name',
     columns='column_without_table'
 )
 # WrongPathOrderException: 'columns' can not be without 'tables' attribute
 ```
+
 * EmptyPathValueException - raises when trying to get a path that is not set up
+
 ```python
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("tables")
 
 # EmptyPathValueException: Path 'tables' is not set up
 ```
+
 * PathDoestExistException - raises when trying to get not existing oddrn path
+
 ```python
 from oddrn_generator import PostgresqlGenerator
+
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("jobs")
 
 # PathDoestExistException: Path 'jobs' doesn't exist in generator
 ```
+
+## Development
+
+```bash
+#Install dependencies
+poetry install
+
+#Activate shell
+poetry shell
+
+# Run tests
+python run pytest
+```
+
```

