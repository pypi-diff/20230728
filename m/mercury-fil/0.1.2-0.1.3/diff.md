# Comparing `tmp/mercury_fil-0.1.2.tar.gz` & `tmp/mercury_fil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury_fil-0.1.2.tar", max compression
+gzip compressed data, was "mercury_fil-0.1.3.tar", max compression
```

## Comparing `mercury_fil-0.1.2.tar` & `mercury_fil-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7306 2023-07-27 23:17:26.874462 mercury_fil-0.1.2/README.md
--rw-r--r--   0        0        0      602 2023-07-27 23:19:16.999719 mercury_fil-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-21 06:08:07.446477 mercury_fil-0.1.2/src/mercury/__init__.py
--rw-r--r--   0        0        0     7630 2023-07-27 23:17:05.268256 mercury_fil-0.1.2/src/mercury/client.py
--rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 mercury_fil-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7306 2023-07-27 23:17:26.874462 mercury_fil-0.1.3/README.md
+-rw-r--r--   0        0        0      602 2023-07-27 23:22:15.188431 mercury_fil-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-21 06:08:07.446477 mercury_fil-0.1.3/src/mercury/__init__.py
+-rw-r--r--   0        0        0     7601 2023-07-27 23:22:05.960866 mercury_fil-0.1.3/src/mercury/client.py
+-rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 mercury_fil-0.1.3/PKG-INFO
```

### Comparing `mercury_fil-0.1.2/README.md` & `mercury_fil-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mercury_fil-0.1.2/pyproject.toml` & `mercury_fil-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mercury-fil"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python client for accessing Filecoin chain data."
 authors = ["Steph Samson <ayo@kasteph.com>"]
 license = "MIT, Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "mercury", from = "src" },
 ]
```

### Comparing `mercury_fil-0.1.2/src/mercury/client.py` & `mercury_fil-0.1.3/src/mercury/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
     bq_project: str = "protocol-labs-data"
     dataset: str = "lily"
 
     def __init__(
         self,
     ) -> None:
-        credentials, self._project = google.auth.default()
-        self._project = self._project or self.bq_project
+        credentials, _ = google.auth.default()
+        self._project = self.bq_project
         
         pandas_gbq.context.credentials = credentials
         pandas_gbq.context.project = self._project
         
         self._bqc = bigquery.Client()
         self._dry_run_config = bigquery.QueryJobConfig(
             dry_run=True, use_query_cache=False
```

### Comparing `mercury_fil-0.1.2/PKG-INFO` & `mercury_fil-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-fil
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for accessing Filecoin chain data.
 License: MIT, Apache-2.0
 Keywords: filecoin,bigquery
 Author: Steph Samson
 Author-email: ayo@kasteph.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

