# Comparing `tmp/dask-expr-0.1.1.tar.gz` & `tmp/dask-expr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-expr-0.1.1.tar", last modified: Fri Jul 21 07:51:37 2023, max compression
+gzip compressed data, was "dask-expr-0.1.2.tar", last modified: Fri Jul 28 08:41:23 2023, max compression
```

## Comparing `dask-expr-0.1.1.tar` & `dask-expr-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.006375 dask-expr-0.1.1/
--rw-r--r--   0 patrick    (502) staff       (20)     1516 2023-07-12 18:00:13.000000 dask-expr-0.1.1/LICENSE.txt
--rw-r--r--   0 patrick    (502) staff       (20)     4456 2023-07-21 07:51:37.006429 dask-expr-0.1.1/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)     3524 2023-07-21 07:49:20.000000 dask-expr-0.1.1/README.md
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.006761 dask-expr-0.1.1/dask_expr/
--rw-r--r--   0 patrick    (502) staff       (20)      127 2023-07-12 17:51:26.000000 dask-expr-0.1.1/dask_expr/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)     2603 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_accessor.py
--rw-r--r--   0 patrick    (502) staff       (20)     1434 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_align.py
--rw-r--r--   0 patrick    (502) staff       (20)     3683 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_categorical.py
--rw-r--r--   0 patrick    (502) staff       (20)    35504 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_collection.py
--rw-r--r--   0 patrick    (502) staff       (20)     4982 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_concat.py
--rw-r--r--   0 patrick    (502) staff       (20)    66800 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_expr.py
--rw-r--r--   0 patrick    (502) staff       (20)    15912 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_groupby.py
--rw-r--r--   0 patrick    (502) staff       (20)     9161 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_merge.py
--rw-r--r--   0 patrick    (502) staff       (20)     2169 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_quantiles.py
--rw-r--r--   0 patrick    (502) staff       (20)    18184 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_reductions.py
--rw-r--r--   0 patrick    (502) staff       (20)    11011 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_repartition.py
--rw-r--r--   0 patrick    (502) staff       (20)    27547 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_shuffle.py
--rw-r--r--   0 patrick    (502) staff       (20)      217 2023-06-27 15:57:00.000000 dask-expr-0.1.1/dask_expr/_typing.py
--rw-r--r--   0 patrick    (502) staff       (20)      732 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_util.py
--rw-r--r--   0 patrick    (502) staff       (20)      497 2023-07-21 07:51:37.006795 dask-expr-0.1.1/dask_expr/_version.py
--rw-r--r--   0 patrick    (502) staff       (20)     6228 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/datasets.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.006216 dask-expr-0.1.1/dask_expr/io/
--rw-r--r--   0 patrick    (502) staff       (20)       96 2023-05-16 14:29:09.000000 dask-expr-0.1.1/dask_expr/io/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)      980 2023-06-26 11:37:37.000000 dask-expr-0.1.1/dask_expr/io/csv.py
--rw-r--r--   0 patrick    (502) staff       (20)     3068 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/io/io.py
--rw-r--r--   0 patrick    (502) staff       (20)    33353 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/io/parquet.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.005365 dask-expr-0.1.1/dask_expr.egg-info/
--rw-r--r--   0 patrick    (502) staff       (20)     4456 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)      700 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (502) staff       (20)        1 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (502) staff       (20)       32 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/requires.txt
--rw-r--r--   0 patrick    (502) staff       (20)       10 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/top_level.txt
--rw-r--r--   0 patrick    (502) staff       (20)     1615 2023-07-21 07:49:20.000000 dask-expr-0.1.1/pyproject.toml
--rw-r--r--   0 patrick    (502) staff       (20)      230 2023-07-21 07:51:37.006650 dask-expr-0.1.1/setup.cfg
--rwxr-xr-x   0 patrick    (502) staff       (20)      194 2023-07-12 17:44:05.000000 dask-expr-0.1.1/setup.py
--rw-r--r--   0 patrick    (502) staff       (20)    86677 2023-07-12 17:47:49.000000 dask-expr-0.1.1/versioneer.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.732414 dask-expr-0.1.2/
+-rw-r--r--   0 patrick    (501) staff       (20)     1516 2023-07-21 10:19:51.000000 dask-expr-0.1.2/LICENSE.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     4558 2023-07-28 08:41:23.732477 dask-expr-0.1.2/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     3626 2023-07-26 09:32:50.000000 dask-expr-0.1.2/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.732787 dask-expr-0.1.2/dask_expr/
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2603 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_accessor.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1434 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_align.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3683 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_categorical.py
+-rw-r--r--   0 patrick    (501) staff       (20)    38879 2023-07-28 08:40:24.000000 dask-expr-0.1.2/dask_expr/_collection.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6820 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/_concat.py
+-rw-r--r--   0 patrick    (501) staff       (20)    70009 2023-07-28 08:40:24.000000 dask-expr-0.1.2/dask_expr/_expr.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15912 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_groupby.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9161 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_merge.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2169 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_quantiles.py
+-rw-r--r--   0 patrick    (501) staff       (20)    24731 2023-07-27 14:56:31.000000 dask-expr-0.1.2/dask_expr/_reductions.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11011 2023-07-27 14:56:31.000000 dask-expr-0.1.2/dask_expr/_repartition.py
+-rw-r--r--   0 patrick    (501) staff       (20)    31301 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/_shuffle.py
+-rw-r--r--   0 patrick    (501) staff       (20)      950 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/_util.py
+-rw-r--r--   0 patrick    (501) staff       (20)      497 2023-07-28 08:41:23.732828 dask-expr-0.1.2/dask_expr/_version.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6228 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/datasets.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.732221 dask-expr-0.1.2/dask_expr/io/
+-rw-r--r--   0 patrick    (501) staff       (20)       96 2023-05-12 07:18:29.000000 dask-expr-0.1.2/dask_expr/io/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      980 2023-06-27 13:49:53.000000 dask-expr-0.1.2/dask_expr/io/csv.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3068 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/io/io.py
+-rw-r--r--   0 patrick    (501) staff       (20)    33982 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/io/parquet.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.730871 dask-expr-0.1.2/dask_expr.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     4558 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)      665 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       32 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       10 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1615 2023-07-21 10:19:51.000000 dask-expr-0.1.2/pyproject.toml
+-rw-r--r--   0 patrick    (501) staff       (20)      230 2023-07-28 08:41:23.732681 dask-expr-0.1.2/setup.cfg
+-rwxr-xr-x   0 patrick    (501) staff       (20)      194 2023-07-21 10:19:51.000000 dask-expr-0.1.2/setup.py
```

### Comparing `dask-expr-0.1.1/LICENSE.txt` & `dask-expr-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/PKG-INFO` & `dask-expr-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 0.1.1
+Version: 0.1.2
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -81,14 +81,16 @@
 
 API Coverage
 ------------
 
 **`dask_expr.DataFrame`**
 
 - `abs`
+- `add_prefix`
+- `add_sufix`
 - `align`
 - `all`
 - `any`
 - `apply`
 - `assign`
 - `astype`
 - `clip`
@@ -118,22 +120,24 @@
 - `min`
 - `min`
 - `mode`
 - `nlargest`
 - `nsmallest`
 - `nunique_approx`
 - `partitions`
+- `pivot_table`
 - `prod`
 - `rename`
 - `rename_axis`
 - `repartition`
 - `replace`
 - `reset_index`
 - `round`
 - `sample`
+- `sort_values`
 - `select_dtypes`
 - `set_index`
 - `shuffle`
 - `std`
 - `sum`
 - `tail`
 - `to_parquet`
