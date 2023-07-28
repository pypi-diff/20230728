# Comparing `tmp/wasmstore-0.1.0.tar.gz` & `tmp/wasmstore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmstore-0.1.0.tar", max compression
+gzip compressed data, was "wasmstore-0.2.0.tar", max compression
```

## Comparing `wasmstore-0.1.0.tar` & `wasmstore-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1457 2023-06-01 23:29:45.170702 wasmstore-0.1.0/LICENSE
--rw-r--r--   0        0        0       83 2023-06-01 23:29:34.762628 wasmstore-0.1.0/README.md
--rw-r--r--   0        0        0      433 2023-06-01 23:29:34.766628 wasmstore-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-01 23:29:34.766628 wasmstore-0.1.0/wasmstore/__init__.py
--rw-r--r--   0        0        0     3461 2023-06-01 23:29:34.766628 wasmstore-0.1.0/wasmstore/wasmstore.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 wasmstore-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1457 2023-07-28 19:57:30.233640 wasmstore-0.2.0/LICENSE
+-rw-r--r--   0        0        0       83 2023-07-28 19:57:15.213364 wasmstore-0.2.0/README.md
+-rw-r--r--   0        0        0      433 2023-07-28 19:57:15.213364 wasmstore-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-28 19:57:15.213364 wasmstore-0.2.0/wasmstore/__init__.py
+-rw-r--r--   0        0        0     3461 2023-07-28 19:57:15.213364 wasmstore-0.2.0/wasmstore/wasmstore.py
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 wasmstore-0.2.0/PKG-INFO
```

### Comparing `wasmstore-0.1.0/LICENSE` & `wasmstore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmstore-0.1.0/wasmstore/wasmstore.py` & `wasmstore-0.2.0/wasmstore/wasmstore.py`

 * *Files identical despite different names*

### Comparing `wasmstore-0.1.0/PKG-INFO` & `wasmstore-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmstore
-Version: 0.1.0
+Version: 0.2.0
 Summary: Wasmstore client for Python
 License: BSD-3-Clause
 Author: Dylibso
 Author-email: oss@dylib.so
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

