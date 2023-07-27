# Comparing `tmp/propertysync-0.7.0.tar.gz` & `tmp/propertysync-0.7.1.tar.gz`

## Comparing `propertysync-0.7.0.tar` & `propertysync-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 propertysync-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/__init__.py
--rw-r--r--   0        0        0    17456 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/api.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/batch.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.7.0/tests/test_batch.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.7.0/tests/test_document.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.7.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.7.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.7.0/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 propertysync-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/__init__.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.7.1/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.7.1/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.7.1/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.7.1/PKG-INFO
```

### Comparing `propertysync-0.7.0/CHANGELOG.md` & `propertysync-0.7.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/propertysync/api.py` & `propertysync-0.7.1/propertysync/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,25 +373,31 @@
     def validate_document(self, document_json):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/validate"
 
         # if document_json contains an "id" key and no "json" key, it will validate the stored copy of the document
         # if document_json contains a "json" key and no "id" key, it will validate the json
         # if document_json contains a "json" key and no "id" key and the "json" contains a "indexingRecordId" key, it will validate the stored copy of the document
 
-        # if they are passing in "json", assume they want that validated and remove any ID keys
-        if "json" in document_json and "id" in document_json:
-            del document_json["id"]
-        if "json" in document_json and "indexingRecordId" in document_json["json"]:
-            del document_json["json"]["indexingRecordId"]
+        # if they are passing in "json", assume they want that validated, create a copy of the json and remove the "id" and "indexingRecordId" keys
+
+        # create a copy of the json so that we don't modify the original document
+        new_json = None
+        if "json" in document_json:
+            new_json = {"json": document_json["json"]}
+            if "indexingRecordId" in new_json["json"]:
+                del new_json["json"]["indexingRecordId"]
+        elif "id" in document_json:
+            new_json = {"id": document_json["id"]}
+
 
         # if they are not passing in "json", assume they want the stored copy validated and ensure they have passed an ID
-        if "json" not in document_json and "id" not in document_json:
+        if "json" not in new_json and "id" not in new_json:
             raise Exception("You must pass either an ID or JSON to validate a document")
 
-        return self.api_call("POST", url, body=document_json)
+        return self.api_call("POST", url, body=new_json)
         
         
     # run a search, then create a batch and wait for the batch to fully hydrate, then retrieve the batch and optionally delete it
     def run_search_and_create_batch(self, search_query, minimum_results=1,wait_time=2,batch_name='python-api-client temp batch', delete_batch=True):
         search = self.run_search(search_query)
         search_id = search["id"]
```

### Comparing `propertysync-0.7.0/propertysync/batch.py` & `propertysync-0.7.1/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/propertysync/document.py` & `propertysync-0.7.1/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/propertysync/search.py` & `propertysync-0.7.1/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/propertysync/titlesearch_batch.py` & `propertysync-0.7.1/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/tests/test_batch.py` & `propertysync-0.7.1/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/tests/test_document.py` & `propertysync-0.7.1/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/LICENSE` & `propertysync-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/README.md` & `propertysync-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/pyproject.toml` & `propertysync-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.0/PKG-INFO` & `propertysync-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