@@ -288,7 +292,11 @@
 
 
 **Unary operators (`DataFrame`, `Series`, and `Index`)**:
 
 - `__invert__`
 - `__neg__`
 - `__pos__`
+
+**Accessors**:
+
+- `CategoricalAccessor`
```

### Comparing `dask-expr-0.1.1/README.md` & `dask-expr-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
 API Coverage
 ------------
 
 **`dask_expr.DataFrame`**
 
 - `abs`
+- `add_prefix`
+- `add_sufix`
 - `align`
 - `all`
 - `any`
 - `apply`
 - `assign`
 - `astype`
 - `clip`
@@ -94,22 +96,24 @@
 - `min`
 - `min`
 - `mode`
 - `nlargest`
 - `nsmallest`
 - `nunique_approx`
 - `partitions`
+- `pivot_table`
 - `prod`
 - `rename`
 - `rename_axis`
 - `repartition`
 - `replace`
 - `reset_index`
 - `round`
 - `sample`
+- `sort_values`
 - `select_dtypes`
 - `set_index`
 - `shuffle`
 - `std`
 - `sum`
 - `tail`
 - `to_parquet`
@@ -264,7 +268,11 @@
 
 
 **Unary operators (`DataFrame`, `Series`, and `Index`)**:
 
 - `__invert__`
 - `__neg__`
 - `__pos__`
+
+**Accessors**:
+
+- `CategoricalAccessor`
```

### Comparing `dask-expr-0.1.1/dask_expr/_accessor.py` & `dask-expr-0.1.2/dask_expr/_accessor.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_align.py` & `dask-expr-0.1.2/dask_expr/_align.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_categorical.py` & `dask-expr-0.1.2/dask_expr/_categorical.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_collection.py` & `dask-expr-0.1.2/dask_expr/_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 
 import functools
 import warnings
-from collections.abc import Hashable
+from collections.abc import Callable, Hashable, Mapping
 from numbers import Number
+from typing import Any, Literal
 
 import numpy as np
 import pandas as pd
 from dask.base import DaskMethodsMixin, is_dask_collection, named_schedulers
+from dask.dataframe import methods
 from dask.dataframe.accessor import CachedAccessor
 from dask.dataframe.core import (
     _concat,
     _Frame,
     check_divisions,
     is_dataframe_like,
     is_index_like,
     is_series_like,
     new_dd_object,
 )
 from dask.dataframe.dispatch import meta_nonempty
+from dask.dataframe.utils import has_known_categories
 from dask.utils import IndexCallable, random_state_data, typename
 from fsspec.utils import stringify_path
 from tlz import first
 
 from dask_expr import _expr as expr
 from dask_expr._align import AlignPartitions
 from dask_expr._categorical import CategoricalAccessor
@@ -33,20 +36,21 @@
 from dask_expr._reductions import (
     DropDuplicates,
     Len,
     MemoryUsageFrame,
     MemoryUsageIndex,
     NLargest,
     NSmallest,
+    PivotTable,
     Unique,
     ValueCounts,
 )
 from dask_expr._repartition import Repartition
-from dask_expr._shuffle import SetIndex, SetIndexBlockwise
-from dask_expr._util import _convert_to_list
+from dask_expr._shuffle import SetIndex, SetIndexBlockwise, SortValues
+from dask_expr._util import _convert_to_list, is_scalar
 
 #
 # Utilities to wrap Expr API
 # (Helps limit boiler-plate code in collection APIs)
 #
 
 
@@ -112,15 +116,15 @@
 
     @property
     def size(self):
         return new_collection(self.expr.size)
 
     @property
     def columns(self):
-        return pd.Index(self.expr.columns, name=self._meta.columns.name)
+        return self._meta.columns
 
     def __len__(self):
         return new_collection(Len(self.expr)).compute()
 
     @property
     def nbytes(self):
         raise NotImplementedError("nbytes is not implemented on DataFrame")
@@ -824,14 +828,15 @@
         self,
         other,
         drop=True,
         sorted=False,
         npartitions: int | None = None,
         divisions=None,
         sort: bool = True,
+        upsample: float = 1.0,
     ):
         if isinstance(other, DataFrame):
             raise TypeError("other can't be of type DataFrame")
         if isinstance(other, Series):
             if other._name == self.index._name:
                 return self
         elif other == self.index.name:
@@ -857,14 +862,95 @@
         return new_collection(
             SetIndex(
                 self.expr,
                 other,
                 drop,
                 user_divisions=divisions,
                 npartitions=npartitions,
+                upsample=upsample,
+            )
+        )
+
+    def sort_values(
+        self,
+        by: str | list[str],
+        npartitions: int | None = None,
+        ascending: bool | list[bool] = True,
+        na_position: Literal["first"] | Literal["last"] = "last",
+        partition_size: float = 128e6,
+        sort_function: Callable[[pd.DataFrame], pd.DataFrame] | None = None,
+        sort_function_kwargs: Mapping[str, Any] | None = None,
+        upsample: float = 1.0,
+    ):
+        """See DataFrame.sort_values for docstring"""
+        if na_position not in ("first", "last"):
+            raise ValueError("na_position must be either 'first' or 'last'")
+        if not isinstance(by, list):
+            by = [by]
+        if any(not isinstance(b, str) for b in by):
+            raise NotImplementedError(
+                "Dataframes only support sorting by named columns which must be passed as a "
+                "string or a list of strings.\n"
+                "You passed %s" % str(by)
+            )
+
+        if not isinstance(ascending, bool):
+            # support [True] as input
+            if (
+                isinstance(ascending, list)
+                and len(ascending) == 1
+                and isinstance(ascending[0], bool)
+            ):
+                ascending = ascending[0]
+            else:
+                raise NotImplementedError(
+                    f"Dask currently only supports a single boolean for ascending. You passed {str(ascending)}"
+                )
+
+        return new_collection(
+            SortValues(
+                self.expr,
+                by,
+                ascending,
+                na_position,
+                npartitions,
+                partition_size,
+                sort_function,
+                sort_function_kwargs,
+                upsample,
+            )
+        )
+
+    def add_prefix(self, prefix):
+        return new_collection(expr.AddPrefix(self.expr, prefix))
+
+    def add_suffix(self, suffix):
+        return new_collection(expr.AddSuffix(self.expr, suffix))
+
+    def pivot_table(self, index, columns, values, aggfunc="mean"):
+        if not is_scalar(index) or index not in self._meta.columns:
+            raise ValueError("'index' must be the name of an existing column")
+        if not is_scalar(columns) or columns not in self._meta.columns:
+            raise ValueError("'columns' must be the name of an existing column")
+        if not methods.is_categorical_dtype(self._meta[columns]):
+            raise ValueError("'columns' must be category dtype")
+        if not has_known_categories(self._meta[columns]):
+            raise ValueError("'columns' categories must be known")
+
+        if not (
+            is_scalar(values)
+            and values in self._meta.columns
+            or not is_scalar(values)
+            and all(is_scalar(x) and x in self._meta.columns for x in values)
+        ):
+            raise ValueError("'values' must refer to an existing column or columns")
+
+        return new_collection(
+            PivotTable(
+                self.expr, index=index, columns=columns, values=values, aggfunc=aggfunc
             )
         )
 
 
 class Series(FrameBase):
     """Series-like Expr Collection"""
 
@@ -961,14 +1047,15 @@
         return first, ()
 
 
 def new_collection(expr):
     """Create new collection from an expr"""
 
     meta = expr._meta
+    expr._name  # Ensure backend is imported
     if is_dataframe_like(meta):
         return DataFrame(expr)
     elif is_series_like(meta):
         return Series(expr)
     elif is_index_like(meta):
         return Index(expr)
     else:
