# Comparing `tmp/quickbase-client-0.6.2.tar.gz` & `tmp/quickbase_client-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbase-client-0.6.2.tar", max compression
+gzip compressed data, was "quickbase_client-0.6.3.tar", max compression
```

## Comparing `quickbase-client-0.6.2.tar` & `quickbase_client-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1084 2022-04-09 23:52:19.129891 quickbase-client-0.6.2/LICENSE.md
--rw-r--r--   0        0        0     6690 2023-06-06 17:43:13.601663 quickbase-client-0.6.2/README.rst
--rw-r--r--   0        0        0     1624 2023-06-22 15:38:15.284114 quickbase-client-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1805 2023-06-06 17:43:13.606541 quickbase-client-0.6.2/src/quickbase_client/__init__.py
--rw-r--r--   0        0        0      326 2022-04-09 23:52:19.134446 quickbase-client-0.6.2/src/quickbase_client/__version__.py
--rw-r--r--   0        0        0      154 2023-06-06 17:43:13.606831 quickbase-client-0.6.2/src/quickbase_client/client/__init__.py
--rw-r--r--   0        0        0     3402 2023-06-06 17:43:13.607099 quickbase-client-0.6.2/src/quickbase_client/client/api.py
--rw-r--r--   0        0        0     3381 2023-06-06 17:43:13.607412 quickbase-client-0.6.2/src/quickbase_client/client/legacy_client.py
--rw-r--r--   0        0        0      954 2023-06-06 17:43:13.607675 quickbase-client-0.6.2/src/quickbase_client/client/pager.py
--rw-r--r--   0        0        0     2541 2023-06-06 17:43:13.608053 quickbase-client-0.6.2/src/quickbase_client/client/request_factory.py
--rw-r--r--   0        0        0     8488 2023-06-06 17:43:13.608349 quickbase-client-0.6.2/src/quickbase_client/client/table_client.py
--rw-r--r--   0        0        0       85 2023-01-10 13:22:49.818758 quickbase-client-0.6.2/src/quickbase_client/orm/__init__.py
--rw-r--r--   0        0        0      226 2023-06-06 17:43:13.608591 quickbase-client-0.6.2/src/quickbase_client/orm/app.py
--rw-r--r--   0        0        0     3197 2023-06-06 17:43:13.608834 quickbase-client-0.6.2/src/quickbase_client/orm/field.py
--rw-r--r--   0        0        0      221 2023-06-06 17:43:13.609088 quickbase-client-0.6.2/src/quickbase_client/orm/report.py
--rw-r--r--   0        0        0     2738 2023-06-06 17:43:13.609366 quickbase-client-0.6.2/src/quickbase_client/orm/serialize.py
--rw-r--r--   0        0        0     3819 2023-06-06 17:43:13.609682 quickbase-client-0.6.2/src/quickbase_client/orm/table.py
--rw-r--r--   0        0        0     1334 2022-04-09 23:52:19.135570 quickbase-client-0.6.2/src/quickbase_client/query/__init__.py
--rw-r--r--   0        0        0     3678 2023-06-06 17:43:13.609996 quickbase-client-0.6.2/src/quickbase_client/query/ast.py
--rw-r--r--   0        0        0     1015 2023-06-06 17:43:13.610281 quickbase-client-0.6.2/src/quickbase_client/query/query_base.py
--rw-r--r--   0        0        0     1054 2023-06-06 17:43:13.610590 quickbase-client-0.6.2/src/quickbase_client/query/query_utils.py
--rw-r--r--   0        0        0      102 2022-04-09 23:52:19.135975 quickbase-client-0.6.2/src/quickbase_client/tools/__init__.py
--rw-r--r--   0        0        0     2693 2023-06-06 17:43:13.610985 quickbase-client-0.6.2/src/quickbase_client/tools/log_handler.py
--rw-r--r--   0        0        0     9684 2023-06-06 17:43:13.611315 quickbase-client-0.6.2/src/quickbase_client/tools/model_generate.py
--rw-r--r--   0        0        0     1480 2022-04-09 23:52:19.136280 quickbase-client-0.6.2/src/quickbase_client/tools/qbc.py
--rw-r--r--   0        0        0      314 2022-04-09 23:52:19.136349 quickbase-client-0.6.2/src/quickbase_client/tools/script.py
--rw-r--r--   0        0        0      883 2022-04-09 23:52:19.136438 quickbase-client-0.6.2/src/quickbase_client/tools/script_loader.py
--rw-r--r--   0        0        0        0 2022-04-09 23:52:19.136532 quickbase-client-0.6.2/src/quickbase_client/utils/__init__.py
--rw-r--r--   0        0        0     2725 2022-04-09 23:52:19.136632 quickbase-client-0.6.2/src/quickbase_client/utils/pywriting_utils.py
--rw-r--r--   0        0        0     2521 2023-06-22 15:40:21.740870 quickbase-client-0.6.2/src/quickbase_client/utils/string_utils.py
--rw-r--r--   0        0        0     8000 2023-06-22 15:41:27.159476 quickbase-client-0.6.2/setup.py
--rw-r--r--   0        0        0     7955 2023-06-22 15:41:27.159855 quickbase-client-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-04-09 23:52:19.129891 quickbase_client-0.6.3/LICENSE.md
+-rw-r--r--   0        0        0     6690 2023-06-06 17:43:13.601663 quickbase_client-0.6.3/README.rst
+-rw-r--r--   0        0        0     1624 2023-07-28 13:40:26.843369 quickbase_client-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1805 2023-06-06 17:43:13.606541 quickbase_client-0.6.3/src/quickbase_client/__init__.py
+-rw-r--r--   0        0        0      326 2022-04-09 23:52:19.134446 quickbase_client-0.6.3/src/quickbase_client/__version__.py
+-rw-r--r--   0        0        0      154 2023-06-06 17:43:13.606831 quickbase_client-0.6.3/src/quickbase_client/client/__init__.py
+-rw-r--r--   0        0        0     3402 2023-06-06 17:43:13.607099 quickbase_client-0.6.3/src/quickbase_client/client/api.py
+-rw-r--r--   0        0        0     3388 2023-07-28 13:37:08.107925 quickbase_client-0.6.3/src/quickbase_client/client/legacy_client.py
+-rw-r--r--   0        0        0      954 2023-06-06 17:43:13.607675 quickbase_client-0.6.3/src/quickbase_client/client/pager.py
+-rw-r--r--   0        0        0     2541 2023-06-06 17:43:13.608053 quickbase_client-0.6.3/src/quickbase_client/client/request_factory.py
+-rw-r--r--   0        0        0     8488 2023-06-06 17:43:13.608349 quickbase_client-0.6.3/src/quickbase_client/client/table_client.py
+-rw-r--r--   0        0        0       85 2023-01-10 13:22:49.818758 quickbase_client-0.6.3/src/quickbase_client/orm/__init__.py
+-rw-r--r--   0        0        0      226 2023-06-06 17:43:13.608591 quickbase_client-0.6.3/src/quickbase_client/orm/app.py
+-rw-r--r--   0        0        0     3197 2023-06-06 17:43:13.608834 quickbase_client-0.6.3/src/quickbase_client/orm/field.py
+-rw-r--r--   0        0        0      221 2023-06-06 17:43:13.609088 quickbase_client-0.6.3/src/quickbase_client/orm/report.py
+-rw-r--r--   0        0        0     2738 2023-06-06 17:43:13.609366 quickbase_client-0.6.3/src/quickbase_client/orm/serialize.py
+-rw-r--r--   0        0        0     3819 2023-06-06 17:43:13.609682 quickbase_client-0.6.3/src/quickbase_client/orm/table.py
+-rw-r--r--   0        0        0     1334 2022-04-09 23:52:19.135570 quickbase_client-0.6.3/src/quickbase_client/query/__init__.py
+-rw-r--r--   0        0        0     3678 2023-06-06 17:43:13.609996 quickbase_client-0.6.3/src/quickbase_client/query/ast.py
+-rw-r--r--   0        0        0     1015 2023-06-06 17:43:13.610281 quickbase_client-0.6.3/src/quickbase_client/query/query_base.py
+-rw-r--r--   0        0        0     1054 2023-06-06 17:43:13.610590 quickbase_client-0.6.3/src/quickbase_client/query/query_utils.py
+-rw-r--r--   0        0        0      102 2022-04-09 23:52:19.135975 quickbase_client-0.6.3/src/quickbase_client/tools/__init__.py
+-rw-r--r--   0        0        0     2693 2023-06-06 17:43:13.610985 quickbase_client-0.6.3/src/quickbase_client/tools/log_handler.py
+-rw-r--r--   0        0        0     9684 2023-06-06 17:43:13.611315 quickbase_client-0.6.3/src/quickbase_client/tools/model_generate.py
+-rw-r--r--   0        0        0     1480 2022-04-09 23:52:19.136280 quickbase_client-0.6.3/src/quickbase_client/tools/qbc.py
+-rw-r--r--   0        0        0      314 2022-04-09 23:52:19.136349 quickbase_client-0.6.3/src/quickbase_client/tools/script.py
+-rw-r--r--   0        0        0      883 2022-04-09 23:52:19.136438 quickbase_client-0.6.3/src/quickbase_client/tools/script_loader.py
+-rw-r--r--   0        0        0        0 2022-04-09 23:52:19.136532 quickbase_client-0.6.3/src/quickbase_client/utils/__init__.py
+-rw-r--r--   0        0        0     2725 2022-04-09 23:52:19.136632 quickbase_client-0.6.3/src/quickbase_client/utils/pywriting_utils.py
+-rw-r--r--   0        0        0     2521 2023-06-22 15:40:21.740870 quickbase_client-0.6.3/src/quickbase_client/utils/string_utils.py
+-rw-r--r--   0        0        0     8006 1970-01-01 00:00:00.000000 quickbase_client-0.6.3/PKG-INFO
```

### Comparing `quickbase-client-0.6.2/LICENSE.md` & `quickbase_client-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/README.rst` & `quickbase_client-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/pyproject.toml` & `quickbase_client-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbase-client"
-version = "0.6.2"
+version = "0.6.3"
 description = "A Quickbase Python API Client Generator"
 authors = ["Tim Kutcher <tim@tkutcher.com>"]
 maintainers = ["Tim Kutcher <tim@tkutcher.com>"]
 readme = "README.rst"
 license = "LICENSE.md"
 homepage = "https://github.com/tkutcher/quickbase-client"
 repository = "https://github.com/tkutcher/quickbase-client"
