# Comparing `tmp/keyof-0.3.2.tar.gz` & `tmp/keyof-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyof-0.3.2.tar", max compression
+gzip compressed data, was "keyof-0.3.3.tar", max compression
```

## Comparing `keyof-0.3.2.tar` & `keyof-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-26 06:50:31.381683 keyof-0.3.2/LICENSE
--rw-r--r--   0        0        0     1712 2023-07-28 06:25:30.985553 keyof-0.3.2/README.md
--rw-r--r--   0        0        0      974 2023-07-28 06:08:21.488849 keyof-0.3.2/keyof/__init__.py
--rw-r--r--   0        0        0      123 2023-07-28 05:59:12.275609 keyof-0.3.2/keyof/compat.py
--rw-r--r--   0        0        0     3039 2023-07-28 06:08:21.566648 keyof-0.3.2/keyof/mypy_plugin.py
--rw-r--r--   0        0        0        0 2023-07-26 06:50:01.388419 keyof-0.3.2/keyof/py.typed
--rw-r--r--   0        0        0     2164 2023-07-28 06:25:46.203098 keyof-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 keyof-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 06:50:31.381683 keyof-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1712 2023-07-28 06:25:30.985553 keyof-0.3.3/README.md
+-rw-r--r--   0        0        0      974 2023-07-28 06:08:21.488849 keyof-0.3.3/keyof/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-28 13:20:32.977131 keyof-0.3.3/keyof/compat.py
+-rw-r--r--   0        0        0     3039 2023-07-28 06:08:21.566648 keyof-0.3.3/keyof/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:50:01.388419 keyof-0.3.3/keyof/py.typed
+-rw-r--r--   0        0        0     2198 2023-07-28 13:22:04.252925 keyof-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 keyof-0.3.3/PKG-INFO
```

### Comparing `keyof-0.3.2/LICENSE` & `keyof-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keyof-0.3.2/README.md` & `keyof-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `keyof-0.3.2/keyof/__init__.py` & `keyof-0.3.3/keyof/__init__.py`

 * *Files identical despite different names*

### Comparing `keyof-0.3.2/keyof/mypy_plugin.py` & `keyof-0.3.3/keyof/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `keyof-0.3.2/pyproject.toml` & `keyof-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keyof"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Viliam Valent <keyof@valent.email>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ViliamV/keyof"
 homepage = "https://github.com/ViliamV/keyof"
 packages = [{include = "keyof"}]
@@ -70,14 +70,15 @@
 cache-dir = ".cache/ruff"
 line-length = 120
 target-version = "py311"
 # Never enforce line length violations
 ignore = ["E501"]
 format = "grouped"
 extend-exclude = [".cache"]
+ignore-init-module-imports = true
 
 [tool.poe.tasks]
 
 [tool.poe.tasks.clean]
 help = "Remove generated files"
 cmd = """
     rm -rf .coverage
```

### Comparing `keyof-0.3.2/PKG-INFO` & `keyof-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyof
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://github.com/ViliamV/keyof
 License: MIT
 Author: Viliam Valent
 Author-email: keyof@valent.email
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

