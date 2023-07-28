# Comparing `tmp/dsds-0.0.23.tar.gz` & `tmp/dsds-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.23.tar", last modified: Fri Jul 28 04:34:34 2023, max compression
+gzip compressed data, was "dsds-0.0.24.tar", last modified: Fri Jul 28 04:51:50 2023, max compression
```

## Comparing `dsds-0.0.23.tar` & `dsds-0.0.24.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.077995 dsds-0.0.23/
--rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.23/LICENSE
--rw-rw-rw-   0        0        0     9216 2023-07-28 04:34:34.077995 dsds-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     6844 2023-07-27 22:37:38.000000 dsds-0.0.23/README.md
--rw-rw-rw-   0        0        0     1398 2023-07-24 20:26:15.000000 dsds-0.0.23/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 04:34:34.077995 dsds-0.0.23/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.019562 dsds-0.0.23/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.058757 dsds-0.0.23/src/dsds/
--rw-rw-rw-   0        0        0       87 2023-07-23 18:27:29.000000 dsds-0.0.23/src/dsds/__init__.py
--rw-rw-rw-   0        0        0    14049 2023-07-27 04:22:14.000000 dsds-0.0.23/src/dsds/blueprint.py
--rw-rw-rw-   0        0        0      206 2023-07-27 04:58:44.000000 dsds-0.0.23/src/dsds/compare.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.23/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    26636 2023-07-27 05:09:06.000000 dsds-0.0.23/src/dsds/encoders.py
--rw-rw-rw-   0        0        0    37634 2023-07-25 05:03:42.000000 dsds-0.0.23/src/dsds/fs.py
--rw-rw-rw-   0        0        0    11007 2023-07-26 03:13:51.000000 dsds-0.0.23/src/dsds/metrics.py
--rw-rw-rw-   0        0        0    38259 2023-07-28 04:30:11.000000 dsds-0.0.23/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0    20414 2023-07-27 15:49:24.000000 dsds-0.0.23/src/dsds/sample.py
--rw-rw-rw-   0        0        0    28954 2023-07-28 04:16:34.000000 dsds-0.0.23/src/dsds/transform.py
--rw-rw-rw-   0        0        0     3510 2023-07-28 04:29:38.000000 dsds-0.0.23/src/dsds/type_alias.py
--rw-rw-rw-   0        0        0    14259 2023-07-27 04:37:24.000000 dsds-0.0.23/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.075995 dsds-0.0.23/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     9216 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.610767 dsds-0.0.24/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.24/LICENSE
+-rw-rw-rw-   0        0        0     9216 2023-07-28 04:51:50.610767 dsds-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0     6844 2023-07-27 22:37:38.000000 dsds-0.0.24/README.md
+-rw-rw-rw-   0        0        0     1396 2023-07-28 04:45:59.000000 dsds-0.0.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:51:50.610767 dsds-0.0.24/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.577413 dsds-0.0.24/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.595138 dsds-0.0.24/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-28 04:46:03.000000 dsds-0.0.24/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0    14005 2023-07-28 04:44:23.000000 dsds-0.0.24/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0      206 2023-07-27 04:58:44.000000 dsds-0.0.24/src/dsds/compare.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.24/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    26636 2023-07-27 05:09:06.000000 dsds-0.0.24/src/dsds/encoders.py
+-rw-rw-rw-   0        0        0    37634 2023-07-25 05:03:42.000000 dsds-0.0.24/src/dsds/fs.py
+-rw-rw-rw-   0        0        0    11007 2023-07-26 03:13:51.000000 dsds-0.0.24/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    38259 2023-07-28 04:30:11.000000 dsds-0.0.24/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0    20420 2023-07-28 04:43:26.000000 dsds-0.0.24/src/dsds/sample.py
+-rw-rw-rw-   0        0        0    28954 2023-07-28 04:16:34.000000 dsds-0.0.24/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     3522 2023-07-28 04:50:51.000000 dsds-0.0.24/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0    14259 2023-07-27 04:37:24.000000 dsds-0.0.24/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.610767 dsds-0.0.24/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     9216 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.23/LICENSE` & `dsds-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/PKG-INFO` & `dsds-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.23
+Version: 0.0.24
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dsds-0.0.23/README.md` & `dsds-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/pyproject.toml` & `dsds-0.0.24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "dsds"
-version = "0.0.23"
+version = "0.0.24"
 requires-python = ">=3.9"
 readme = "README.md"
 description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
 authors = [
     {name = "Tianren Qin", email = "tq9695@gmail.com"}
 ]
 license = {file = "LICENSE"}
 dependencies = [
     "polars >= 0.18.7",
     "scipy >= 1.11.1",
-    "pandas",
     "numpy",
+    "tqdm",
     "typing_extensions >= 4.0.1"
 ]
 
 keywords = ["data pipeline", "EDA", "feature-screening", "feature-selection"]
 
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
```

### Comparing `dsds-0.0.23/src/dsds/blueprint.py` & `dsds-0.0.24/src/dsds/blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 from polars import LazyFrame, DataFrame
 from dataclasses import dataclass
 from typing import (
     Any
     , Union
     , Iterable
     , Optional
-    # , Callable
-    # , Concatenate
-    # , ParamSpec
 )
 from polars.type_aliases import IntoExpr
 from .type_alias import (
     PolarsFrame
     , ActionType
     , PipeFunction
     , ClassifModel
@@ -298,15 +295,15 @@
             Step(action = "classif", associated_data={"model":model,
                                                       "target": target,
                                                       "features": features,
                                                       "score_col":score_col})
         )
         return output
     
