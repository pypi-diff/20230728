# Comparing `tmp/pushcart-0.1.9.tar.gz` & `tmp/pushcart-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart-0.1.9.tar", max compression
+gzip compressed data, was "pushcart-1.6.4.tar", max compression
```

## Comparing `pushcart-0.1.9.tar` & `pushcart-1.6.4.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-0.1.9/LICENSE
--rw-r--r--   0        0        0       80 2023-07-08 07:35:44.303369 pushcart-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-07-13 07:34:25.976683 pushcart-0.1.9/pushcart/__init__.py
--rw-r--r--   0        0        0    14232 2023-07-13 21:38:54.698467 pushcart-0.1.9/pushcart/metadata.py
--rw-r--r--   0        0        0     1318 2023-07-13 08:57:41.740193 pushcart-0.1.9/pushcart/utils.py
--rw-r--r--   0        0        0     2543 2023-07-13 21:42:26.395141 pushcart-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 pushcart-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-1.6.4/LICENSE
+-rw-r--r--   0        0        0       63 2023-07-13 21:53:22.768497 pushcart-1.6.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 21:50:18.218490 pushcart-1.6.4/pushcart/__init__.py
+-rw-r--r--   0        0        0      580 2023-07-13 21:50:18.218490 pushcart-1.6.4/pushcart/log_handlers/__init__.py
+-rw-r--r--   0        0        0     5969 2023-07-13 21:50:18.218490 pushcart-1.6.4/pushcart/log_handlers/delta_table_handler.py
+-rw-r--r--   0        0        0    16279 2023-07-28 10:32:58.383848 pushcart-1.6.4/pushcart/metadata.py
+-rw-r--r--   0        0        0     5295 2023-07-13 21:50:18.218490 pushcart-1.6.4/pushcart/plugins.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:32:58.383848 pushcart-1.6.4/pushcart/sources/rest_api/__init__.py
+-rw-r--r--   0        0        0    13724 2023-07-28 10:32:58.383848 pushcart-1.6.4/pushcart/sources/rest_api/request.py
+-rw-r--r--   0        0        0     3223 2023-07-28 10:32:58.383848 pushcart-1.6.4/pushcart/sources/rest_api/spark.py
+-rw-r--r--   0        0        0     1318 2023-07-13 21:50:18.218490 pushcart-1.6.4/pushcart/utils.py
+-rw-r--r--   0        0        0     2695 2023-07-28 10:46:31.050543 pushcart-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 pushcart-1.6.4/PKG-INFO
```

### Comparing `pushcart-0.1.9/LICENSE` & `pushcart-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart-0.1.9/pushcart/metadata.py` & `pushcart-1.6.4/pushcart/metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -272,14 +272,16 @@
             "source_column_name": f"{flat_parent}.{name}" if parent else name,
             "source_column_type": dtype.simpleString(),
             "dest_column_name": f"{flat_parent}_{name}" if parent else name,
             "dest_column_type": dtype.elementType.simpleString()
             if isinstance(dtype, T.ArrayType)
             else dtype.simpleString(),
             "transform_function": f'F.explode("{flat_parent}.{name}")'
+            if parent
+            else f'F.explode("{name}")'
             if isinstance(dtype, T.ArrayType)
             else self._infer(f"{parent}.{name}" if parent else name)
             if isinstance(dtype, T.StringType)
             else "",
             "default_value": "",
             "validation_rule": "",
             "validation_action": "",
@@ -381,26 +383,29 @@
         excluded_columns = (
             metadata_df.loc[tech_cols]["dest_column_name"].to_list() or None
         )
         log.info(f"Excluding technical columns: {excluded_columns}")
 
         return metadata_df.loc[~tech_cols]
 
-    def generate_code(self, keep_technical_cols: bool = False) -> str | None:
-        """Generate PySpark transformation code based on existing metadata.
+    def _prepare_metadata(
+        self,
+        keep_technical_cols: bool = False,
+    ) -> tuple[pd.DataFrame, list[str]]:
+        """Parse the metadata and keep or drop technical columns (starting with underscore).
 
         Parameters
         ----------
         keep_technical_cols : bool, optional
             Generate transformations for columns whose names start with underscore, by default False
 
         Returns
         -------
