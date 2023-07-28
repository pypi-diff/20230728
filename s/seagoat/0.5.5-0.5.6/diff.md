# Comparing `tmp/seagoat-0.5.5.tar.gz` & `tmp/seagoat-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.5.5.tar", max compression
+gzip compressed data, was "seagoat-0.5.6.tar", max compression
```

## Comparing `seagoat-0.5.5.tar` & `seagoat-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-23 11:33:18.356000 seagoat-0.5.5/LICENSE
--rw-r--r--   0        0        0      957 2023-07-23 11:33:18.356000 seagoat-0.5.5/README.md
--rw-r--r--   0        0        0     3028 2023-07-23 11:33:19.340005 seagoat-0.5.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/cache.py
--rw-r--r--   0        0        0     2859 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/common.py
--rw-r--r--   0        0        0     4512 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/result.py
--rw-r--r--   0        0        0     5624 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/server.py
--rw-r--r--   0        0        0     1878 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1210 2023-07-23 11:33:18.360000 seagoat-0.5.5/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 seagoat-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-28 11:20:56.366351 seagoat-0.5.6/LICENSE
+-rw-r--r--   0        0        0      957 2023-07-28 11:20:56.366351 seagoat-0.5.6/README.md
+-rw-r--r--   0        0        0     3056 2023-07-28 11:20:57.306421 seagoat-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/cache.py
+-rw-r--r--   0        0        0     2859 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/common.py
+-rw-r--r--   0        0        0     4512 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/result.py
+-rw-r--r--   0        0        0     5624 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/server.py
+-rw-r--r--   0        0        0     1878 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1210 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 seagoat-0.5.6/PKG-INFO
```

### Comparing `seagoat-0.5.5/LICENSE` & `seagoat-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/README.md` & `seagoat-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/pyproject.toml` & `seagoat-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.5.5"
+version = "0.5.6"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
@@ -46,14 +46,15 @@
 pytest-flask = "^1.2.0"
 exceptiongroup = "^1.1.2"
 pytest-mock = "^3.11.1"
 pytest-fast-first = "^1.0.5"
 pytest-sugar = "^0.9.7"
 pytest-testmon = "^2.0.12"
 pytest-leaks = "^0.3.1"
+mkdocs-material = "^9.1.19"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 venvPath = "."
```

### Comparing `seagoat-0.5.5/seagoat/cache.py` & `seagoat-0.5.6/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/cli.py` & `seagoat-0.5.6/seagoat/cli.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/engine.py` & `seagoat-0.5.6/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/file.py` & `seagoat-0.5.6/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/repository.py` & `seagoat-0.5.6/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/result.py` & `seagoat-0.5.6/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/server.py` & `seagoat-0.5.6/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/sources/chroma.py` & `seagoat-0.5.6/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/seagoat/sources/ripgrep.py` & `seagoat-0.5.6/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.5/PKG-INFO` & `seagoat-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.5.5
+Version: 0.5.6
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