```

### Comparing `quickbase-client-0.6.2/src/quickbase_client/__init__.py` & `quickbase_client-0.6.3/src/quickbase_client/__init__.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/client/api.py` & `quickbase_client-0.6.3/src/quickbase_client/client/api.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/client/legacy_client.py` & `quickbase_client-0.6.3/src/quickbase_client/client/legacy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         </qdbapi>
         """
         headers = {
             "Content-Type": "application/xml",
             "QUICKBASE-ACTION": quickbase_action,
         }
         url = f"https://{self.realm_hostname}/{endpoint.lstrip('/')}"
-        self.session.request(
+        return self.session.request(
             method=http_method,
             url=url,
             headers=headers,
             data=data_xml,
         )
 
     # Common Use Cases:
```

### Comparing `quickbase-client-0.6.2/src/quickbase_client/client/pager.py` & `quickbase_client-0.6.3/src/quickbase_client/client/pager.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/client/request_factory.py` & `quickbase_client-0.6.3/src/quickbase_client/client/request_factory.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/client/table_client.py` & `quickbase_client-0.6.3/src/quickbase_client/client/table_client.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/orm/field.py` & `quickbase_client-0.6.3/src/quickbase_client/orm/field.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/orm/serialize.py` & `quickbase_client-0.6.3/src/quickbase_client/orm/serialize.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/orm/table.py` & `quickbase_client-0.6.3/src/quickbase_client/orm/table.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/query/__init__.py` & `quickbase_client-0.6.3/src/quickbase_client/query/__init__.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/query/ast.py` & `quickbase_client-0.6.3/src/quickbase_client/query/ast.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/query/query_base.py` & `quickbase_client-0.6.3/src/quickbase_client/query/query_base.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/query/query_utils.py` & `quickbase_client-0.6.3/src/quickbase_client/query/query_utils.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/tools/log_handler.py` & `quickbase_client-0.6.3/src/quickbase_client/tools/log_handler.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/tools/model_generate.py` & `quickbase_client-0.6.3/src/quickbase_client/tools/model_generate.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/tools/qbc.py` & `quickbase_client-0.6.3/src/quickbase_client/tools/qbc.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/tools/script_loader.py` & `quickbase_client-0.6.3/src/quickbase_client/tools/script_loader.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/utils/pywriting_utils.py` & `quickbase_client-0.6.3/src/quickbase_client/utils/pywriting_utils.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/src/quickbase_client/utils/string_utils.py` & `quickbase_client-0.6.3/src/quickbase_client/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.2/PKG-INFO` & `quickbase_client-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbase-client
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Quickbase Python API Client Generator
 Home-page: https://github.com/tkutcher/quickbase-client
 License: LICENSE.md
 Keywords: quickbase,client,quickbase-api,orm,generator
 Author: Tim Kutcher
 Author-email: tim@tkutcher.com
 Maintainer: Tim Kutcher
@@ -12,18 +12,19 @@
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/tkutcher/quickbase-client/issues
 Project-URL: Documentation, https://quickbase-client.readthedocs.io/en/latest/?badge=latest
 Project-URL: Repository, https://github.com/tkutcher/quickbase-client
 Description-Content-Type: text/x-rst
```

