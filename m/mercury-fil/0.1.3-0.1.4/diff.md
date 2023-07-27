# Comparing `tmp/mercury_fil-0.1.3.tar.gz` & `tmp/mercury_fil-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury_fil-0.1.3.tar", max compression
+gzip compressed data, was "mercury_fil-0.1.4.tar", max compression
```

## Comparing `mercury_fil-0.1.3.tar` & `mercury_fil-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7306 2023-07-27 23:17:26.874462 mercury_fil-0.1.3/README.md
--rw-r--r--   0        0        0      602 2023-07-27 23:22:15.188431 mercury_fil-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-21 06:08:07.446477 mercury_fil-0.1.3/src/mercury/__init__.py
--rw-r--r--   0        0        0     7601 2023-07-27 23:22:05.960866 mercury_fil-0.1.3/src/mercury/client.py
--rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 mercury_fil-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7306 2023-07-27 23:17:26.874462 mercury_fil-0.1.4/README.md
+-rw-r--r--   0        0        0      602 2023-07-27 23:41:59.748739 mercury_fil-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-21 06:08:07.446477 mercury_fil-0.1.4/src/mercury/__init__.py
+-rw-r--r--   0        0        0     7626 2023-07-27 23:41:33.504548 mercury_fil-0.1.4/src/mercury/client.py
+-rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 mercury_fil-0.1.4/PKG-INFO
```

### Comparing `mercury_fil-0.1.3/README.md` & `mercury_fil-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mercury_fil-0.1.3/src/mercury/client.py` & `mercury_fil-0.1.4/src/mercury/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         if dry_run:
             bytes = self._bqc.query(
                 query, job_config=self._dry_run_config
             ).total_bytes_processed
             return to_gib(bytes)
 
-        return pd.read_gbq(query)
+        return pd.read_gbq(query, project_id=self.project)
 
     @property
     def project(self):
         return self._project
 
     @cache
     def fevm_contracts(
```

### Comparing `mercury_fil-0.1.3/PKG-INFO` & `mercury_fil-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-fil
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python client for accessing Filecoin chain data.
 License: MIT, Apache-2.0
 Keywords: filecoin,bigquery
 Author: Steph Samson
 Author-email: ayo@kasteph.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

