# Comparing `tmp/pyspark_helpers-0.1.3.tar.gz` & `tmp/pyspark_helpers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_helpers-0.1.3.tar", max compression
+gzip compressed data, was "pyspark_helpers-0.1.4.tar", max compression
```

## Comparing `pyspark_helpers-0.1.3.tar` & `pyspark_helpers-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      860 2023-02-23 14:17:09.687248 pyspark_helpers-0.1.3/README.md
--rw-r--r--   0        0        0      814 2023-02-23 14:26:31.733750 pyspark_helpers-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-22 22:57:51.210421 pyspark_helpers-0.1.3/pyspark_helpers/__init__.py
--rw-r--r--   0        0        0     9467 2023-02-23 14:05:08.537295 pyspark_helpers-0.1.3/pyspark_helpers/schema.py
--rw-r--r--   0        0        0     1372 2023-02-23 14:15:43.251892 pyspark_helpers-0.1.3/pyspark_helpers/utils.py
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 pyspark_helpers-0.1.3/setup.py
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pyspark_helpers-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1418 2023-03-15 06:42:36.560383 pyspark_helpers-0.1.4/README.md
+-rw-r--r--   0        0        0     1447 2023-07-28 01:26:06.897575 pyspark_helpers-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 06:42:36.561160 pyspark_helpers-0.1.4/pyspark_helpers/__init__.py
+-rw-r--r--   0        0        0    10061 2023-07-28 02:01:37.520353 pyspark_helpers-0.1.4/pyspark_helpers/schema.py
+-rw-r--r--   0        0        0     1472 2023-07-28 01:14:59.219520 pyspark_helpers-0.1.4/pyspark_helpers/utils.py
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 pyspark_helpers-0.1.4/PKG-INFO
```

### Comparing `pyspark_helpers-0.1.3/pyspark_helpers/schema.py` & `pyspark_helpers-0.1.4/pyspark_helpers/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from pyspark_helpers.utils import get_logger
-
-
+import json
+import re
 from collections import Counter
+from datetime import datetime
 from pathlib import Path
-from pyspark.sql.types import ArrayType, StructType
 from typing import Any, Dict, List, Optional, Union
-from datetime import datetime
-import json
-import re
 
+import black
+import isort
+import pyspark.sql.types as T
+
+from pyspark_helpers.utils import get_logger
 
 logger = get_logger(__name__)
 
 
 def _recurse_schema(d: Dict[str, Any]) -> List[Dict[str, Any]]:
     """Recurse schema.
 
@@ -76,15 +77,15 @@
         value (List[Any]): Array to parse.
 
     Returns:
         dict: Parsed array.
     """
 
     schemas = []
-    contains_null = False
+    contains_null = any([item is None for item in value])
 
     for item in value:
         schema: Dict[str, Any] = {
             "type": "array",
         }
         if isinstance(item, dict):
             schema["elementType"] = parse_struct(item)
@@ -124,40 +125,40 @@
         "type": "struct",
         "fields": _recurse_schema(value),
     }
 
     return schema
 
 
-def _get_pyspark_type(schema: Dict[str, Any]) -> Union[StructType, ArrayType]:
+def _get_pyspark_type(schema: Dict[str, Any]) -> Union[T.StructType, T.ArrayType]:
     """Get transform schema.
 
     Args:
         schema (Dict[str, Any]): Schema to transform.
 
     Returns:
-        Union[StructType, ArrayType]: Transformed schema.
+        Union[T.StructType, T.ArrayType]: Transformed schema.
 
     Raises:
         ValueError: If schema is not a dict or list.
     """
     _type = schema.get("type", None)
 
     ## We ignore the type because mypy doesn't know that the type is
-    ## StructType or ArrayType.
+    ## T.StructType or T.ArrayType.
     if _type == "array":
-        return ArrayType  # type: ignore
+        return T.ArrayType  # type: ignore
     elif _type == "struct":
