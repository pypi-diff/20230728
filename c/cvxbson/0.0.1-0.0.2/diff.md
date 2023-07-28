# Comparing `tmp/cvxbson-0.0.1.tar.gz` & `tmp/cvxbson-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxbson-0.0.1.tar", max compression
+gzip compressed data, was "cvxbson-0.0.2.tar", max compression
```

## Comparing `cvxbson-0.0.1.tar` & `cvxbson-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10790 2023-07-27 21:29:11.152535 cvxbson-0.0.1/LICENSE
--rw-r--r--   0        0        0     2588 2023-07-27 21:29:11.156535 cvxbson-0.0.1/README.md
--rw-r--r--   0        0        0       64 2023-07-27 21:29:11.156535 cvxbson-0.0.1/cvx/bson/__init__.py
--rw-r--r--   0        0        0     1975 2023-07-27 21:29:11.156535 cvxbson-0.0.1/cvx/bson/file.py
--rw-r--r--   0        0        0       64 2023-07-27 21:29:11.156535 cvxbson-0.0.1/cvx/json/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-27 21:29:11.156535 cvxbson-0.0.1/cvx/json/file.py
--rw-r--r--   0        0        0     1067 2023-07-27 21:29:40.561944 cvxbson-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 cvxbson-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-07-28 00:17:43.443217 cvxbson-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2588 2023-07-28 00:17:43.443217 cvxbson-0.0.2/README.md
+-rw-r--r--   0        0        0       40 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/bson/__init__.py
+-rw-r--r--   0        0        0     1951 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/bson/file.py
+-rw-r--r--   0        0        0       40 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/json/__init__.py
+-rw-r--r--   0        0        0     1009 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/json/file.py
+-rw-r--r--   0        0        0     1066 2023-07-28 00:18:18.889892 cvxbson-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 cvxbson-0.0.2/PKG-INFO
```

### Comparing `cvxbson-0.0.1/LICENSE` & `cvxbson-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxbson-0.0.1/README.md` & `cvxbson-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cvxbson-0.0.1/cvx/bson/file.py` & `cvxbson-0.0.2/cvx/bson/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Tools to support working with bson files and strings
 """
 from __future__ import annotations
 
 from os import PathLike
 from typing import Any, Dict, Union
```

### Comparing `cvxbson-0.0.1/cvx/json/file.py` & `cvxbson-0.0.2/cvx/json/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Tools to support working with json files
 """
 import json
 from collections.abc import Iterable
 from os import PathLike
 from typing import Any, Dict, Union
@@ -17,15 +16,15 @@
 FILE = Union[str, bytes, PathLike]
 MATRIX: TypeAlias = npt.NDArray[Any]
 DATA = Dict[str, Any]
 
 
 def read_json(json_file: FILE) -> DATA:
     """Read a json file and return a genaerator of key-value pairs"""
-    with open(json_file, "r") as f:
+    with open(json_file) as f:
         json_data = json.load(f)
         d = {}
         for name, data in json_data.items():
             if isinstance(data, Iterable):
                 d[name] = np.asarray(data)
             else:
                 d[name] = data
```

### Comparing `cvxbson-0.0.1/pyproject.toml` & `cvxbson-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxbson"
-version = "v0.0.1"
+version = "v0.0.2"
 description = "Dealing with json and bson files"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxbson"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
@@ -35,15 +35,14 @@
 loguru = "*"
 fire = "*"
 
 
 [tool.poetry.group.stubs.dependencies]
 mypy = "*"
 
-
 [tool.poetry.scripts]
 weather-fire = "cli.weather_fire:main"
 smallest-eigenvalue = "cli.smallest_eigenvalue:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cvxbson-0.0.1/PKG-INFO` & `cvxbson-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxbson
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dealing with json and bson files
 Home-page: https://github.com/cvxgrp/cvxbson
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

