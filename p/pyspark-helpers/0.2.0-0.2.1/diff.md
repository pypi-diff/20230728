# Comparing `tmp/pyspark_helpers-0.2.0.tar.gz` & `tmp/pyspark_helpers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_helpers-0.2.0.tar", max compression
+gzip compressed data, was "pyspark_helpers-0.2.1.tar", max compression
```

## Comparing `pyspark_helpers-0.2.0.tar` & `pyspark_helpers-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1418 2023-03-15 06:42:36.560383 pyspark_helpers-0.2.0/README.md
--rw-r--r--   0        0        0     1447 2023-07-28 02:13:17.917582 pyspark_helpers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 06:42:36.561160 pyspark_helpers-0.2.0/pyspark_helpers/__init__.py
--rw-r--r--   0        0        0     9745 2023-07-28 02:14:58.577114 pyspark_helpers-0.2.0/pyspark_helpers/schema.py
--rw-r--r--   0        0        0     1525 2023-07-28 02:15:58.702777 pyspark_helpers-0.2.0/pyspark_helpers/utils.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pyspark_helpers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1418 2023-03-15 06:42:36.560383 pyspark_helpers-0.2.1/README.md
+-rw-r--r--   0        0        0     1447 2023-07-28 10:49:05.093074 pyspark_helpers-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 06:42:36.561160 pyspark_helpers-0.2.1/pyspark_helpers/__init__.py
+-rw-r--r--   0        0        0     9769 2023-07-28 10:48:06.525372 pyspark_helpers-0.2.1/pyspark_helpers/schema.py
+-rw-r--r--   0        0        0     1525 2023-07-28 02:15:58.702777 pyspark_helpers-0.2.1/pyspark_helpers/utils.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pyspark_helpers-0.2.1/PKG-INFO
```

### Comparing `pyspark_helpers-0.2.0/README.md` & `pyspark_helpers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspark_helpers-0.2.0/pyproject.toml` & `pyspark_helpers-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspark-helpers"
-version = "0.2.0"
+version = "0.2.1"
 description = "A collection of tools to help when developing PySpark applications"
 authors = ["Jens Peder Meldgaard <jenspederm@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pyspark_helpers" }]
 
 [tool.poetry.scripts]
 psh-schema-from-json = "pyspark_helpers.schema:main"
@@ -30,15 +30,15 @@
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.isort]
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0"
+version = "0.2.1"
 version_files = ["pyproject.toml:version"]
 use_shortcuts = true
 
 [tool.black]
 line-length = 88 # Specify the line length
 target-version = ['py37'] # Specify your Python version
 include = "pyspark_helpers" # Include the files that should be formatted
```

### Comparing `pyspark_helpers-0.2.0/pyspark_helpers/schema.py` & `pyspark_helpers-0.2.1/pyspark_helpers/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,23 +187,24 @@
         print("Saving schema as python file.")
         ext = "py"
 
     write_mode = "w" if not overwrite else "w+"
 
     with open(f"{output_path}.{ext}", write_mode) as f:
         if ext == "json":
-            json.dump(schema, f)
+            output = json.dumps(schema, indent=4)
         else:
             string_schema = str(schema)
             import_statement = get_imports(string_schema)
             script = f"{import_statement}\n\n{string_schema}"
-            res = black.format_str(script, mode=black.FileMode())
-            f.write(res)
+            output = black.format_str(script, mode=black.FileMode())
 
-    return script
+        f.write(output)
+
+        return output
 
 
 def get_imports(string_schema):
     pyspark_types = re.findall(r"([A-Z]\w+)(Type|Field)", string_schema)
     unique_pyspark_types = set(["".join(t) for t in pyspark_types])
 
     imports = ", ".join(unique_pyspark_types)
```

### Comparing `pyspark_helpers-0.2.0/pyspark_helpers/utils.py` & `pyspark_helpers-0.2.1/pyspark_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_helpers-0.2.0/PKG-INFO` & `pyspark_helpers-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-helpers
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of tools to help when developing PySpark applications
 Author: Jens Peder Meldgaard
 Author-email: jenspederm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