-        return StructType  # type: ignore
+        return T.StructType  # type: ignore
     else:
         raise ValueError("Schema must be dict or list.")
 
 
 def save_schema(
-    schema: Union[Dict[str, Any], ArrayType, StructType],
+    schema: Union[Dict[str, Any], T.ArrayType, T.StructType],
     output: Union[str, Path],
     overwrite: bool = False,
 ) -> None:
     """Save schema to file.
 
     Args:
         schema (Dict[str, Any]): Schema to save.
@@ -178,41 +179,55 @@
     else:
         if not output.parent.exists():
             output.parent.mkdir(parents=True, exist_ok=True)
         output_path = output.parent / output.stem
 
     ext = "json"
 
-    if type(schema) is ArrayType or type(schema) is StructType:
+    if type(schema) is T.ArrayType or type(schema) is T.StructType:
         print("Saving schema as python file.")
         ext = "py"
 
     write_mode = "w" if not overwrite else "w+"
 
     with open(f"{output_path}.{ext}", write_mode) as f:
         if ext == "json":
             json.dump(schema, f)
         else:
             string_schema = str(schema)
-            pyspark_types = re.findall(r"([A-Z]\w+)(Type|Field)", string_schema)
-            unique_pyspark_types = ", ".join(set(["".join(t) for t in pyspark_types]))
-            import_statement = f"from pyspark.sql.types import {unique_pyspark_types}"
-            f.write("\n\n".join([import_statement, string_schema]))
+            import_statement = get_imports(string_schema)
+            script = f"{import_statement}\n\n{string_schema}"
+            res = black.format_str(script, mode=black.FileMode())
+            print("Formatted:", res)
+            f.write(res)
+
+    return script
 
-    return None
 
+def get_imports(string_schema):
+    pyspark_types = re.findall(r"([A-Z]\w+)(Type|Field)", string_schema)
+    unique_pyspark_types = set(["".join(t) for t in pyspark_types])
 
-def get_pyspark_schema(schema: Dict[str, Any]) -> Union[StructType, ArrayType]:
+    imports = ", ".join(unique_pyspark_types)
+    import_statement = f"from pyspark.sql.types import {imports}"
+    print("Imports:", imports)
+    print("Sorted:", isort.code(string_schema))
+    print("Import statement:", import_statement)
+    print("Sorted import statement:", isort.code(import_statement))
+    return import_statement
+
+
+def get_pyspark_schema(schema: Dict[str, Any]) -> Union[T.StructType, T.ArrayType]:
     """Transform schema to pyspark schema.
 
     Args:
         schema (Dict[str, Any]): Schema to transform.
 
     Returns:
-        Union[StructType, ArrayType]: Transformed schema.
+        Union[T.StructType, T.ArrayType]: Transformed schema.
     """
     pyspark_type = _get_pyspark_type(schema)
     pyspark_schema = None
 
     try:
         logger.debug("Transforming schema to pyspark schema. {}".format(schema))
         pyspark_schema = pyspark_type.fromJson(schema)
@@ -260,17 +275,17 @@
 
     return data
 
 
 def schema_from_json(
     path: Union[str, Path],
     to_pyspark: bool = False,
-    output: Optional[Path] = None,
+    output: Optional[Union[str, Path]] = None,
     overwrite: bool = False,
-) -> Union[Dict[str, Any], ArrayType, StructType]:
+) -> Union[Dict[str, Any], T.ArrayType, T.StructType]:
     """Read schema file.
 
     Args:
         path (str): Path to schema file. Defaults to None.
         to_pyspark (bool, optional): Transform schema to pyspark schema. Defaults to False.
         output (Optional[Path], optional): Saves schema as json to this path. Defaults to None.
         overwrite (bool, optional): Overwrite existing file. Defaults to False.
@@ -282,40 +297,41 @@
     data = load_json(path)
     schema = parse_json(data)
 
     if to_pyspark is True:
         pyspark_schema = get_pyspark_schema(schema)
 
         if output is not None:
-            save_schema(pyspark_schema, output, overwrite=overwrite)
+            output = save_schema(pyspark_schema, output, overwrite=overwrite)
+            print(f"Schema saved to {output}")
 
         return pyspark_schema
 
     if output is not None:
         save_schema(schema, output, overwrite=overwrite)
 
     return schema
 
 
 def bulk_schema_from_json(
     files: Union[List[Path], List[str]],
     to_pyspark: bool = False,
     output: Optional[Path] = None,
     overwrite: bool = False,
-) -> List[Union[Dict[str, Any], ArrayType, StructType]]:
-    """Read schema file.
+) -> List[Union[Dict[str, Any], T.ArrayType, T.StructType]]:
+    """Read schema file in bulk.
 
     Args:
         files (List[Path]): List of paths to schema files.
         to_pyspark (bool, optional): Transform schema to pyspark schema. Defaults to False.
         output (Path, optional): Path to save schema. Defaults to None.
         overwrite (bool, optional): Overwrite existing file. Defaults to False.
 
     Returns:
-        Union[List[dict], List[ArrayType], List[StructType]]: List of schemas.
+        Union[List[dict], List[T.ArrayType], List[T.StructType]]: List of schemas.
     """
 
     schemas = []
 
     for _file in files:
         logger.info(f"Parsing {_file}")
         schema = schema_from_json(
```

### Comparing `pyspark_helpers-0.1.3/pyspark_helpers/utils.py` & `pyspark_helpers-0.1.4/pyspark_helpers/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import tempfile
-
-from typing import Tuple
 from pathlib import Path
-from pyspark.sql import SparkSession
+from typing import Tuple
+
 from delta import configure_spark_with_delta_pip
+from pyspark.sql import SparkSession
 
 ROOT_LOGGER = logging.getLogger("pyspark_helpers")
 
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s [%(name)s.%(funcName)s:%(lineno)d] %(message)s",
     level="DEBUG",
     datefmt="%Y-%m-%d %H:%M:%S",
@@ -16,28 +16,33 @@
 
 
 def get_logger(name: str) -> logging.Logger:
     """Get logger.
 
     Args:
         name (str): Name of logger.
-        log_level (str, optional): Log level. Defaults to "INFO".
 
     Returns:
         logging.Logger: Logger.
     """
     return ROOT_LOGGER.getChild(name)
 
 
 def create_spark_session() -> Tuple[SparkSession, str]:
+    """Create Spark session.
+
+    Returns:
+        Tuple[SparkSession, str]: Spark session and warehouse directory.
+    """
     logging.info("Configuring Spark session for testing environment")
     warehouse_dir = tempfile.TemporaryDirectory().name
+    warehouse_dir_uri = Path(warehouse_dir).as_uri()
     _builder = (
         SparkSession.builder.master("local[1]")
-        .config("spark.hive.metastore.warehouse.dir", Path(warehouse_dir).as_uri())
+        .config("spark.hive.metastore.warehouse.dir", warehouse_dir_uri)
         .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension")
         .config(
             "spark.sql.catalog.spark_catalog",
             "org.apache.spark.sql.delta.catalog.DeltaCatalog",
         )
     )
     spark: SparkSession = configure_spark_with_delta_pip(_builder).getOrCreate()
```

### Comparing `pyspark_helpers-0.1.3/PKG-INFO` & `pyspark_helpers-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-helpers
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of tools to help when developing PySpark applications
 Author: Jens Peder Meldgaard
 Author-email: jenspederm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -60,7 +60,33 @@
 files = [Path(f) for f in Path.glob(f"{data_dir}/*.json")]
 schemas = bulk_schema_from_jsom(files)
 
 for _file, schema in zip(files, schemas):
     print(_file.name, schema)
 ```
 
+## Guidelies for Contributing
+
+Use [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/) messages. 
+
+To help with this, I encourage you to use commitizen when making your commits. The process for this is straight forward:
+
+```sh
+# Checkout a new branch
+git checkout -b <my-new-branch>
+
+# Make changes to the code....
+
+# Add your changes
+git add <changed-file-1> <changed-file-2> ...
+
+# Run commitizen commit and follow prompts
+commitizen commit # `cz c` in short
+
+# Push branch
+git push
+
+# Open a Pull Request
+## This is done in Github
+```
+
+
```

