# Comparing `tmp/orchestrate_api-0.3.3.tar.gz` & `tmp/orchestrate_api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrate_api-0.3.3.tar", max compression
+gzip compressed data, was "orchestrate_api-0.3.4.tar", max compression
```

## Comparing `orchestrate_api-0.3.3.tar` & `orchestrate_api-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      821 2023-07-28 15:28:08.492465 orchestrate_api-0.3.3/README.md
--rw-r--r--   0        0        0      165 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/_internal/__init__.py
--rw-r--r--   0        0        0    26557 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/_internal/api.py
--rw-r--r--   0        0        0     1356 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/_internal/fhir.py
--rw-r--r--   0        0        0      261 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/convert.py
--rw-r--r--   0        0        0      543 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/insight.py
--rw-r--r--   0        0        0     8092 2023-07-28 15:27:41.107742 orchestrate_api-0.3.3/orchestrate/terminology.py
--rw-r--r--   0        0        0      848 2023-07-28 15:28:12.488692 orchestrate_api-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 orchestrate_api-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-28 15:34:02.960615 orchestrate_api-0.3.4/README.md
+-rw-r--r--   0        0        0      165 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/_internal/__init__.py
+-rw-r--r--   0        0        0    26557 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/_internal/api.py
+-rw-r--r--   0        0        0     1356 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/_internal/fhir.py
+-rw-r--r--   0        0        0      261 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/convert.py
+-rw-r--r--   0        0        0      543 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/insight.py
+-rw-r--r--   0        0        0     8092 2023-07-28 15:33:46.500548 orchestrate_api-0.3.4/orchestrate/terminology.py
+-rw-r--r--   0        0        0      848 2023-07-28 15:34:05.940639 orchestrate_api-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 orchestrate_api-0.3.4/PKG-INFO
```

### Comparing `orchestrate_api-0.3.3/README.md` & `orchestrate_api-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.3/orchestrate/_internal/api.py` & `orchestrate_api-0.3.4/orchestrate/_internal/api.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.3/orchestrate/_internal/fhir.py` & `orchestrate_api-0.3.4/orchestrate/_internal/fhir.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.3/orchestrate/insight.py` & `orchestrate_api-0.3.4/orchestrate/insight.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.3/orchestrate/terminology.py` & `orchestrate_api-0.3.4/orchestrate/terminology.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-0.3.3/pyproject.toml` & `orchestrate_api-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 keywords = ["careevolution", "rosetta", "orchestrate"]
 license = "Apache-2.0"
 name = "orchestrate-api"
 packages = [
   {include = "orchestrate"},
 ]
 readme = "README.md"
-version = "0.3.3"
+version = "0.3.4"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
```

### Comparing `orchestrate_api-0.3.3/PKG-INFO` & `orchestrate_api-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrate-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: SDK for the Orchestrate API at rosetta.careevolution.com
 Home-page: https://rosetta-api.docs.careevolution.com/
 License: Apache-2.0
 Keywords: careevolution,rosetta,orchestrate
 Author: Jeremy Fortune
 Author-email: jeremy@careevolution.com
 Requires-Python: >=3.9,<4.0
```