-        str | None
-            String containing runnable PySpark code
+        tuple[pd.DataFrame, list[str]]
+            Pandas DataFrame with the final set of pending transformations and list of columns to keep.
 
         Raises
         ------
         ValueError
             Can only generate code based on metadata that is present in memory.
         """
         if self.metadata_df is None:
@@ -415,15 +420,30 @@
                 "No destination columns defined in metadata. No code to generate.",
             )
             return None
 
         if not keep_technical_cols:
             mdf = self._drop_technical_cols(mdf)
 
-        transformations = mdf.sort_values(by=["column_order"]).to_dict(orient="records")
+        return mdf.sort_values(by=["column_order"]).to_dict(orient="records"), dest_cols
+
+    def generate_code(self, keep_technical_cols: bool = False) -> str | None:
+        """Generate PySpark transformation code based on existing metadata.
+
+        Parameters
+        ----------
+        keep_technical_cols : bool, optional
+            Generate transformations for columns whose names start with underscore, by default False
+
+        Returns
+        -------
+        str | None
+            String containing runnable PySpark code
+        """
+        transformations, dest_cols = self._prepare_metadata(keep_technical_cols)
         code_lines = ["df = (df"]
         for t in transformations:
             if (
                 isinstance(t["transform_function"], str)
                 and len(t["transform_function"]) > 0
             ):
                 code_lines.append(
@@ -438,7 +458,42 @@
 
         code_lines.append(f"\t.select({dest_cols}))")
         code_str = "\n" + "\n".join(code_lines)
 
         log.info(code_str)
 
         return code_str
+
+    def transform(self, keep_technical_cols: bool = False) -> DataFrame:
+        """Perform the transformations configured in the metadata table.
+
+        Parameters
+        ----------
+        keep_technical_cols : bool, optional
+            Generate transformations for columns whose names start with underscore, by default False
+
+        Returns
+        -------
+        DataFrame
+            Spark DataFrame containing the transformed data
+        """
+        transformations, dest_cols = self._prepare_metadata(keep_technical_cols)
+
+        result_df = self.data_df
+        for t in transformations:
+            if (
+                isinstance(t["transform_function"], str)
+                and len(t["transform_function"]) > 0
+            ):
+                result_df = result_df.withColumn(
+                    t["dest_column_name"],
+                    eval(t["transform_function"]),  # noqa: PGH001
+                )
+            elif (t["source_column_name"] != t["dest_column_name"]) or (
+                t["source_column_type"] != t["dest_column_type"]
+            ):
+                result_df = result_df.withColumn(
+                    t["dest_column_name"],
+                    F.col(t["source_column_name"]).cast(t["dest_column_type"]),
+                )
+
+        return result_df.select(dest_cols)
```

### Comparing `pushcart-0.1.9/pushcart/utils.py` & `pushcart-1.6.4/pushcart/utils.py`

 * *Files identical despite different names*

### Comparing `pushcart-0.1.9/pyproject.toml` & `pushcart-1.6.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -74,35 +74,41 @@
   "YTT",
 ]
 unfixable = []
 exclude = [".venv", "tests"]
 
 [tool.poetry]
 name = "pushcart"
-version = "0.1.9"
+version = "1.6.4"
 description = "Metadata transformations for Spark"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Topic :: Database :: Database Engines/Servers",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
+authlib = "^1.2.1"
+dtale = "^3.3.0"
+httpx = "^0.24.1"
 ipydatagrid = "^1.1.16"
 ipywidgets = "^8.0.7"
+kaleido = { version = "0.2.1", allow-prereleases = true }
 pandas = "^2.0.2"
 pyspark = "^3.4.1"
 python = "^3.10"
 python-dotenv = "^1.0.0"
+tqdm = "^4.65.0"
+validators = "^0.20.0"
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "*", allow-prereleases = true }
 bumpver = "^2023.1124"
 coverage = "^7.2.7"
 ipykernel = "^6.22.0"
 pytest = "^7.2.0"
@@ -112,15 +118,15 @@
 ruff = "^0.0.265"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.6.1"
+current_version = "1.6.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