@@ -1025,17 +1112,18 @@
     ignore_metadata_file=False,
     metadata_task_size=None,
     split_row_groups="infer",
     blocksize="default",
     aggregate_files=None,
     parquet_file_extension=(".parq", ".parquet", ".pq"),
     filesystem="fsspec",
+    engine=None,
     **kwargs,
 ):
-    from dask_expr.io.parquet import ReadParquet
+    from dask_expr.io.parquet import ReadParquet, _set_parquet_engine
 
     if not isinstance(path, str):
         path = stringify_path(path)
 
     kwargs["dtype_backend"] = dtype_backend
 
     return new_collection(
@@ -1050,47 +1138,46 @@
             ignore_metadata_file=ignore_metadata_file,
             metadata_task_size=metadata_task_size,
             split_row_groups=split_row_groups,
             blocksize=blocksize,
             aggregate_files=aggregate_files,
             parquet_file_extension=parquet_file_extension,
             filesystem=filesystem,
+            engine=_set_parquet_engine(engine),
             kwargs=kwargs,
         )
     )
 
 
 def concat(
     dfs,
     axis=0,
     join="outer",
     ignore_unknown_divisions=False,
     ignore_order=False,
     **kwargs,
 ):
-    if axis == 1:
-        # TODO: implement
-        raise NotImplementedError
-    if ignore_unknown_divisions:
-        # TODO: implement
-        raise NotImplementedError
-
     if not isinstance(dfs, list):
         raise TypeError("dfs must be a list of DataFrames/Series objects")
     if len(dfs) == 0:
         raise ValueError("No objects to concatenate")
     if len(dfs) == 1:
         return dfs[0]
 
     if join not in ("inner", "outer"):
         raise ValueError("'join' must be 'inner' or 'outer'")
 
     dfs = [from_pandas(df) if not is_dask_collection(df) else df for df in dfs]
 
+    if axis == 1:
+        dfs = [df for df in dfs if len(df.columns) > 0]
+
     return new_collection(
         Concat(
             join,
             ignore_order,
             kwargs,
+            axis,
+            ignore_unknown_divisions,
             *[df.expr for df in dfs],
         )
     )
```

### Comparing `dask-expr-0.1.1/dask_expr/_concat.py` & `dask-expr-0.1.2/dask_expr/_concat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 import functools
+import warnings
 
 import pandas as pd
 from dask.dataframe import methods
 from dask.dataframe.dispatch import make_meta, meta_nonempty
+from dask.dataframe.multi import concat_and_check
 from dask.dataframe.utils import check_meta, strip_unknown_categories
 from dask.utils import apply, is_dataframe_like, is_series_like
 
-from dask_expr._expr import AsType, Expr, Projection
+from dask_expr._expr import AsType, Blockwise, Expr, Projection, are_co_aligned
 
 
 class Concat(Expr):
-    _parameters = ["join", "ignore_order", "_kwargs"]
-    _defaults = {"join": "outer", "ignore_order": False, "_kwargs": {}}
+    _parameters = [
+        "join",
+        "ignore_order",
+        "_kwargs",
+        "axis",
+        "ignore_unknown_divisions",
+    ]
+    _defaults = {
+        "join": "outer",
+        "ignore_order": False,
+        "_kwargs": {},
+        "axis": 0,
+        "ignore_unknown_divisions": False,
+    }
 
     def __str__(self):
         s = (
             "frames="
             + str(self.dependencies())
             + ", "
             + ", ".join(
@@ -57,14 +71,33 @@
                 divisions += dfs[-1].divisions
                 return divisions
 
         return [None] * (sum(df.npartitions for df in dfs) + 1)
 
     def _lower(self):
         dfs = self._frames
+        if self.axis == 1:
+            if are_co_aligned(*self._frames):
+                return ConcatUnindexed(self.ignore_order, self._kwargs, *dfs)
+
+            elif (
+                all(not df.known_divisions for df in dfs)
+                and len({df.npartitions for df in dfs}) == 1
+            ):
+                if not self.ignore_unknown_divisions:
+                    warnings.warn(
+                        "Concatenating dataframes with unknown divisions.\n"
+                        "We're assuming that the indices of each dataframes"
+                        " are \n aligned. This assumption is not generally "
+                        "safe."
+                    )
+                return ConcatUnindexed(self.ignore_order, self._kwargs, *dfs)
+            else:
+                raise NotImplementedError
+
         cast_dfs = []
         for df in dfs:
             # dtypes of all dfs need to be coherent
             # refer to https://github.com/dask/dask/issues/4685
             # and https://github.com/dask/dask/issues/5968.
             if is_dataframe_like(df.frame):
                 shared_columns = list(set(df.columns).intersection(self._meta.columns))
@@ -108,17 +141,25 @@
                 for frame, cols in zip(self._frames, columns_frame)
             ):
                 return
 
             frames = [
                 frame[cols] if cols != sorted(frame.columns) else frame
                 for frame, cols in zip(self._frames, columns_frame)
+                if len(cols) > 0
             ]
             return type(parent)(
-                type(self)(self.join, self.ignore_order, self._kwargs, *frames),
+                type(self)(
+                    self.join,
+                    self.ignore_order,
+                    self._kwargs,
+                    self.axis,
+                    self.ignore_unknown_divisions,
+                    *frames,
+                ),
                 *parent.operands[1:],
             )
 
 
 class StackPartition(Concat):
     _parameters = ["join", "ignore_order", "_kwargs"]
     _defaults = {"join": "outer", "ignore_order": False, "_kwargs": {}}
@@ -143,7 +184,24 @@
                         self._kwargs,
                     )
                 i += 1
         return dsk
 
     def _lower(self):
         return
+
+
+class ConcatUnindexed(Blockwise):
+    _parameters = ["ignore_order", "_kwargs"]
+    _defaults = {"ignore_order": False, "_kwargs": {}}
+    _keyword_only = ["ignore_order", "_kwargs"]
+
+    @functools.cached_property
+    def _meta(self):
+        return methods.concat(
+            [df._meta for df in self.dependencies()],
+            ignore_order=self.ignore_order,
+            **self.operand("_kwargs"),
+        )
+
+    def operation(self, *args, ignore_order, _kwargs):
+        return concat_and_check(args, ignore_order=ignore_order)
```

### Comparing `dask-expr-0.1.1/dask_expr/_expr.py` & `dask-expr-0.1.2/dask_expr/_expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,26 @@
         for parameter in type(self)._parameters[len(operands) :]:
             try:
                 operands.append(kwargs.pop(parameter))
             except KeyError:
                 operands.append(type(self)._defaults[parameter])
         assert not kwargs
         self.operands = operands
+        if self._required_attribute:
+            dep = next(iter(self.dependencies()))._meta
+            if not hasattr(dep, self._required_attribute):
+                # Raise a ValueError instead of AttributeError to
+                # avoid infinite recursion
+                raise ValueError(f"{dep} has no attribute {self._required_attribute}")
+
+    @property
+    def _required_attribute(self) -> str:
+        # Specify if the first `dependency` must support
+        # a specific attribute for valid behavior.
+        return None
 
     @functools.cached_property
     def ndim(self):
         meta = self._meta
         try:
             return meta.ndim
         except AttributeError:
@@ -135,14 +147,22 @@
         else:
             return max(expr._depth() for expr in self.dependencies()) + 1
 
     def __getattr__(self, key):
         try:
             return object.__getattribute__(self, key)
         except AttributeError as err:
