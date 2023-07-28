# Comparing `tmp/pyspark_helpers-0.1.4.tar.gz` & `tmp/pyspark_helpers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_helpers-0.1.4.tar", max compression
+gzip compressed data, was "pyspark_helpers-0.2.0.tar", max compression
```

## Comparing `pyspark_helpers-0.1.4.tar` & `pyspark_helpers-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1418 2023-03-15 06:42:36.560383 pyspark_helpers-0.1.4/README.md
--rw-r--r--   0        0        0     1447 2023-07-28 01:26:06.897575 pyspark_helpers-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 06:42:36.561160 pyspark_helpers-0.1.4/pyspark_helpers/__init__.py
--rw-r--r--   0        0        0    10061 2023-07-28 02:01:37.520353 pyspark_helpers-0.1.4/pyspark_helpers/schema.py
--rw-r--r--   0        0        0     1472 2023-07-28 01:14:59.219520 pyspark_helpers-0.1.4/pyspark_helpers/utils.py
--rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 pyspark_helpers-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1418 2023-03-15 06:42:36.560383 pyspark_helpers-0.2.0/README.md
+-rw-r--r--   0        0        0     1447 2023-07-28 02:13:17.917582 pyspark_helpers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 06:42:36.561160 pyspark_helpers-0.2.0/pyspark_helpers/__init__.py
+-rw-r--r--   0        0        0     9745 2023-07-28 02:14:58.577114 pyspark_helpers-0.2.0/pyspark_helpers/schema.py
+-rw-r--r--   0        0        0     1525 2023-07-28 02:15:58.702777 pyspark_helpers-0.2.0/pyspark_helpers/utils.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pyspark_helpers-0.2.0/PKG-INFO
```

### Comparing `pyspark_helpers-0.1.4/README.md` & `pyspark_helpers-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyspark_helpers-0.1.4/pyproject.toml` & `pyspark_helpers-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "pyspark-helpers"
-version = "0.1.4"
+version = "0.2.0"
 description = "A collection of tools to help when developing PySpark applications"
 authors = ["Jens Peder Meldgaard <jenspederm@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pyspark_helpers" }]
 
 [tool.poetry.scripts]
 psh-schema-from-json = "pyspark_helpers.schema:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyspark = "^3.3.2"
 delta-spark = "^2.2.0"
+black = "^23.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 tox = "^4.4.6"
-black = "^23.1.0"
 mypy = "^1.0.1"
 commitizen = "^2.42.0"
 pre-commit = "^3.1.0"
 isort = "^5.12.0"
 
 [tool.pytest.ini_options]
 log_cli = true
@@ -30,15 +30,15 @@
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.isort]
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.4"
+version = "0.2.0"
 version_files = ["pyproject.toml:version"]
 use_shortcuts = true
 
 [tool.black]
 line-length = 88 # Specify the line length
 target-version = ['py37'] # Specify your Python version
 include = "pyspark_helpers" # Include the files that should be formatted
```

### Comparing `pyspark_helpers-0.1.4/pyspark_helpers/schema.py` & `pyspark_helpers-0.2.0/pyspark_helpers/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 import re
 from collections import Counter
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import black
-import isort
 import pyspark.sql.types as T
 
 from pyspark_helpers.utils import get_logger
 
 logger = get_logger(__name__)
 
+TYPE_MAP = {
+    "str": "string",
+    "int": "integer",
+    "float": "double",
+    "bool": "boolean",
+}
+
 
 def _recurse_schema(d: Dict[str, Any]) -> List[Dict[str, Any]]:
     """Recurse schema.
 
     Args:
         d (Dict[str, Any]): Schema to recurse.
 
@@ -50,22 +56,16 @@
 
     Args:
         value (Any): Value to parse.
 
     Returns:
         str: Parsed value.
     """
-    type_map = {
-        "str": "string",
-        "int": "integer",
-        "float": "double",
-        "bool": "boolean",
-    }
 
-    _type = type_map.get(type(value).__name__, "string")
+    _type = TYPE_MAP.get(type(value).__name__, "string")
 
     if _type == "integer":
         if value > 2147483647:
             _type = "long"
 
     return _type
 
@@ -193,30 +193,25 @@
         if ext == "json":
             json.dump(schema, f)
         else:
             string_schema = str(schema)
             import_statement = get_imports(string_schema)
             script = f"{import_statement}\n\n{string_schema}"
             res = black.format_str(script, mode=black.FileMode())
-            print("Formatted:", res)
             f.write(res)
 
     return script
 
 
 def get_imports(string_schema):
     pyspark_types = re.findall(r"([A-Z]\w+)(Type|Field)", string_schema)
     unique_pyspark_types = set(["".join(t) for t in pyspark_types])
 
     imports = ", ".join(unique_pyspark_types)
     import_statement = f"from pyspark.sql.types import {imports}"
-    print("Imports:", imports)
-    print("Sorted:", isort.code(string_schema))
-    print("Import statement:", import_statement)
-    print("Sorted import statement:", isort.code(import_statement))
     return import_statement
 
 
 def get_pyspark_schema(schema: Dict[str, Any]) -> Union[T.StructType, T.ArrayType]:
     """Transform schema to pyspark schema.
 
     Args:
@@ -298,15 +293,14 @@
     schema = parse_json(data)
 
     if to_pyspark is True:
         pyspark_schema = get_pyspark_schema(schema)
 
         if output is not None:
             output = save_schema(pyspark_schema, output, overwrite=overwrite)
-            print(f"Schema saved to {output}")
 
         return pyspark_schema
 
     if output is not None:
         save_schema(schema, output, overwrite=overwrite)
 
     return schema
```

### Comparing `pyspark_helpers-0.1.4/pyspark_helpers/utils.py` & `pyspark_helpers-0.2.0/pyspark_helpers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Tuple
 
 from delta import configure_spark_with_delta_pip
 from pyspark.sql import SparkSession
 
 ROOT_LOGGER = logging.getLogger("pyspark_helpers")
-
+logging.getLogger("blib2to3").setLevel(logging.ERROR)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s [%(name)s.%(funcName)s:%(lineno)d] %(message)s",
     level="DEBUG",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
```

### Comparing `pyspark_helpers-0.1.4/PKG-INFO` & `pyspark_helpers-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyspark-helpers
-Version: 0.1.4
+Version: 0.2.0
 Summary: A collection of tools to help when developing PySpark applications
 Author: Jens Peder Meldgaard
 Author-email: jenspederm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: black (>=23.7.0,<24.0.0)
 Requires-Dist: delta-spark (>=2.2.0,<3.0.0)
 Requires-Dist: pyspark (>=3.3.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # PySpark Helpers
 
 A collection of tools to help when developing PySpark applications
```

