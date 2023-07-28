# Comparing `tmp/ftmq-0.1.5.tar.gz` & `tmp/ftmq-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.1.5.tar", max compression
+gzip compressed data, was "ftmq-0.1.6.tar", max compression
```

## Comparing `ftmq-0.1.5.tar` & `ftmq-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.5/LICENSE
--rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.5/README.md
--rw-r--r--   0        0        0       22 2023-07-28 05:11:44.990689 ftmq-0.1.5/ftmq/__init__.py
--rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.5/ftmq/cli.py
--rw-r--r--   0        0        0      287 2023-07-27 16:03:41.306274 ftmq-0.1.5/ftmq/enums.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.5/ftmq/exceptions.py
--rw-r--r--   0        0        0     4982 2023-07-28 04:09:12.400103 ftmq-0.1.5/ftmq/filters.py
--rw-r--r--   0        0        0     2151 2023-07-26 18:11:21.346315 ftmq-0.1.5/ftmq/io.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.5/ftmq/query.py
--rw-r--r--   0        0        0      556 2023-07-28 05:01:23.599175 ftmq-0.1.5/ftmq/types.py
--rw-r--r--   0        0        0      973 2023-07-28 04:58:52.872628 ftmq-0.1.5/ftmq/util.py
--rw-r--r--   0        0        0     1415 2023-07-28 05:11:44.990689 ftmq-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5652 1970-01-01 00:00:00.000000 ftmq-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 05:24:37.608824 ftmq-0.1.6/ftmq/__init__.py
+-rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.6/ftmq/cli.py
+-rw-r--r--   0        0        0      287 2023-07-27 16:03:41.306274 ftmq-0.1.6/ftmq/enums.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.6/ftmq/exceptions.py
+-rw-r--r--   0        0        0     4982 2023-07-28 04:09:12.400103 ftmq-0.1.6/ftmq/filters.py
+-rw-r--r--   0        0        0     2151 2023-07-26 18:11:21.346315 ftmq-0.1.6/ftmq/io.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.6/ftmq/query.py
+-rw-r--r--   0        0        0      564 2023-07-28 05:20:05.583374 ftmq-0.1.6/ftmq/types.py
+-rw-r--r--   0        0        0      973 2023-07-28 04:58:52.872628 ftmq-0.1.6/ftmq/util.py
+-rw-r--r--   0        0        0     1415 2023-07-28 05:24:37.608824 ftmq-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5652 1970-01-01 00:00:00.000000 ftmq-0.1.6/PKG-INFO
```

### Comparing `ftmq-0.1.5/LICENSE` & `ftmq-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/README.md` & `ftmq-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/ftmq/cli.py` & `ftmq-0.1.6/ftmq/cli.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/ftmq/filters.py` & `ftmq-0.1.6/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/ftmq/io.py` & `ftmq-0.1.6/ftmq/io.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/ftmq/query.py` & `ftmq-0.1.6/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/ftmq/types.py` & `ftmq-0.1.6/ftmq/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 
 # composite entity generator
 CEGenerator: TypeAlias = Generator[CE, None, None]
 
 StrGenerator: TypeAlias = Generator[str, None, None]
 BytesGenerator: TypeAlias = Generator[bytes, None, None]
 
-Schemata: TypeAlias = Literal[*[s.name for s in Schemata]]
-Properties: TypeAlias = Literal[*[p.name for p in Properties]]
+Schemata: TypeAlias = Literal[tuple(s.name for s in Schemata)]
+Properties: TypeAlias = Literal[tuple(p.name for p in Properties)]
```

### Comparing `ftmq-0.1.5/ftmq/util.py` & `ftmq-0.1.6/ftmq/util.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.5/pyproject.toml` & `ftmq-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.1.5"
+version = "0.1.6"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
```

### Comparing `ftmq-0.1.5/PKG-INFO` & `ftmq-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.1.5
+Version: 0.1.6
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Developers
```