+            if key == "_meta":
+                # Avoid a recursive loop if/when `self._meta`
+                # produces an `AttributeError`
+                raise RuntimeError(
+                    f"Failed to generate metadata for {self}. "
+                    "This operation may not be supported by the current backend."
+                )
+
             # Allow operands to be accessed as attributes
             # as long as the keys are not already reserved
             # by existing methods/properties
             _parameters = type(self)._parameters
             if key in _parameters:
                 idx = _parameters.index(key)
                 return self.operands[idx]
@@ -936,14 +956,21 @@
     Note that `Fused` expressions rely on every `Blockwise`
     expression defining a proper `_task` method.
     """
 
     operation = None
     _keyword_only = []
     _projection_passthrough = False
+    _filter_passthrough = False
+
+    @property
+    def _required_attribute(self):
+        if isinstance(self.operation, type(M.method_caller)):
+            return self.operation.method
+        return None
 
     @functools.cached_property
     def _meta(self):
         args = [op._meta if isinstance(op, Expr) else op for op in self._args]
         return self.operation(*args, **self._kwargs)
 
     @functools.cached_property
@@ -1022,29 +1049,49 @@
     def _simplify_up(self, parent):
         if self._projection_passthrough and isinstance(parent, Projection):
             return type(self)(self.frame[parent.operand("columns")], *self.operands[1:])
 
     def _combine_similar(self, root: Expr):
         # Push projections back up through `_projection_passthrough`
         # operations if it reduces the number of unique expression nodes.
-        if self._projection_passthrough and isinstance(self.frame, Projection):
-            common = type(self)(self.frame.frame, *self.operands[1:])
-            projection = self.frame.operand("columns")
-            push_up_projection = False
+        if (
+            self._projection_passthrough
+            and isinstance(self.frame, Projection)
+            or self._filter_passthrough
+            and isinstance(self.frame, Filter)
+        ):
+            frame, operations = self.frame, []
+            # We have to go back until we reach an operation that was not pushed down
+            while isinstance(frame, (Filter, Projection)):
+                operations.append(frame.operands[1])
+                frame = frame.frame
+            else:
+                try:
+                    common = type(self)(frame, *self.operands[1:])
+                except ValueError:
+                    # May have encountered a problem with `_required_attribute`.
+                    # (There is no guarentee that the same method will exist for
+                    # both a Series and DataFrame)
+                    return None
+            push_up_op = False
             for op in self._find_similar_operations(root, ignore=self._parameters):
                 if (
-                    isinstance(op.frame, Projection)
+                    isinstance(op.frame, (Projection, Filter))
                     and (
                         common._name == type(op)(op.frame.frame, *op.operands[1:])._name
                     )
                 ) or common._name == op._name:
-                    push_up_projection = True
+                    push_up_op = True
+                    break
 
-            if push_up_projection:
-                return common[projection]
+            if push_up_op:
+                # Add operations back in the same order
+                for op in reversed(operations):
+                    common = common[op]
+                return common
         return None
 
 
 class MapPartitions(Blockwise):
     _parameters = [
         "frame",
         "func",
@@ -1182,35 +1229,14 @@
                 return
             return type(parent)(
                 type(self)(self.frame[frame_columns], self.other[other_columns]),
                 *parent.operands[1:],
             )
 
 
-class RenameFrame(Blockwise):
-    _parameters = ["frame", "columns"]
-    _keyword_only = ["columns"]
-    operation = M.rename
-
-    def _simplify_up(self, parent):
-        if isinstance(parent, Projection) and isinstance(
-            self.operand("columns"), Mapping
-        ):
-            reverse_mapping = {val: key for key, val in self.operand("columns").items()}
-            if is_series_like(parent._meta):
-                # Fill this out when Series.rename is implemented
-                return
-            else:
-                columns = [
-                    reverse_mapping[col] if col in reverse_mapping else col
-                    for col in parent.columns
-                ]
-            return type(self)(self.frame[columns], *self.operands[1:])
-
-
 class Sample(Blockwise):
     _parameters = ["frame", "state_data", "frac", "replace"]
     operation = staticmethod(methods.sample)
 
     @functools.cached_property
     def _meta(self):
         args = [self.operands[0]._meta] + [self.operands[1][0]] + self.operands[2:]
@@ -1221,28 +1247,14 @@
             self.state_data[index],
             self.frac,
             self.replace,
         ]
         return (self.operation,) + tuple(args)
 
 
-class ToFrame(Blockwise):
-    _parameters = ["frame", "name"]
-    _defaults = {"name": no_default}
-    _keyword_only = ["name"]
-    operation = M.to_frame
-
-
-class ToFrameIndex(Blockwise):
-    _parameters = ["frame", "index", "name"]
-    _defaults = {"name": no_default, "index": True}
-    _keyword_only = ["name", "index"]
-    operation = M.to_frame
-
-
 class VarColumns(Blockwise):
     _parameters = ["frame", "skipna", "ddof", "numeric_only"]
     _defaults = {"skipna": True, "ddof": 1, "numeric_only": False}
     _keyword_only = ["skipna", "ddof", "numeric_only"]
     operation = M.var
 
     @functools.cached_property
@@ -1257,15 +1269,43 @@
 
 class Elemwise(Blockwise):
     """
     This doesn't really do anything, but we anticipate that future
     optimizations, like `len` will care about which operations preserve length
     """
 
-    pass
+    _filter_passthrough = True
+
+    def _simplify_up(self, parent):
+        if self._filter_passthrough and isinstance(parent, Filter):
+            return type(self)(
+                self.frame[parent.operand("predicate")], *self.operands[1:]
+            )
+        return super()._simplify_up(parent)
+
+
+class RenameFrame(Elemwise):
+    _parameters = ["frame", "columns"]
+    _keyword_only = ["columns"]
+    operation = M.rename
+
+    def _simplify_up(self, parent):
+        if isinstance(parent, Projection) and isinstance(
+            self.operand("columns"), Mapping
+        ):
+            reverse_mapping = {val: key for key, val in self.operand("columns").items()}
+            if is_series_like(parent._meta):
+                # Fill this out when Series.rename is implemented
+                return
+            else:
+                columns = [
+                    reverse_mapping[col] if col in reverse_mapping else col
+                    for col in parent.columns
+                ]
+            return type(self)(self.frame[columns], *self.operands[1:])
 
 
 class Fillna(Elemwise):
     _projection_passthrough = True
     _parameters = ["frame", "value"]
     _defaults = {"value": None}
     operation = M.fillna
@@ -1382,14 +1422,28 @@
         "columns": no_default,
         "axis": 0,
     }
     _keyword_only = ["mapper", "index", "columns", "axis"]
     operation = M.rename_axis
 
 
+class ToFrame(Elemwise):
+    _parameters = ["frame", "name"]
+    _defaults = {"name": no_default}
+    _keyword_only = ["name"]
+    operation = M.to_frame
+
+
+class ToFrameIndex(Elemwise):
+    _parameters = ["frame", "index", "name"]
+    _defaults = {"name": no_default, "index": True}
+    _keyword_only = ["name", "index"]
+    operation = M.to_frame
+
+
 class Apply(Elemwise):
     """A good example of writing a less-trivial blockwise operation"""
 
     _parameters = ["frame", "function", "args", "kwargs"]
     _defaults = {"args": (), "kwargs": {}}
     operation = M.apply
 
@@ -1516,14 +1570,15 @@
 
 
 class Projection(Elemwise):
     """Column Selection"""
 
     _parameters = ["frame", "columns"]
     operation = operator.getitem
+    _filter_passthrough = False
 
     @property
     def columns(self):
         if isinstance(self.operand("columns"), list):
             return self.operand("columns")
         elif isinstance(self.operand("columns"), pd.Index):
             return list(self.operand("columns"))
@@ -1580,14 +1635,15 @@
 
 
 class Index(Elemwise):
     """Column Selection"""
 
     _parameters = ["frame"]
     operation = getattr
+    _filter_passthrough = False
 
     @property
     def _meta(self):
         meta = self.frame._meta
         # Handle scalar results
         if is_series_like(meta) or is_dataframe_like(meta):
             return self.frame._meta.index
@@ -1636,14 +1692,42 @@
     _keyword_only = ["drop"]
     operation = M.reset_index
 
     def _divisions(self):
         return (None,) * (self.frame.npartitions + 1)
 
 
+class AddPrefix(Elemwise):
+    _parameters = ["frame", "prefix"]
+    operation = M.add_prefix
+
+    def _convert_columns(self, columns):
+        len_prefix = len(self.prefix)
+        return [col[len_prefix:] for col in columns]
+
+    def _simplify_up(self, parent):
+        if isinstance(parent, Projection):
+            columns = self._convert_columns(parent.columns)
+            if columns == self.frame.columns:
+                return
+            return type(parent)(
+                type(self)(self.frame[columns], self.operands[1]),
+                parent.operand("columns"),
+            )
+
+
+class AddSuffix(AddPrefix):
+    _parameters = ["frame", "suffix"]
+    operation = M.add_suffix
+
+    def _convert_columns(self, columns):
+        len_suffix = len(self.suffix)
+        return [col[:-len_suffix] for col in columns]
+
+
 class Head(Expr):
     """Take the first `n` rows of the first partition"""
 
     _parameters = ["frame", "n"]
     _defaults = {"n": 5}
 
     @property
@@ -1732,27 +1816,28 @@
 
     def _task(self, index: int):
         return (M.tail, (self.frame._name, index), self.n)
 
 
 class Binop(Elemwise):
     _parameters = ["left", "right"]
+    _filter_passthrough = False
 
     def __str__(self):
         return f"{self.left} {self._operator_repr} {self.right}"
 
     def _simplify_up(self, parent):
         if isinstance(parent, Projection):
-            if isinstance(self.left, Expr):
+            if isinstance(self.left, Expr) and self.left.ndim:
                 left = self.left[
                     parent.operand("columns")
                 ]  # TODO: filter just the correct columns
             else:
                 left = self.left
-            if isinstance(self.right, Expr):
+            if isinstance(self.right, Expr) and self.right.ndim:
                 right = self.right[parent.operand("columns")]
             else:
                 right = self.right
             return type(self)(left, right)
 
     def _node_label_args(self):
         return [self.left, self.right]
@@ -2109,15 +2194,17 @@
                         # in the local group (or the local stack
                         # of expr nodes that we know we will be
                         # adding to the local group).
                         # All nodes must also have the same number
                         # of partitions, since broadcasting within
                         # a group is not allowed.
                         stack.append(dep)
-                    elif dep not in roots and dependencies[dep]:
+                    elif dependencies[dep] and dep._name not in [
+                        r._name for r in roots
+                    ]:
                         # Couldn't fuse dep, but we may be able to
                         # use it as a new root on the next pass
                         roots.append(dep)
 
             # Replace fusable sub-group
             if len(group) > 1:
                 group_deps = []
```

### Comparing `dask-expr-0.1.1/dask_expr/_groupby.py` & `dask-expr-0.1.2/dask_expr/_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_merge.py` & `dask-expr-0.1.2/dask_expr/_merge.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_quantiles.py` & `dask-expr-0.1.2/dask_expr/_quantiles.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_reductions.py` & `dask-expr-0.1.2/dask_expr/_reductions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import functools
+
+import numpy as np
 import pandas as pd
 import toolz
 from dask.dataframe import hyperloglog, methods
 from dask.dataframe.core import (
     _concat,
     idxmaxmin_agg,
     idxmaxmin_chunk,
     idxmaxmin_combine,
     is_dataframe_like,
     is_series_like,
     make_meta,
     meta_nonempty,
 )
-from dask.utils import M, apply
+from dask.utils import M, apply, funcname
 
-from dask_expr._expr import Elemwise, Expr, Index, Projection
+from dask_expr._expr import Blockwise, Elemwise, Expr, Index, Projection
+from dask_expr._util import is_scalar
 
 
 class ApplyConcatApply(Expr):
     """Perform reduction-like operation on dataframes
 
     This pattern is commonly used for reductions, groupby-aggregations, and
     more.  It requires three methods to be implemented:
@@ -38,89 +42,189 @@
     chunk = None
     combine = None
     aggregate = None
     chunk_kwargs = {}
     combine_kwargs = {}
     aggregate_kwargs = {}
 
-    def __dask_postcompute__(self):
-        return toolz.first, ()
-
     def _layer(self):
+        # This is an abstract expression
+        raise NotImplementedError()
+
+    @property
+    def _meta(self):
+        meta = meta_nonempty(self.frame._meta)
+        meta = self.chunk(meta, **self.chunk_kwargs)
+        aggregate = self.aggregate or (lambda x: x)
+        if self.combine:
+            combine = self.combine
+            combine_kwargs = self.combine_kwargs
+        else:
+            combine = aggregate
+            combine_kwargs = self.aggregate_kwargs
+
+        meta = combine([meta], **combine_kwargs)
+        meta = aggregate([meta], **self.aggregate_kwargs)
+        return make_meta(meta)
+
+    def _divisions(self):
+        return (None, None)
+
+    def _lower(self):
         # Normalize functions in case not all are defined
         chunk = self.chunk
         chunk_kwargs = self.chunk_kwargs
-        split_every = getattr(self, "split_every", 0)
-
         if self.aggregate:
             aggregate = self.aggregate
             aggregate_kwargs = self.aggregate_kwargs
         else:
             aggregate = chunk
             aggregate_kwargs = chunk_kwargs
 
         if self.combine:
             combine = self.combine
             combine_kwargs = self.combine_kwargs
         else:
             combine = aggregate
             combine_kwargs = aggregate_kwargs
 
-        d = {}
-        keys = self.frame.__dask_keys__()
+        # Decompose ApplyConcatApply into Chunk and TreeReduce
+        aca_type = type(self)
+        return TreeReduce(
+            Chunk(self.frame, aca_type, chunk, chunk_kwargs),
+            aca_type,
+            self._meta,
+            combine,
+            aggregate,
+            combine_kwargs,
+            aggregate_kwargs,
+        )
 
-        # apply chunk to every input partition
-        for i, key in enumerate(keys):
-            if chunk_kwargs:
-                d[self._name, 0, i] = (apply, chunk, [key], chunk_kwargs)
-            else:
-                d[self._name, 0, i] = (chunk, key)
 
-        keys = list(d)
-        j = 1
+class Chunk(Blockwise):
+    """Partition-wise component of `ApplyConcatApply`
+
+    This class is used within `ApplyConcatApply._lower`.
+
+    See Also
+    --------
+    ApplyConcatApply
+    """
+
+    _parameters = ["frame", "kind", "chunk", "chunk_kwargs"]
+
+    def operation(self, *args, **kwargs):
+        return self.chunk(*args, **kwargs)
+
+    @functools.cached_property
+    def _args(self) -> list:
+        return [self.frame]
+
+    @functools.cached_property
+    def _kwargs(self) -> dict:
+        return self.chunk_kwargs or {}
+
+    def _tree_repr_lines(self, indent=0, recursive=True):
+        header = f"{funcname(self.kind)}({funcname(type(self))}):"
+        lines = []
+        if recursive:
+            for dep in self.dependencies():
+                lines.extend(dep._tree_repr_lines(2))
+
+        for k, v in self.chunk_kwargs.items():
+            try:
+                if v != self.kind._defaults[k]:
+                    header += f" {k}={v}"
+            except KeyError:
+                header += f" {k}={v}"
+
+        lines = [header] + lines
+        lines = [" " * indent + line for line in lines]
+        return lines
+
+
+class TreeReduce(Expr):
+    """Tree-reduction component of `ApplyConcatApply`
+
+    This class is used within `ApplyConcatApply._lower`.
+
+    See Also
+    --------
+    ApplyConcatApply
+    """
+
+    _parameters = [
+        "frame",
+        "kind",
+        "_meta",
+        "combine",
+        "aggregate",
+        "combine_kwargs",
+        "aggregate_kwargs",
+    ]
 
