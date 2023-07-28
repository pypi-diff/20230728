# Comparing `tmp/exergenics-etl-1.6.0.tar.gz` & `tmp/exergenics-etl-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.6.0.tar", last modified: Thu Jul 27 00:19:47 2023, max compression
+gzip compressed data, was "exergenics-etl-1.6.1.tar", last modified: Fri Jul 28 03:37:34 2023, max compression
```

## Comparing `exergenics-etl-1.6.0.tar` & `exergenics-etl-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    43240 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 00:19:46.000000 exergenics-etl-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.265580 exergenics-etl-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58210 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43240 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 03:37:34.265580 exergenics-etl-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-28 03:37:32.000000 exergenics-etl-1.6.1/setup.py
```

### Comparing `exergenics-etl-1.6.0/LICENSE` & `exergenics-etl-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.0/app/exergenics_etl/__init__.py` & `exergenics-etl-1.6.1/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.6.1/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,15 +614,15 @@
                         errorMessage = 'The table in this file is in a long format. ' \
                             + f'This column (column name = \"{nameColumnName}\") is detected to be a variable name column. '
                         logger.error(errorMessage)
                         raise EtlError(errorMessage, namesColumnId, valuesColumnId)
 
         return True
 
-    def check_input_dataframe(self, df: pd.DataFrame) -> bool:
+    def check_input_dataframe(self, df: pd.DataFrame, timestampColumnNames: List[str]) -> bool:
         """Validate the format of a dataframe read from a data file.
 
         Args:
             df (pd.DataFrame): Pandas DataFrame to validate timestamp and 
             wide format. 
 
         Raises:
@@ -633,15 +633,15 @@
             bool: True if all validations are passed.
         """
 
         logger = Logger()
 
         try:
             self._validate_timestamp_column_header(df)
-            self._check_for_wide_format(df)
+            self._check_for_wide_format(df, timestampColumnNames)
         except EtlError as e:
             raise EtlError(e)
         except Exception as e:
             msg = f'Unknown error: {e}'
             logger.error(msg)
             raise e
```

### Comparing `exergenics-etl-1.6.0/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.6.1/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.0/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.6.1/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.6.1/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.0/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.6.1/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.0/setup.py` & `exergenics-etl-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.6.0",
+    version="v1.6.1",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

