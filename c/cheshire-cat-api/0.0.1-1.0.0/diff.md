# Comparing `tmp/cheshire-cat-api-0.0.1.tar.gz` & `tmp/cheshire-cat-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheshire-cat-api-0.0.1.tar", last modified: Thu Jul 27 22:32:17 2023, max compression
+gzip compressed data, was "cheshire-cat-api-1.0.0.tar", last modified: Thu Jul 27 22:18:30 2023, max compression
```

## Comparing `cheshire-cat-api-0.0.1.tar` & `cheshire-cat-api-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:17.413105 cheshire-cat-api-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 22:32:17.413105 cheshire-cat-api-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:17.401104 cheshire-cat-api-0.0.1/cheshire_cat_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:17.405104 cheshire-cat-api-0.0.1/cheshire_cat_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36993 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/memory_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42623 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/plugins_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21931 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/rabbit_hole_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_embedder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31434 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_general_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_large_language_model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_prompt_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api/status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29994 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/cat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:17.405104 cheshire-cat-api-0.0.1/cheshire_cat_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/models/body_upload_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/models/location_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/models/setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/cheshire_cat_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:17.401104 cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 22:32:17.000000 cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-27 22:32:17.000000 cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:32:17.000000 cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 22:32:17.000000 cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 22:32:17.000000 cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 22:32:17.413105 cheshire-cat-api-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:32:17.413105 cheshire-cat-api-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_body_upload_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_location_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_memory_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_plugins_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_rabbit_hole_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_settings_embedder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_settings_general_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_settings_large_language_model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_settings_prompt_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-27 22:32:01.000000 cheshire-cat-api-0.0.1/test/test_validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:30.183534 cheshire-cat-api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 22:18:30.183534 cheshire-cat-api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:30.179534 cheshire-cat-api-1.0.0/cheshire_cat_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:30.183534 cheshire-cat-api-1.0.0/cheshire_cat_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36993 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/memory_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42623 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/plugins_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21931 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/rabbit_hole_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_embedder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31434 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_general_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_large_language_model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_prompt_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api/status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29994 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/cat_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:30.183534 cheshire-cat-api-1.0.0/cheshire_cat_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/models/body_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/models/location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/models/setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/cheshire_cat_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:30.179534 cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 22:18:30.000000 cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-27 22:18:30.000000 cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:18:30.000000 cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 22:18:30.000000 cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 22:18:30.000000 cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 22:18:30.187534 cheshire-cat-api-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:18:30.183534 cheshire-cat-api-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_body_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_memory_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_plugins_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_rabbit_hole_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_settings_embedder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_settings_general_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_settings_large_language_model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_settings_prompt_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-27 22:18:13.000000 cheshire-cat-api-1.0.0/test/test_validation_error.py
```

### Comparing `cheshire-cat-api-0.0.1/README.md` & `cheshire-cat-api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/__init__.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.5
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.29"
 
 from .cat_client import CatClient
 
 # import apis into sdk package
 from cheshire_cat_api.api.memory_api import MemoryApi
 from cheshire_cat_api.api.plugins_api import PluginsApi
 from cheshire_cat_api.api.rabbit_hole_api import RabbitHoleApi
```

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/__init__.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/memory_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/memory_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/plugins_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/plugins_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/rabbit_hole_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/rabbit_hole_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_embedder_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_embedder_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_general_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_general_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_large_language_model_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_large_language_model_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/settings_prompt_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/settings_prompt_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api/status_api.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api/status_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api_client.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api_client.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/api_response.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/api_response.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/cat_client.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/cat_client.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/configuration.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.5\n"\
-               "SDK Package Version: 0.0.1".\
+               "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/exceptions.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/models/__init__.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/models/body_upload_url.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/models/body_upload_url.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/models/http_validation_error.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/models/location_inner.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/models/setting_body.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/models/setting_body.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/models/validation_error.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/rest.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/rest.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api/utils.py` & `cheshire-cat-api-1.0.0/cheshire_cat_api/utils.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/cheshire_cat_api.egg-info/SOURCES.txt` & `cheshire-cat-api-1.0.0/cheshire_cat_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/pyproject.toml` & `cheshire-cat-api-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/setup.py` & `cheshire-cat-api-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "cheshire-cat-api"
-VERSION = "0.0.1"
-PYTHON_REQUIRES = ">=3.10"
+VERSION = "1.0.0"
+PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
-    "aenum",
-    "websocket-client >=1.6.1"
+    "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="😸 Cheshire-Cat API",
     author="OpenAPI Generator community",
```

### Comparing `cheshire-cat-api-0.0.1/test/test_body_upload_url.py` & `cheshire-cat-api-1.0.0/test/test_body_upload_url.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_http_validation_error.py` & `cheshire-cat-api-1.0.0/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_location_inner.py` & `cheshire-cat-api-1.0.0/test/test_location_inner.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_memory_api.py` & `cheshire-cat-api-1.0.0/test/test_memory_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_plugins_api.py` & `cheshire-cat-api-1.0.0/test/test_plugins_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_rabbit_hole_api.py` & `cheshire-cat-api-1.0.0/test/test_rabbit_hole_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_setting_body.py` & `cheshire-cat-api-1.0.0/test/test_setting_body.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_settings_embedder_api.py` & `cheshire-cat-api-1.0.0/test/test_settings_embedder_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_settings_general_api.py` & `cheshire-cat-api-1.0.0/test/test_settings_general_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_settings_large_language_model_api.py` & `cheshire-cat-api-1.0.0/test/test_settings_large_language_model_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_settings_prompt_api.py` & `cheshire-cat-api-1.0.0/test/test_settings_prompt_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_status_api.py` & `cheshire-cat-api-1.0.0/test/test_status_api.py`

 * *Files identical despite different names*

### Comparing `cheshire-cat-api-0.0.1/test/test_validation_error.py` & `cheshire-cat-api-1.0.0/test/test_validation_error.py`

 * *Files identical despite different names*