+    def __dask_postcompute__(self):
+        return toolz.first, ()
+
+    def _layer(self):
         # apply combine to batches of intermediate results
+        j = 1
+        d = {}
+        keys = self.frame.__dask_keys__()
+        split_every = getattr(self, "split_every", 0)
         while len(keys) > 1:
             new_keys = []
             for i, batch in enumerate(
                 toolz.partition_all(split_every or len(keys), keys)
             ):
                 batch = list(batch)
-                if combine_kwargs:
-                    d[self._name, j, i] = (apply, combine, [batch], combine_kwargs)
+                if self.combine_kwargs:
+                    d[self._name, j, i] = (
+                        apply,
+                        self.combine,
+                        [batch],
+                        self.combine_kwargs,
+                    )
                 else:
-                    d[self._name, j, i] = (combine, batch)
+                    d[self._name, j, i] = (self.combine, batch)
                 new_keys.append((self._name, j, i))
             j += 1
             keys = new_keys
 
         # apply aggregate to the final result
-        d[self._name, 0] = (apply, aggregate, [keys], aggregate_kwargs)
+        d[self._name, 0] = (apply, self.aggregate, [keys], self.aggregate_kwargs)
 
         return d
 
     @property
     def _meta(self):
-        meta = meta_nonempty(self.frame._meta)
-        meta = self.chunk(meta, **self.chunk_kwargs)
-        aggregate = self.aggregate or (lambda x: x)
-        if self.combine:
-            combine = self.combine
-            combine_kwargs = self.combine_kwargs
-        else:
-            combine = aggregate
-            combine_kwargs = self.aggregate_kwargs
-
-        meta = combine([meta], **combine_kwargs)
-        meta = aggregate([meta], **self.aggregate_kwargs)
-        return make_meta(meta)
+        return self.operand("_meta")
 
     def _divisions(self):
         return (None, None)
 
+    def __str__(self):
+        chunked = str(self.frame)
+        split_every = getattr(self, "split_every", 0)
+        return f"{type(self).__name__}({chunked}, kind={funcname(self.kind)}, split_every={split_every})"
+
+    def _tree_repr_lines(self, indent=0, recursive=True):
+        header = f"{funcname(self.kind)}({funcname(type(self))}):"
+        lines = []
+        if recursive:
+            for dep in self.dependencies():
+                lines.extend(dep._tree_repr_lines(2))
+
+        split_every = getattr(self, "split_every", 0)
+        header += f" split_every={split_every}"
+
+        lines = [header] + lines
+        lines = [" " * indent + line for line in lines]
+        return lines
+
 
 class Unique(ApplyConcatApply):
     _parameters = ["frame"]
     chunk = staticmethod(lambda x, **kwargs: methods.unique(x, **kwargs))
     aggregate_func = methods.unique
 
     @property
@@ -184,14 +288,120 @@
 
             return type(parent)(
                 type(self)(self.frame[sorted(columns)], *self.operands[1:]),
                 *parent.operands[1:],
             )
 
 
+class PivotTable(ApplyConcatApply):
+    _parameters = ["frame", "columns", "index", "values", "aggfunc"]
+    _defaults = {"columns": None, "index": None, "values": None, "aggfunc": "mean"}
+
+    @functools.cached_property
+    def _meta(self):
+        df = self.frame._meta
+        columns = self.operand("columns")
+        values = self.operand("values")
+        index = self.operand("index")
+        columns_contents = pd.CategoricalIndex(df[columns].cat.categories, name=columns)
+
+        if is_scalar(values):
+            new_columns = columns_contents
+        else:
+            new_columns = pd.MultiIndex.from_product(
+                (sorted(values), columns_contents), names=[None, columns]
+            )
+
+        if self.operand("aggfunc") in ["first", "last"]:
+            # Infer datatype as non-numeric values are allowed
+            if is_scalar(values):
+                meta = pd.DataFrame(
+                    columns=new_columns,
+                    dtype=df[values].dtype,
+                    index=pd.Index(df[index]),
+                )
+            else:
+                meta = pd.DataFrame(
+                    columns=new_columns,
+                    index=pd.Index(df[index]),
+                )
+                for value_col in values:
+                    meta[value_col] = meta[value_col].astype(
+                        df[values].dtypes[value_col]
+                    )
+        else:
+            # Use float64 as other aggregate functions require numerical data
+            meta = pd.DataFrame(
+                columns=new_columns, dtype=np.float64, index=pd.Index(df[index])
+            )
+        return meta
+
+    def _lower(self):
+        args = [
+            self.frame,
+            self.operand("columns"),
+            self.operand("index"),
+            self.operand("values"),
+        ]
+        if self.aggfunc == "sum":
+            return PivotTableSum(*args)
+        elif self.aggfunc == "mean":
+            return PivotTableSum(*args) / PivotTableCount(*args)
+        elif self.aggfunc == "count":
+            return PivotTableCount(*args)
+        elif self.aggfunc == "first":
+            return PivotTableFirst(*args)
+        elif self.aggfunc == "last":
+            return PivotTableLast(*args)
+        else:
+            raise NotImplementedError(f"{self.aggfunc=} is not implemented")
+
+
+class PivotTableAbstract(ApplyConcatApply):
+    _parameters = ["frame", "columns", "index", "values", "aggfunc"]
+    _defaults = {"columns": None, "index": None, "values": None, "aggfunc": "mean"}
+
+    @property
+    def chunk_kwargs(self):
+        return {
+            "index": self.operand("index"),
+            "columns": self.operand("columns"),
+            "values": self.operand("values"),
+        }
+
+    @classmethod
+    def combine(cls, inputs: list, **kwargs):
+        return _concat(inputs)
+
+    @classmethod
+    def aggregate(cls, inputs: list, **kwargs):
+        df = _concat(inputs)
+        return cls.aggregate_func(df, **kwargs)
+
+
+class PivotTableSum(PivotTableAbstract):
+    chunk = staticmethod(methods.pivot_sum)
+    aggregate_func = staticmethod(methods.pivot_agg)
+
+
+class PivotTableCount(PivotTableAbstract):
+    chunk = staticmethod(methods.pivot_count)
+    aggregate_func = staticmethod(methods.pivot_agg)
+
+
+class PivotTableFirst(PivotTableAbstract):
+    chunk = staticmethod(methods.pivot_first)
+    aggregate_func = staticmethod(methods.pivot_agg_first)
+
+
+class PivotTableLast(PivotTableAbstract):
+    chunk = staticmethod(methods.pivot_last)
+    aggregate_func = staticmethod(methods.pivot_agg_last)
+
+
 class Reduction(ApplyConcatApply):
     """A common pattern of apply concat apply
 
     Common reductions like sum/min/max/count/... have some shared code around
     `_concat` and so on.  This class inherits from `ApplyConcatApply` in order
     to leverage this shared structure.
 
@@ -382,14 +592,15 @@
         return
 
 
 class NBytes(Reduction):
     # Only supported for Series objects
     reduction_chunk = lambda ser: ser.nbytes
     reduction_aggregate = sum
+    _required_attribute = "nbytes"
 
 
 class Var(Reduction):
     # Uses the parallel version of Welford's online algorithm (Chan 79')
     # (http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf)
     _parameters = ["frame", "skipna", "ddof", "numeric_only"]
     _defaults = {"skipna": True, "ddof": 1, "numeric_only": False}
@@ -413,24 +624,29 @@
     @property
     def aggregate_kwargs(self):
         return dict(ddof=self.ddof)
 
     @classmethod
     def reduction_chunk(cls, x, skipna=True, numeric_only=False):
         kwargs = {"numeric_only": numeric_only} if is_dataframe_like(x) else {}
-        if skipna:
+        if skipna or numeric_only:
             n = x.count(**kwargs)
             kwargs["skipna"] = skipna
             avg = x.mean(**kwargs)
         else:
             # Not skipping nulls, so might as well
             # avoid the full `count` operation
             n = len(x)
             kwargs["skipna"] = skipna
             avg = x.sum(**kwargs) / n
+        if numeric_only:
+            # Workaround for cudf bug
+            # (see: https://github.com/rapidsai/cudf/issues/13731)
+            x = x.select_dtypes("number")
+            n = n.loc[x.columns]
         m2 = ((x - avg) ** 2).sum(**kwargs)
         return n, avg, m2
 
     @classmethod
     def reduction_combine(cls, parts):
         n, avg, m2 = parts[0]
         for i in range(1, len(parts)):
```

### Comparing `dask-expr-0.1.1/dask_expr/_repartition.py` & `dask-expr-0.1.2/dask_expr/_repartition.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/_shuffle.py` & `dask-expr-0.1.2/dask_expr/_shuffle.py`

 * *Files 10% similar despite different names*

```diff
@@ -614,15 +614,35 @@
             index = [index] if isinstance(index, str) else list(index)
             index = partitioning_index(df[index], npartitions)
         else:
             index = partitioning_index(index, npartitions)
         return df.assign(**{name: index})
 
 
-class SetIndex(Expr):
+class BaseSetIndexSortValues(Expr):
+    def _divisions(self):
+        if self.user_divisions is not None:
+            return self.user_divisions
+        divisions, mins, maxes, presorted = _calculate_divisions(
+            self.frame,
+            self.other,
+            self.npartitions,
+            self.ascending,
+            upsample=self.upsample,
+        )
+        if presorted:
+            divisions = mins.copy() + [maxes[-1]]
+        return divisions
+
+    @property
+    def npartitions(self):
+        return self.operand("npartitions") or self.frame.npartitions
+
+
+class SetIndex(BaseSetIndexSortValues):
     """Abstract ``set_index`` class.
 
     Simplifies (later lowers) either to Blockwise ops if we are already sorted
     or to ``SetPartition`` which handles shuffling.
 
     Parameters
     ----------
