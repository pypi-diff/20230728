# Comparing `tmp/marqo-1.1.0.tar.gz` & `tmp/marqo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-1.1.0.tar", last modified: Mon Jul 24 07:09:36 2023, max compression
+gzip compressed data, was "marqo-1.1.1.tar", last modified: Fri Jul 28 06:39:55 2023, max compression
```

## Comparing `marqo-1.1.0.tar` & `marqo-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.437403 marqo-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-24 07:09:25.000000 marqo-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-24 07:09:36.437403 marqo-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-24 07:09:25.000000 marqo-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 07:09:25.000000 marqo-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:09:36.437403 marqo-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 07:09:25.000000 marqo-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.429403 marqo-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.433403 marqo-1.1.0/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25545 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/marqo_url_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.437403 marqo-1.1.0/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.546959 marqo-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-28 06:39:44.000000 marqo-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-28 06:39:55.546959 marqo-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-28 06:39:44.000000 marqo-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 06:39:44.000000 marqo-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 06:39:55.546959 marqo-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 06:39:44.000000 marqo-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.542959 marqo-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.542959 marqo-1.1.1/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25718 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/marqo_url_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.546959 marqo-1.1.1/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-1.1.0/LICENSE` & `marqo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/PKG-INFO` & `marqo-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 1.1.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.1.1 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

### Comparing `marqo-1.1.0/README.md` & `marqo-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/setup.py` & `marqo-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="1.1.0",
+    version="1.1.1",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-1.1.0/src/marqo/_httprequests.py` & `marqo-1.1.1/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo/client.py` & `marqo-1.1.1/src/marqo/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,26 +48,26 @@
         else:
             self.url = url
         self.config = Config(self.url, use_telemetry=return_telemetry, api_key=api_key)
         self.http = HttpRequests(self.config)
         self._marqo_minimum_supported_version_check()
 
     def create_index(
-        self, index_name: str,
-        treat_urls_and_pointers_as_images=False, model=None,
-        normalize_embeddings=True,
-        sentences_per_chunk=2,
-        sentence_overlap=0,
-        image_preprocessing_method=None,
-        settings_dict=None,
-        inference_node_type=None,
-        storage_node_type=None,
-        inference_node_count=1,
-        storage_node_count=1,
-        replicas_count=0,
+            self, index_name: str,
+            treat_urls_and_pointers_as_images=False, model=None,
+            normalize_embeddings=True,
+            sentences_per_chunk=2,
+            sentence_overlap=0,
+            image_preprocessing_method=None,
+            settings_dict=None,
+            inference_node_type=None,
+            storage_node_type=None,
+            inference_node_count=1,
+            storage_node_count=1,
+            replicas_count=0,
     ) -> Dict[str, Any]:
         """Create the index. Please refer to the marqo cloud to see options for inference and storage node types.
 
         Args:
             index_name: name of the index.
             treat_urls_and_pointers_as_images:
             model:
@@ -188,15 +188,25 @@
     ) -> str:
         return base64.urlsafe_b64encode(data).decode('utf-8').replace('=', '')
 
     def get_marqo(self):
         return self.http.get(path="")
 
     def health(self):
-        return self.http.get(path="health")
+        mq_logger.warning('The `client.health()` API has been deprecated and will be removed in '
+                          'Marqo 2.0.0. Use `client.index(index_name).health()` instead. '
+                          'Check `https://docs.marqo.ai/latest/API-Reference/indexes/` for more details.')
+        try:
+            return self.http.get(path="health")
+        except (MarqoWebError, RequestException, TypeError, KeyError) as e:
+            raise errors.BadRequestError("Marqo encountered an error trying to check the health of the Marqo instance. "
+                                         "If you are trying to check the health on Marqo Cloud, please note that "
+                                         "the `client.health()` API is not supported on Marqo Cloud and will be removed in "
+                                         "Marqo 2.0.0. Please Use `client.index('your-index-name').health()` instead. "
+                                         "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details.")
 
     def eject_model(self, model_name: str, model_device: str):
         return self.http.delete(path=f"models?model_name={model_name}&model_device={model_device}")
 
     def get_loaded_models(self):
         return self.http.get(path="models")
 
@@ -235,9 +245,7 @@
                                   f"{minimum_supported_marqo_version()} to function properly, but your Marqo version is {marqo_version}. "
                                   f"Please upgrade your Marqo instance to avoid potential errors. "
                                   f"If you have already changed your Marqo instance but still get this warning, please restart your Marqo client Python interpreter.")
         except (MarqoWebError, RequestException, TypeError, KeyError) as e:
             mq_logger.warning(skip_warning_message)
             marqo_url_and_version_cache[self.url] = "_skipped"
         return
-
-
```

### Comparing `marqo-1.1.0/src/marqo/config.py` & `marqo-1.1.1/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo/defaults.py` & `marqo-1.1.1/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo/errors.py` & `marqo-1.1.1/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo/index.py` & `marqo-1.1.1/src/marqo/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,7 +542,11 @@
             self.refresh()
         mq_logger.debug('completed batch ingestion.')
         return results
 
     def get_settings(self) -> dict:
         """Get all settings of the index"""
         return self.http.get(path=f"indexes/{self.index_name}/settings", index_name=self.index_name,)
+
+    def health(self) -> dict:
+        """Check the health of an index"""
+        return self.http.get(path=f"indexes/{self.index_name}/health", index_name=self.index_name)
```

### Comparing `marqo-1.1.0/src/marqo/marqo_url_resolver.py` & `marqo-1.1.1/src/marqo/marqo_url_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,12 +43,12 @@
                 f" persists."
             )
             return None
 
         if not response.ok:
             mq_logger.warning(response.text)
         response_json = response.json()
-        for index in response_json['indices']:
+        for index in response_json['results']:
             if index.get('index_status') in ["READY", "CREATING"]:
                 self._urls_mapping[index['index_status']][index['index_name']] = index.get('endpoint')
         if self._urls_mapping:
             self.timestamp = time.time()
```

### Comparing `marqo-1.1.0/src/marqo/models.py` & `marqo-1.1.1/src/marqo/models.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo/utils.py` & `marqo-1.1.1/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo/version.py` & `marqo-1.1.1/src/marqo/version.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.0/src/marqo.egg-info/PKG-INFO` & `marqo-1.1.1/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 1.1.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.1.1 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

