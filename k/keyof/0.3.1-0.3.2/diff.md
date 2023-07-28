# Comparing `tmp/keyof-0.3.1.tar.gz` & `tmp/keyof-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyof-0.3.1.tar", max compression
+gzip compressed data, was "keyof-0.3.2.tar", max compression
```

## Comparing `keyof-0.3.1.tar` & `keyof-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-26 06:50:31.381683 keyof-0.3.1/LICENSE
--rw-r--r--   0        0        0     1700 2023-07-28 06:23:24.822710 keyof-0.3.1/README.md
--rw-r--r--   0        0        0      974 2023-07-28 06:08:21.488849 keyof-0.3.1/keyof/__init__.py
--rw-r--r--   0        0        0      123 2023-07-28 05:59:12.275609 keyof-0.3.1/keyof/compat.py
--rw-r--r--   0        0        0     3039 2023-07-28 06:08:21.566648 keyof-0.3.1/keyof/mypy_plugin.py
--rw-r--r--   0        0        0        0 2023-07-26 06:50:01.388419 keyof-0.3.1/keyof/py.typed
--rw-r--r--   0        0        0     2164 2023-07-28 06:23:45.246361 keyof-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 keyof-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 06:50:31.381683 keyof-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1712 2023-07-28 06:25:30.985553 keyof-0.3.2/README.md
+-rw-r--r--   0        0        0      974 2023-07-28 06:08:21.488849 keyof-0.3.2/keyof/__init__.py
+-rw-r--r--   0        0        0      123 2023-07-28 05:59:12.275609 keyof-0.3.2/keyof/compat.py
+-rw-r--r--   0        0        0     3039 2023-07-28 06:08:21.566648 keyof-0.3.2/keyof/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:50:01.388419 keyof-0.3.2/keyof/py.typed
+-rw-r--r--   0        0        0     2164 2023-07-28 06:25:46.203098 keyof-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 keyof-0.3.2/PKG-INFO
```

### Comparing `keyof-0.3.1/LICENSE` & `keyof-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keyof-0.3.1/README.md` & `keyof-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 ```toml
 [tool.mypy]
 plugins = ["keyof.mypy_plugin"]
 ```
 
 ## Features
 
-✅ `KeyOf`, `RequiredKeyOf`, and `NotRequiredKeyOf` types
-✅ Supports inheritance
-✅ Plays nicely with other types, e.g. `KeyOf[Foo] | Literal["bar"]`
-✅ Compatibility module for `Pylance` and `Pyright`
-✅ Zero dependencies
+- ✅ `KeyOf`, `RequiredKeyOf`, and `NotRequiredKeyOf` types
+- ✅ Supports inheritance
+- ✅ Plays nicely with other types, e.g. `KeyOf[Foo] | Literal["bar"]`
+- ✅ Compatibility module for `Pylance` and `Pyright`
+- ✅ Zero dependencies
 
-❌ Generic `TypeVar` arguments
+- ❌ Generic `TypeVar` arguments
 
 ## Usage
 
 ```python
 from typing import TypedDict
 
 from keyof import KeyOf
```

### Comparing `keyof-0.3.1/keyof/__init__.py` & `keyof-0.3.2/keyof/__init__.py`

 * *Files identical despite different names*

### Comparing `keyof-0.3.1/keyof/mypy_plugin.py` & `keyof-0.3.2/keyof/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `keyof-0.3.1/pyproject.toml` & `keyof-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keyof"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Viliam Valent <keyof@valent.email>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ViliamV/keyof"
 homepage = "https://github.com/ViliamV/keyof"
 packages = [{include = "keyof"}]
```

### Comparing `keyof-0.3.1/PKG-INFO` & `keyof-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyof
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/ViliamV/keyof
 License: MIT
 Author: Viliam Valent
 Author-email: keyof@valent.email
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -37,21 +37,21 @@
 ```toml
 [tool.mypy]
 plugins = ["keyof.mypy_plugin"]
 ```
 
 ## Features
 
-✅ `KeyOf`, `RequiredKeyOf`, and `NotRequiredKeyOf` types
-✅ Supports inheritance
-✅ Plays nicely with other types, e.g. `KeyOf[Foo] | Literal["bar"]`
-✅ Compatibility module for `Pylance` and `Pyright`
-✅ Zero dependencies
+- ✅ `KeyOf`, `RequiredKeyOf`, and `NotRequiredKeyOf` types
+- ✅ Supports inheritance
+- ✅ Plays nicely with other types, e.g. `KeyOf[Foo] | Literal["bar"]`
+- ✅ Compatibility module for `Pylance` and `Pyright`
+- ✅ Zero dependencies
 
-❌ Generic `TypeVar` arguments
+- ❌ Generic `TypeVar` arguments
 
 ## Usage
 
 ```python
 from typing import TypedDict
 
 from keyof import KeyOf
```