@@ -632,38 +652,46 @@
         Either a Series-like expression to use as Index or a scalar defining the column.
     drop: bool
         Whether we drop the old column.
     sorted: str
         No need for shuffling if we are already sorted.
     user_divisions: int
         Divisions as passed by the user.
+    upsample: float
+        Used to increase the number of samples for quantiles.
     """
 
     _parameters = [
         "frame",
         "_other",
         "drop",
         "user_divisions",
         "partition_size",
         "ascending",
         "npartitions",
+        "upsample",
     ]
     _defaults = {
         "drop": True,
         "user_divisions": None,
         "partition_size": 128e6,
         "ascending": True,
         "npartitions": None,
+        "upsample": 1.0,
     }
 
     def _divisions(self):
         if self.user_divisions is not None:
             return self.user_divisions
         divisions, mins, maxes, presorted = _calculate_divisions(
-            self.frame, self.other, self.npartitions, self.ascending
+            self.frame,
+            self.other,
+            self.npartitions,
+            self.ascending,
+            upsample=self.upsample,
         )
         if presorted:
             divisions = mins.copy() + [maxes[-1]]
         return divisions
 
     @property
     def npartitions(self):
@@ -685,15 +713,19 @@
             return self._other
         return self.frame[self._other]
 
     def _lower(self):
         if self.user_divisions is None:
             divisions = self._divisions()
             presorted = _calculate_divisions(
-                self.frame, self.other, self.npartitions, self.ascending
+                self.frame,
+                self.other,
+                self.npartitions,
+                self.ascending,
+                upsample=self.upsample,
             )[3]
 
             if presorted and self.npartitions == self.frame.npartitions:
                 index_set = SetIndexBlockwise(
                     self.frame, self._other, self.drop, divisions
                 )
                 return SortIndexBlockwise(index_set)
@@ -712,14 +744,93 @@
                 return
             return type(parent)(
                 type(self)(self.frame[columns], *self.operands[1:]),
                 parent.operand("columns"),
             )
 
 
+class SortValues(BaseSetIndexSortValues):
+    _parameters = [
+        "frame",
+        "by",
+        "ascending",
+        "na_position",
+        "npartitions",
+        "partition_size",
+        "sort_function",
+        "sort_function_kwargs",
+        "upsample",
+    ]
+    _defaults = {
+        "partition_size": 128e6,
+        "ascending": True,
+        "npartitions": None,
+        "na_position": "last",
+        "sort_function": None,
+        "sort_function_kwargs": None,
+        "upsample": 1.0,
+    }
+
+    @property
+    def sort_function(self):
+        if self.operand("sort_function") is not None:
+            return self.operand("sort_function")
+        return M.sort_values
+
+    @property
+    def sort_function_kwargs(self):
+        sort_kwargs = {
+            "by": self.by,
+            "ascending": self.ascending,
+            "na_position": self.na_position,
+        }
+        if self.operand("sort_function_kwargs") is not None:
+            sort_kwargs.update(self.operand("sort_function_kwargs"))
+        return sort_kwargs
+
+    @property
+    def _meta(self):
+        return self.frame._meta
+
+    def _lower(self):
+        by = self.frame[self.by[0]]
+        divisions, _, _, presorted = _calculate_divisions(
+            self.frame, by, self.npartitions, self.ascending, upsample=self.upsample
+        )
+        if presorted and self.npartitions == self.frame.npartitions:
+            return SortValuesBlockwise(
+                self.frame, self.sort_function, self.sort_function_kwargs
+            )
+
+        partitions = _SetPartitionsPreSetIndex(by, by._meta._constructor(divisions))
+        assigned = Assign(self.frame, "_partitions", partitions)
+        shuffled = Shuffle(
+            assigned,
+            "_partitions",
+            npartitions_out=len(divisions) - 1,
+            ignore_index=True,
+        )
+        return SortValuesBlockwise(
+            shuffled, self.sort_function, self.sort_function_kwargs
+        )
+
+    def _simplify_up(self, parent):
+        if isinstance(parent, Projection):
+            parent_columns = parent.columns
+            columns = parent_columns + [
+                col for col in self.by if col not in parent_columns
+            ]
+            if self.frame.columns == columns:
+                return
+            return type(parent)(
+                type(self)(self.frame[columns], *self.operands[1:]),
+                parent.operand("columns"),
+            )
+
+
 class SetPartition(SetIndex):
     """Shuffles the DataFrame according to its new divisions.
 
     Simplifies the Expression to blockwise pre-processing, shuffle and
     blockwise post-processing expressions.
 
     Parameters
@@ -785,14 +896,27 @@
 
 class SortIndexBlockwise(Blockwise):
     _projection_passthrough = True
     _parameters = ["frame"]
     operation = M.sort_index
 
 
