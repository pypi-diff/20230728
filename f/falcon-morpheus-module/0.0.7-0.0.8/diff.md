# Comparing `tmp/falcon_morpheus_module-0.0.7.tar.gz` & `tmp/falcon_morpheus_module-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_morpheus_module-0.0.7.tar", max compression
+gzip compressed data, was "falcon_morpheus_module-0.0.8.tar", max compression
```

## Comparing `falcon_morpheus_module-0.0.7.tar` & `falcon_morpheus_module-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6251 2023-06-19 14:55:37.712701 falcon_morpheus_module-0.0.7/README.md
--rw-r--r--   0        0        0       61 2023-06-19 14:55:37.712701 falcon_morpheus_module-0.0.7/falcon_morpheus_module/__init__.py
--rw-r--r--   0        0        0     7266 2023-06-19 14:55:37.712701 falcon_morpheus_module-0.0.7/falcon_morpheus_module/dock_sftp_api.py
--rw-r--r--   0        0        0      325 2023-06-19 14:55:37.712701 falcon_morpheus_module-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6251 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/README.md
+-rw-r--r--   0        0        0       61 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/falcon_morpheus_module/__init__.py
+-rw-r--r--   0        0        0     7314 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/falcon_morpheus_module/dock_sftp_api.py
+-rw-r--r--   0        0        0      325 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.8/PKG-INFO
```

### Comparing `falcon_morpheus_module-0.0.7/README.md` & `falcon_morpheus_module-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `falcon_morpheus_module-0.0.7/falcon_morpheus_module/dock_sftp_api.py` & `falcon_morpheus_module-0.0.8/falcon_morpheus_module/dock_sftp_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
             json={
                 "query": query_string,
                 "variables": {},
             },
         )
 
         if response.status_code != 200:
+            print("Reponse: ", response.json())
             raise Exception(f"Request failed with status code: {response.status_code}")
 
         return {
             "response": response.json(),
             "x-ticket": response.headers.get("x-ticket"),
         }
```

### Comparing `falcon_morpheus_module-0.0.7/PKG-INFO` & `falcon_morpheus_module-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-morpheus-module
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