-    def preserve(self, path:str|Path) -> None:
+    def preserve(self, path:Union[str,Path]) -> None:
         '''
         Writes the blueprint to disk as a Python pickle file at the given path.
 
         Parameters
         ----------
         path
             A valid path to write to
@@ -345,15 +342,15 @@
                     df = df.pipe(Blueprint._process_classif, **s.associated_data)
                 elif s.action == "regression":
                     df = df.pipe(Blueprint._process_regression, **s.associated_data)
             else:
                 break
         return df
 
-def from_pkl(path: str|Path) -> Blueprint:
+def from_pkl(path: Union[str,Path]) -> Blueprint:
     with open(path, "rb") as f:
         obj = pickle.loads(f.read())
         if isinstance(obj, Blueprint):
             return obj
         else:
             raise ValueError("The pickled object is not a blueprint.")
```

### Comparing `dsds-0.0.23/src/dsds/eda_text.py` & `dsds-0.0.24/src/dsds/eda_text.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds/encoders.py` & `dsds-0.0.24/src/dsds/encoders.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds/fs.py` & `dsds-0.0.24/src/dsds/fs.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds/metrics.py` & `dsds-0.0.24/src/dsds/metrics.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds/prescreen.py` & `dsds-0.0.24/src/dsds/prescreen.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds/sample.py` & `dsds-0.0.24/src/dsds/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     output = df.unique(subset=subset, keep = keep)
     if isinstance(df, pl.LazyFrame) and persist:
         return output.blueprint.add_func(df, deduplicate, kwargs = {"subset":subset,"keep":keep})
     return output
 
 def simple_upsample(
     df: PolarsFrame
-    , subgroup: dict[str, list] | pl.Expr
+    , subgroup: Union[dict[str, list], pl.Expr]
     , count:int
     , epsilon: float = 1e-2
     , include: Optional[list[str]] = None
     , exclude: Optional[list[str]] = None
     , positive: bool = False
     , seed: int = 42
     , persist: bool = False
```

### Comparing `dsds-0.0.23/src/dsds/transform.py` & `dsds-0.0.24/src/dsds/transform.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds/type_alias.py` & `dsds-0.0.24/src/dsds/type_alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import (
     Literal
     , Final
     , Tuple
     , Union
+    , Callable
 )
 from abc import ABC, abstractmethod
 import polars as pl
 import sys
 if sys.version_info >= (3, 10):
-    from typing import TypeAlias, Concatenate, ParamSpec, Callable
+    from typing import TypeAlias, Concatenate, ParamSpec
     P = ParamSpec('P')
     PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
     PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
-else:
+else: # 3.9
     from typing_extensions import TypeAlias
     PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
     PipeFunction = Callable
 
 import os
 import numpy as np
```

### Comparing `dsds-0.0.23/src/dsds/utils.py` & `dsds-0.0.24/src/dsds/utils.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.23/src/dsds.egg-info/PKG-INFO` & `dsds-0.0.24/src/dsds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.23
+Version: 0.0.24
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