+def sort_function(self, *args, **kwargs):
+    sort_func = kwargs.pop("sort_function")
+    sort_kwargs = kwargs.pop("sort_kwargs")
+    return sort_func(*args, **kwargs, **sort_kwargs)
+
+
+class SortValuesBlockwise(Blockwise):
+    _projection_passthrough = False
+    _parameters = ["frame", "sort_function", "sort_kwargs"]
+    operation = sort_function
+    _keyword_only = ["sort_function", "sort_kwargs"]
+
+
 class SetIndexBlockwise(Blockwise):
     _parameters = ["frame", "other", "drop", "new_divisions"]
     _keyword_only = ["drop", "new_divisions"]
 
     def operation(self, df, *args, new_divisions, **kwargs):
         return df.set_index(*args, **kwargs)
 
@@ -817,19 +941,20 @@
 @functools.lru_cache  # noqa: B019
 def _calculate_divisions(
     frame,
     other,
     npartitions: int,
     ascending: bool = True,
     partition_size: float = 128e6,
+    upsample: float = 1.0,
 ):
     from dask_expr import RepartitionQuantiles, new_collection
 
     divisions, mins, maxes = compute(
-        new_collection(RepartitionQuantiles(other, npartitions)),
+        new_collection(RepartitionQuantiles(other, npartitions, upsample=upsample)),
         new_collection(other).map_partitions(M.min),
         new_collection(other).map_partitions(M.max),
     )
     sizes = []
 
     empty_dataframe_detected = pd.isna(divisions).all()
     if empty_dataframe_detected:
```

### Comparing `dask-expr-0.1.1/dask_expr/datasets.py` & `dask-expr-0.1.2/dask_expr/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/io/csv.py` & `dask-expr-0.1.2/dask_expr/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/io/io.py` & `dask-expr-0.1.2/dask_expr/io/io.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.1/dask_expr/io/parquet.py` & `dask-expr-0.1.2/dask_expr/io/parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     get_engine,
     set_index_columns,
     sorted_columns,
 )
 from dask.dataframe.io.parquet.utils import _split_user_options
 from dask.dataframe.io.utils import _is_local_fs
 from dask.delayed import delayed
-from dask.utils import apply, natural_sort_key
+from dask.utils import apply, natural_sort_key, typename
 from fsspec.utils import stringify_path
 
 from dask_expr._expr import (
     EQ,
     GE,
     GT,
     LE,
@@ -153,15 +153,14 @@
         else:
             return {(self._name, 0): (lambda x: None, self.frame.__dask_keys__())}
 
 
 def to_parquet(
     df,
     path,
-    engine="pyarrow",
     compression="snappy",
     write_index=True,
     append=False,
     overwrite=False,
     ignore_divisions=False,
     partition_on=None,
     storage_options=None,
@@ -173,14 +172,15 @@
     name_function=None,
     filesystem=None,
     **kwargs,
 ):
     from dask_expr._collection import new_collection
     from dask_expr.io.parquet import NONE_LABEL, ToParquet
 
+    engine = _set_parquet_engine(meta=df._meta)
     compute_kwargs = compute_kwargs or {}
 
     partition_on = partition_on or []
     if isinstance(partition_on, str):
         partition_on = [partition_on]
 
     if set(partition_on) - set(df.columns):
@@ -387,14 +387,15 @@
         "ignore_metadata_file",
         "metadata_task_size",
         "split_row_groups",
         "blocksize",
         "aggregate_files",
         "parquet_file_extension",
         "filesystem",
+        "engine",
         "kwargs",
         "_partitions",
         "_series",
     ]
     _defaults = {
         "columns": None,
         "filters": None,
@@ -405,23 +406,27 @@
         "ignore_metadata_file": False,
         "metadata_task_size": None,
         "split_row_groups": "infer",
         "blocksize": "default",
         "aggregate_files": None,
         "parquet_file_extension": (".parq", ".parquet", ".pq"),
         "filesystem": "fsspec",
+        "engine": "pyarrow",
         "kwargs": None,
         "_partitions": None,
         "_series": False,
     }
     _pq_length_stats = None
 
     @property
     def engine(self):
-        return get_engine("pyarrow")
+        _engine = self.operand("engine")
+        if isinstance(_engine, str):
+            return get_engine(_engine)
+        return _engine
 
     @property
     def columns(self):
         columns_operand = self.operand("columns")
         if columns_operand is None:
             return list(self._meta.columns)
         else:
@@ -677,14 +682,28 @@
 
 
 #
 # Helper functions
 #
 
 
+def _set_parquet_engine(engine=None, meta=None):
+    # Use `engine` or `meta` input to set the parquet engine
+    if engine is None:
+        if (
+            meta is not None and typename(meta).split(".")[0] == "cudf"
+        ) or dask.config.get("dataframe.backend", "pandas") == "cudf":
+            from dask_cudf.io.parquet import CudfEngine
+
+            engine = CudfEngine
+        else:
+            engine = "pyarrow"
+    return engine
+
+
 def _align_statistics(parts, statistics):
     # Make sure parts and statistics are aligned
     # (if statistics is not empty)
     if statistics and len(parts) != len(statistics):
         statistics = []
     if statistics:
         result = list(
```

### Comparing `dask-expr-0.1.1/dask_expr.egg-info/PKG-INFO` & `dask-expr-0.1.2/dask_expr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 0.1.1
+Version: 0.1.2
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -81,14 +81,16 @@
 
 API Coverage
 ------------
 
 **`dask_expr.DataFrame`**
 
 - `abs`
+- `add_prefix`
+- `add_sufix`
 - `align`
 - `all`
 - `any`
 - `apply`
 - `assign`
 - `astype`
 - `clip`
@@ -118,22 +120,24 @@
 - `min`
 - `min`
 - `mode`
 - `nlargest`
 - `nsmallest`
 - `nunique_approx`
 - `partitions`
+- `pivot_table`
 - `prod`
 - `rename`
 - `rename_axis`
 - `repartition`
 - `replace`
 - `reset_index`
 - `round`
 - `sample`
+- `sort_values`
 - `select_dtypes`
 - `set_index`
 - `shuffle`
 - `std`
 - `sum`
 - `tail`
 - `to_parquet`
@@ -288,7 +292,11 @@
 
 
 **Unary operators (`DataFrame`, `Series`, and `Index`)**:
 
 - `__invert__`
 - `__neg__`
 - `__pos__`
+
+**Accessors**:
+
+- `CategoricalAccessor`
```

### Comparing `dask-expr-0.1.1/dask_expr.egg-info/SOURCES.txt` & `dask-expr-0.1.2/dask_expr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-versioneer.py
 dask_expr/__init__.py
 dask_expr/_accessor.py
 dask_expr/_align.py
 dask_expr/_categorical.py
 dask_expr/_collection.py
 dask_expr/_concat.py
 dask_expr/_expr.py
 dask_expr/_groupby.py
 dask_expr/_merge.py
 dask_expr/_quantiles.py
 dask_expr/_reductions.py
 dask_expr/_repartition.py
 dask_expr/_shuffle.py
-dask_expr/_typing.py
 dask_expr/_util.py
 dask_expr/_version.py
 dask_expr/datasets.py
 dask_expr.egg-info/PKG-INFO
 dask_expr.egg-info/SOURCES.txt
 dask_expr.egg-info/dependency_links.txt
 dask_expr.egg-info/requires.txt
```

### Comparing `dask-expr-0.1.1/pyproject.toml` & `dask-expr-0.1.2/pyproject.toml`

 * *Files identical despite different names*

