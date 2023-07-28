# Comparing `tmp/retakesearch-0.1.15.tar.gz` & `tmp/retakesearch-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.15.tar", max compression
+gzip compressed data, was "retakesearch-0.1.16.tar", max compression
```

## Comparing `retakesearch-0.1.15.tar` & `retakesearch-0.1.16.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-27 17:31:42.520071 retakesearch-0.1.15/README.md
--rw-r--r--   0        0        0      412 2023-07-27 17:32:04.096430 retakesearch-0.1.15/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/__init__.py
--rw-r--r--   0        0        0     1277 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/client.py
--rw-r--r--   0        0        0     2571 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/search.py
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-28 19:30:10.064584 retakesearch-0.1.16/README.md
+-rw-r--r--   0        0        0      412 2023-07-28 19:30:31.536681 retakesearch-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-28 19:30:10.064584 retakesearch-0.1.16/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1277 2023-07-28 19:30:10.064584 retakesearch-0.1.16/retakesearch/client.py
+-rw-r--r--   0        0        0     3204 2023-07-28 19:30:10.064584 retakesearch-0.1.16/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-07-28 19:30:10.064584 retakesearch-0.1.16/retakesearch/search.py
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.16/PKG-INFO
```

### Comparing `retakesearch-0.1.15/retakesearch/client.py` & `retakesearch-0.1.16/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.15/retakesearch/index.py` & `retakesearch-0.1.16/retakesearch/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import httpx
 
 from opensearchpy import Search
-from typing import Any, List
+from typing import Any, List, Dict, Union
 
 
 class Database:
     def __init__(self, host: str, user: str, password: str, port: int):
         self.host = host
         self.user = user
         self.password = password
@@ -62,18 +62,36 @@
             return str(exc)
 
     def search(self, search: Search) -> Any:
         json = {
             "dsl": search.to_dict(),  # type: ignore
             "index_name": self.index_name,
         }
+
         try:
             with httpx.Client(timeout=None) as http:
                 response = http.post(
                     f"{self.url}/index/search", headers=self.headers, json=json
                 )
                 response.raise_for_status()
                 return response.json()
         except httpx.HTTPStatusError as exc:
             return exc.response.json()
         except Exception as exc:
             return str(exc)
+
+    def upsert(
+        self, documents: List[Dict[str, Any]], ids: List[Union[str, int]]
+    ) -> Any:
+        json = {"index_name": self.index_name, "documents": documents, "ids": ids}
+
+        try:
+            with httpx.Client(timeout=None) as http:
+                response = http.post(
+                    f"{self.url}/index/upsert", headers=self.headers, json=json
+                )
+                response.raise_for_status()
+                return response.json()
+        except httpx.HTTPStatusError as exc:
+            return exc.response.json()
+        except Exception as exc:
+            return str(exc)
```

### Comparing `retakesearch-0.1.15/PKG-INFO` & `retakesearch-0.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.15
+Version: 0.1.16
 Summary: Open Source Neural Search Engine Python Client
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

