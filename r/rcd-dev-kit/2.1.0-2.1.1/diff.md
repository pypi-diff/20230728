# Comparing `tmp/rcd_dev_kit-2.1.0.tar.gz` & `tmp/rcd_dev_kit-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcd_dev_kit-2.1.0.tar", max compression
+gzip compressed data, was "rcd_dev_kit-2.1.1.tar", max compression
```

## Comparing `rcd_dev_kit-2.1.0.tar` & `rcd_dev_kit-2.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rwxr-xr-x   0        0        0     1079 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/LICENSE
--rw-r--r--   0        0        0     6157 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/README.md
--rw-r--r--   0        0        0     3298 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      135 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/__init__.py
--rw-r--r--   0        0        0     7119 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/README.md
--rw-r--r--   0        0        0      702 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/__init__.py
--rw-r--r--   0        0        0    10194 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/directus_operator.py
--rw-r--r--   0        0        0    12653 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
--rw-r--r--   0        0        0     8970 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/gcloud_operator.py
--rw-r--r--   0        0        0      469 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/mysql_operator.py
--rw-r--r--   0        0        0    68724 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/redshift_operator.py
--rw-r--r--   0        0        0     7856 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/s3_operator.py
--rw-r--r--   0        0        0    32379 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/snowflake_operator.py
--rw-r--r--   0        0        0     1567 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/README.md
--rw-r--r--   0        0        0       73 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/__init__.py
--rw-r--r--   0        0        0     4602 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/dictionary.py
--rw-r--r--   0        0        0     2253 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
--rw-r--r--   0        0        0      632 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/README.md
--rw-r--r--   0        0        0       75 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/__init__.py
--rw-r--r--   0        0        0      530 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/debug_decorator.py
--rw-r--r--   0        0        0      628 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/functional_decorator.py
--rw-r--r--   0        0        0     3567 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/README.md
--rw-r--r--   0        0        0      270 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/__init__.py
--rw-r--r--   0        0        0      334 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_as_bytes.py
--rw-r--r--   0        0        0     1493 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_detector.py
--rw-r--r--   0        0        0     8908 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_downloader.py
--rw-r--r--   0        0        0     2118 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_operator.py
--rw-r--r--   0        0        0     1390 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_writer.py
--rw-r--r--   0        0        0     1386 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/README.md
--rw-r--r--   0        0        0      206 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/__init__.py
--rw-r--r--   0        0        0     4115 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/checker.py
--rw-r--r--   0        0        0     3178 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/detector.py
--rw-r--r--   0        0        0     1127 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/io.py
--rw-r--r--   0        0        0      579 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/manipulator.py
--rw-r--r--   0        0        0     6151 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/normalizer.py
--rw-r--r--   0        0        0       85 2023-07-28 08:25:33.669205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/__init__.py
--rw-r--r--   0        0        0    21107 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/sql2sf.py
--rw-r--r--   0        0        0     9032 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
--rw-r--r--   0        0        0        0 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/verification_utils/__init__.py
--rw-r--r--   0        0        0     1158 2023-07-28 08:25:33.673205 rcd_dev_kit-2.1.0/src/rcd_dev_kit/verification_utils/verifification.py
--rw-r--r--   0        0        0     8425 1970-01-01 00:00:00.000000 rcd_dev_kit-2.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1079 2023-07-28 10:13:37.255699 rcd_dev_kit-2.1.1/LICENSE
+-rw-r--r--   0        0        0     6157 2023-07-28 10:13:37.255699 rcd_dev_kit-2.1.1/README.md
+-rw-r--r--   0        0        0     3298 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/__init__.py
+-rw-r--r--   0        0        0     7119 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/README.md
+-rw-r--r--   0        0        0      702 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/__init__.py
+-rw-r--r--   0        0        0    10194 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/directus_operator.py
+-rw-r--r--   0        0        0    12653 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
+-rw-r--r--   0        0        0     8970 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/gcloud_operator.py
+-rw-r--r--   0        0        0      469 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/mysql_operator.py
+-rw-r--r--   0        0        0    68724 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/redshift_operator.py
+-rw-r--r--   0        0        0     7856 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/s3_operator.py
+-rw-r--r--   0        0        0    32379 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/snowflake_operator.py
+-rw-r--r--   0        0        0     1567 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/README.md
+-rw-r--r--   0        0        0       73 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/__init__.py
+-rw-r--r--   0        0        0     4602 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/dictionary.py
+-rw-r--r--   0        0        0     2253 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
+-rw-r--r--   0        0        0      632 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/README.md
+-rw-r--r--   0        0        0       75 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/__init__.py
+-rw-r--r--   0        0        0      530 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/debug_decorator.py
+-rw-r--r--   0        0        0      628 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/functional_decorator.py
+-rw-r--r--   0        0        0     3567 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/README.md
+-rw-r--r--   0        0        0      270 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_as_bytes.py
+-rw-r--r--   0        0        0     1493 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_detector.py
+-rw-r--r--   0        0        0     8908 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_downloader.py
+-rw-r--r--   0        0        0     2118 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_operator.py
+-rw-r--r--   0        0        0     1390 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_writer.py
+-rw-r--r--   0        0        0     1386 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/README.md
+-rw-r--r--   0        0        0      206 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/__init__.py
+-rw-r--r--   0        0        0     4115 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/checker.py
+-rw-r--r--   0        0        0     3178 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/detector.py
+-rw-r--r--   0        0        0     1127 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/io.py
+-rw-r--r--   0        0        0      579 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/manipulator.py
+-rw-r--r--   0        0        0     6151 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/normalizer.py
+-rw-r--r--   0        0        0       85 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/sql_utils/__init__.py
+-rw-r--r--   0        0        0    21107 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/sql_utils/sql2sf.py
+-rw-r--r--   0        0        0     9032 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
+-rw-r--r--   0        0        0        0 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/verification_utils/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-28 10:13:37.259699 rcd_dev_kit-2.1.1/src/rcd_dev_kit/verification_utils/verifification.py
+-rw-r--r--   0        0        0     8425 1970-01-01 00:00:00.000000 rcd_dev_kit-2.1.1/PKG-INFO
```

### Comparing `rcd_dev_kit-2.1.0/LICENSE` & `rcd_dev_kit-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/README.md` & `rcd_dev_kit-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/pyproject.toml` & `rcd_dev_kit-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rcd-dev-kit"
-version = "2.1.0"
+version = "2.1.1"
 description = "Interact with OIP ecosystem."
 authors = ["Davi FACANHA", "Yu LE VERN"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/README.md` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/__init__.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/directus_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/directus_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/elasticsearch_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/elasticsearch_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/gcloud_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/gcloud_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/redshift_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/redshift_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/s3_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/s3_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/database_manager/snowflake_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/database_manager/snowflake_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/README.md` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/dictionary.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/dictionary.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/dataclass_manager/raw_data_file.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/dataclass_manager/raw_data_file.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/README.md` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/debug_decorator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/debug_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/decorator_manager/functional_decorator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/decorator_manager/functional_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/README.md` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_detector.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_downloader.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_downloader.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_operator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/file_manager/file_writer.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/file_manager/file_writer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/README.md` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/checker.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/checker.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/detector.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/io.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/io.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/manipulator.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/manipulator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/pandas_manager/normalizer.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/pandas_manager/normalizer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/sql2sf.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/sql_utils/sql2sf.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/src/rcd_dev_kit/verification_utils/verifification.py` & `rcd_dev_kit-2.1.1/src/rcd_dev_kit/verification_utils/verifification.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.1.0/PKG-INFO` & `rcd_dev_kit-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcd-dev-kit
-Version: 2.1.0
+Version: 2.1.1
 Summary: Interact with OIP ecosystem.
 Home-page: https://github.com/Tekkare/rcd-dev-kit
 License: MIT
 Author: Davi FACANHA
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

