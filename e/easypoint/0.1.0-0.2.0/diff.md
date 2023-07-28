# Comparing `tmp/easypoint-0.1.0.tar.gz` & `tmp/easypoint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypoint-0.1.0.tar", max compression
+gzip compressed data, was "easypoint-0.2.0.tar", max compression
```

## Comparing `easypoint-0.1.0.tar` & `easypoint-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-15 21:10:09.768372 easypoint-0.1.0/LICENSE
--rw-r--r--   0        0        0     9484 2023-07-28 06:13:00.910012 easypoint-0.1.0/README.md
--rw-r--r--   0        0        0      126 2023-07-28 04:01:28.742017 easypoint-0.1.0/easypoint/__init__.py
--rw-r--r--   0        0        0      395 2023-07-28 04:28:56.696307 easypoint-0.1.0/easypoint/internal_types.py
--rw-r--r--   0        0        0     7390 2023-07-28 04:56:49.443795 easypoint-0.1.0/easypoint/matrix.py
--rw-r--r--   0        0        0    10670 2023-07-28 04:53:40.221500 easypoint-0.1.0/easypoint/point.py
--rw-r--r--   0        0        0        0 2023-07-25 06:11:56.405760 easypoint-0.1.0/easypoint/py.typed
--rw-r--r--   0        0        0     2353 2023-07-28 04:29:41.102730 easypoint-0.1.0/easypoint/utils.py
--rw-r--r--   0        0        0      427 2023-07-28 05:08:52.316495 easypoint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10145 1970-01-01 00:00:00.000000 easypoint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-28 09:07:35.071899 easypoint-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9613 2023-07-28 09:07:35.071899 easypoint-0.2.0/README.md
+-rw-r--r--   0        0        0      126 2023-07-28 09:07:35.071899 easypoint-0.2.0/easypoint/__init__.py
+-rw-r--r--   0        0        0      456 2023-07-28 09:07:35.071899 easypoint-0.2.0/easypoint/internal_types.py
+-rw-r--r--   0        0        0     7500 2023-07-28 09:07:35.071899 easypoint-0.2.0/easypoint/matrix.py
+-rw-r--r--   0        0        0    10653 2023-07-28 09:07:35.071899 easypoint-0.2.0/easypoint/point.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:07:35.071899 easypoint-0.2.0/easypoint/py.typed
+-rw-r--r--   0        0        0     2355 2023-07-28 09:07:35.071899 easypoint-0.2.0/easypoint/utils.py
+-rw-r--r--   0        0        0      443 2023-07-28 09:07:35.071899 easypoint-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10274 1970-01-01 00:00:00.000000 easypoint-0.2.0/PKG-INFO
```

### Comparing `easypoint-0.1.0/LICENSE` & `easypoint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easypoint-0.1.0/README.md` & `easypoint-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Minimal general-purpose vector / matrix arithmetics library
 
+# Installation
+
+Install `easypoint` module:
+
+```bash
+poetry add easypoint
+```
+
+or
+
+```bash
+python -m pip install easypoint
+```
+
+
 # Introduction
 
 easypoint has 2 main types to work with: `Point` (a.k.a. `Vector`) and `Matrix`
 
 `Point` class builds up on my previous work with [evtn/soda](https://github.com/evtn/soda) and [evtn/soda-old](https://github.com/evtn/soda-old).    
 Both being graphics-oriented, so vector arithmetics is a must-have.
```

### Comparing `easypoint-0.1.0/easypoint/matrix.py` & `easypoint-0.2.0/easypoint/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,19 @@
         new_size = (*self.size[:-1], *other.size[1:])
         new = Matrix(new_size)
         split = len(self.size) - 1
 
         for index in new:
             result: float = 0
             for x in range(self.size[split]):
-                s = self[*index[:split], x]
-                o = other[x, *index[split:]]
+                s_index = (*index[:split], x)
+                o_index = (x, *index[split:])
+
+                s = self[s_index]
+                o = other[o_index]
                 result += s * o
 
             new[index] = result
         return new
 
     def __add__(self, other: Matrix) -> Matrix:
         return self.apply_bin(
@@ -204,15 +207,17 @@
 
         for control, *rest in self.iter((i, *zeros)):
             new_index = tuple(rest)  # `rest` is a list
 
             if control != i:
                 return submatrix
 
-            submatrix[new_index] = self[control, *new_index]
+            cut_index = (control, *new_index)
+
+            submatrix[new_index] = self[cut_index]
 
         if control is not None:
             return submatrix
 
         raise ValueError("can't get a submatrix for an empty matrix")
 
     def to_list(self) -> MatrixList:
```

### Comparing `easypoint-0.1.0/easypoint/point.py` & `easypoint-0.2.0/easypoint/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import (
     Any,
     Callable,
     Iterator,
     Sequence,
     cast,
     overload,
-    reveal_type,
 )
 from typing_extensions import Self
 
 
 def applier(func: Merger) -> ApplyFunc:
     return lambda s, o: Point.from_(s).apply(Point.from_(o), func)
```

### Comparing `easypoint-0.1.0/easypoint/utils.py` & `easypoint-0.2.0/easypoint/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,13 +80,13 @@
             if index not in range(-length, length):
                 return 0
             if index < 0:
                 index %= length
 
         return get(start + index * step)
 
-    result: tuple[IndexFunc, int | None] = new_get, length
+    result: tuple[IndexFunc, int | None] = (new_get, length)
 
     return result
 
 
 from .internal_types import IndexFunc
```

### Comparing `easypoint-0.1.0/PKG-INFO` & `easypoint-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypoint
-Version: 0.1.0
+Version: 0.2.0
 Summary: Minimal general-purpose vector / matrix arithmetics library
 License: MIT
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Minimal general-purpose vector / matrix arithmetics library
 
+# Installation
+
+Install `easypoint` module:
+
+```bash
+poetry add easypoint
+```
+
+or
+
+```bash
+python -m pip install easypoint
+```
+
+
 # Introduction
 
 easypoint has 2 main types to work with: `Point` (a.k.a. `Vector`) and `Matrix`
 
 `Point` class builds up on my previous work with [evtn/soda](https://github.com/evtn/soda) and [evtn/soda-old](https://github.com/evtn/soda-old).    
 Both being graphics-oriented, so vector arithmetics is a must-have.
```

