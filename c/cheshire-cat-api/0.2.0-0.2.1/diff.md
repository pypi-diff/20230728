# Comparing `tmp/cheshire_cat_api-0.2.0.tar.gz` & `tmp/cheshire_cat_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheshire_cat_api-0.2.0.tar", max compression
+gzip compressed data, was "cheshire_cat_api-0.2.1.tar", max compression
```

## Comparing `cheshire_cat_api-0.2.0.tar` & `cheshire_cat_api-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10701 2023-07-28 21:43:44.518515 cheshire_cat_api-0.2.0/README.md
--rw-r--r--   0        0        0     1862 2023-07-28 21:43:44.518515 cheshire_cat_api-0.2.0/cheshire_cat_api/__init__.py
--rw-r--r--   0        0        0      591 2023-07-28 21:43:44.518515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/__init__.py
--rw-r--r--   0        0        0    36993 2023-07-28 21:43:44.518515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/memory_api.py
--rw-r--r--   0        0        0    42623 2023-07-28 21:43:44.518515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/plugins_api.py
--rw-r--r--   0        0        0    22463 2023-07-28 21:43:44.518515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/rabbit_hole_api.py
--rw-r--r--   0        0        0    13212 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_embedder_api.py
--rw-r--r--   0        0        0    31434 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_general_api.py
--rw-r--r--   0        0        0    13128 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_large_language_model_api.py
--rw-r--r--   0        0        0     6437 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_prompt_api.py
--rw-r--r--   0        0        0     6284 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api/status_api.py
--rw-r--r--   0        0        0    29994 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api_client.py
--rw-r--r--   0        0        0      844 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/api_response.py
--rw-r--r--   0        0        0     4550 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/cat_client.py
--rw-r--r--   0        0        0    14352 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/configuration.py
--rw-r--r--   0        0        0     5281 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/exceptions.py
--rw-r--r--   0        0        0      643 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/models/__init__.py
--rw-r--r--   0        0        0     2636 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/models/body_upload_url.py
--rw-r--r--   0        0        0     2378 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/models/http_validation_error.py
--rw-r--r--   0        0        0     4587 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/models/location_inner.py
--rw-r--r--   0        0        0     2008 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/models/setting_body.py
--rw-r--r--   0        0        0     2450 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/models/validation_error.py
--rw-r--r--   0        0        0        0 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/py.typed
--rw-r--r--   0        0        0    12853 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/rest.py
--rw-r--r--   0        0        0     1959 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/cheshire_cat_api/utils.py
--rw-r--r--   0        0        0     1028 2023-07-28 21:43:44.522515 cheshire_cat_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    11819 1970-01-01 00:00:00.000000 cheshire_cat_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10701 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/README.md
+-rw-r--r--   0        0        0     1862 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/__init__.py
+-rw-r--r--   0        0        0      591 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/__init__.py
+-rw-r--r--   0        0        0    36993 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/memory_api.py
+-rw-r--r--   0        0        0    42623 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/plugins_api.py
+-rw-r--r--   0        0        0    22463 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/rabbit_hole_api.py
+-rw-r--r--   0        0        0    13212 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_embedder_api.py
+-rw-r--r--   0        0        0    31434 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_general_api.py
+-rw-r--r--   0        0        0    13128 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_large_language_model_api.py
+-rw-r--r--   0        0        0     6437 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_prompt_api.py
+-rw-r--r--   0        0        0     6284 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api/status_api.py
+-rw-r--r--   0        0        0    29994 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api_client.py
+-rw-r--r--   0        0        0      844 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/api_response.py
+-rw-r--r--   0        0        0     4550 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/cat_client.py
+-rw-r--r--   0        0        0    14352 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/configuration.py
+-rw-r--r--   0        0        0     5281 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/exceptions.py
+-rw-r--r--   0        0        0      643 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/models/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/models/body_upload_url.py
+-rw-r--r--   0        0        0     2378 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/models/http_validation_error.py
+-rw-r--r--   0        0        0     4587 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/models/location_inner.py
+-rw-r--r--   0        0        0     2008 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/models/setting_body.py
+-rw-r--r--   0        0        0     2450 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/models/validation_error.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/py.typed
+-rw-r--r--   0        0        0    12853 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/rest.py
+-rw-r--r--   0        0        0     1959 2023-07-28 21:48:28.740687 cheshire_cat_api-0.2.1/cheshire_cat_api/utils.py
+-rw-r--r--   0        0        0     1028 2023-07-28 21:48:28.744687 cheshire_cat_api-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11819 1970-01-01 00:00:00.000000 cheshire_cat_api-0.2.1/PKG-INFO
```

### Comparing `cheshire_cat_api-0.2.0/README.md` & `cheshire_cat_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/__init__.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/__init__.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/memory_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/memory_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/plugins_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/plugins_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/rabbit_hole_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/rabbit_hole_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_embedder_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_embedder_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_general_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_general_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_large_language_model_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_large_language_model_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/settings_prompt_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/settings_prompt_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api/status_api.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api/status_api.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api_client.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api_client.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/api_response.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/api_response.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/cat_client.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/cat_client.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/configuration.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/configuration.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/exceptions.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/models/__init__.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/models/body_upload_url.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/models/body_upload_url.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/models/http_validation_error.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/models/location_inner.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/models/setting_body.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/models/setting_body.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/models/validation_error.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/rest.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/rest.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/cheshire_cat_api/utils.py` & `cheshire_cat_api-0.2.1/cheshire_cat_api/utils.py`

 * *Files identical despite different names*

### Comparing `cheshire_cat_api-0.2.0/pyproject.toml` & `cheshire_cat_api-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cheshire_cat_api"
-version = "0.2.0"
+version = "0.2.1"
 description = "😸 Cheshire-Cat API Client"
 authors = ["Chesire Cat AI"]
 maintainers = [
     "Nicola Corbellini"
 ]
 homepage = "https://cheshirecat.ai/"
 license = "GPL-3.0-only"
```

### Comparing `cheshire_cat_api-0.2.0/PKG-INFO` & `cheshire_cat_api-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheshire-cat-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: 😸 Cheshire-Cat API Client
 Home-page: https://cheshirecat.ai/
 License: GPL-3.0-only
 Keywords: OpenAPI,Cheshire-Cat,LLM,Open Source
 Author: Chesire Cat AI
 Maintainer: Nicola Corbellini
 Requires-Python: >=3.7,<4.0
```

