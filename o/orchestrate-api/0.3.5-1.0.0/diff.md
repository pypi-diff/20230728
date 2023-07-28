# Comparing `tmp/orchestrate_api-0.3.5.tar.gz` & `tmp/orchestrate_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrate_api-0.3.5.tar", max compression
+gzip compressed data, was "orchestrate_api-1.0.0.tar", max compression
```

## Comparing `orchestrate_api-0.3.5.tar` & `orchestrate_api-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      821 2023-07-28 15:51:54.740055 orchestrate_api-0.3.5/README.md
--rw-r--r--   0        0        0      165 2023-07-28 15:51:34.503908 orchestrate_api-0.3.5/orchestrate/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 15:51:34.503908 orchestrate_api-0.3.5/orchestrate/_internal/__init__.py
--rw-r--r--   0        0        0    26557 2023-07-28 15:51:34.507908 orchestrate_api-0.3.5/orchestrate/_internal/api.py
--rw-r--r--   0        0        0     1356 2023-07-28 15:51:34.507908 orchestrate_api-0.3.5/orchestrate/_internal/fhir.py
--rw-r--r--   0        0        0      261 2023-07-28 15:51:34.507908 orchestrate_api-0.3.5/orchestrate/convert.py
--rw-r--r--   0        0        0      543 2023-07-28 15:51:34.507908 orchestrate_api-0.3.5/orchestrate/insight.py
--rw-r--r--   0        0        0     8092 2023-07-28 15:51:34.507908 orchestrate_api-0.3.5/orchestrate/terminology.py
--rw-r--r--   0        0        0      848 2023-07-28 15:51:58.228083 orchestrate_api-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 orchestrate_api-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-28 15:55:05.848325 orchestrate_api-1.0.0/README.md
+-rw-r--r--   0        0        0      165 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/_internal/__init__.py
+-rw-r--r--   0        0        0    26557 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/_internal/api.py
+-rw-r--r--   0        0        0     1356 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/_internal/fhir.py
+-rw-r--r--   0        0        0      261 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/convert.py
+-rw-r--r--   0        0        0      543 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/insight.py
+-rw-r--r--   0        0        0     8092 2023-07-28 15:54:47.792434 orchestrate_api-1.0.0/orchestrate/terminology.py
+-rw-r--r--   0        0        0      848 2023-07-28 15:55:08.788314 orchestrate_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 orchestrate_api-1.0.0/PKG-INFO
```

### Comparing `orchestrate_api-0.3.5/README.md` & `orchestrate_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.5/orchestrate/_internal/api.py` & `orchestrate_api-1.0.0/orchestrate/_internal/api.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.5/orchestrate/_internal/fhir.py` & `orchestrate_api-1.0.0/orchestrate/_internal/fhir.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.5/orchestrate/insight.py` & `orchestrate_api-1.0.0/orchestrate/insight.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.5/orchestrate/terminology.py` & `orchestrate_api-1.0.0/orchestrate/terminology.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.5/pyproject.toml` & `orchestrate_api-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 keywords = ["careevolution", "rosetta", "orchestrate"]
 license = "Apache-2.0"
 name = "orchestrate-api"
 packages = [
   {include = "orchestrate"},
 ]
 readme = "README.md"
-version = "0.3.5"
+version = "1.0.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
```

### Comparing `orchestrate_api-0.3.5/PKG-INFO` & `orchestrate_api-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrate-api
-Version: 0.3.5
+Version: 1.0.0
 Summary: SDK for the Orchestrate API at rosetta.careevolution.com
 Home-page: https://rosetta-api.docs.careevolution.com/
 License: Apache-2.0
 Keywords: careevolution,rosetta,orchestrate
 Author: Jeremy Fortune
 Author-email: jeremy@careevolution.com
 Requires-Python: >=3.9,<4.0
```

