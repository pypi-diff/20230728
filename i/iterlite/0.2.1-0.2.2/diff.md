# Comparing `tmp/iterlite-0.2.1.tar.gz` & `tmp/iterlite-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterlite-0.2.1.tar", last modified: Sun Jul 23 20:45:36 2023, max compression
+gzip compressed data, was "iterlite-0.2.2.tar", last modified: Fri Jul 28 13:05:23 2023, max compression
```

## Comparing `iterlite-0.2.1.tar` & `iterlite-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 20:45:36.529576 iterlite-0.2.1/
--rw-rw-rw-   0        0        0     1968 2023-07-23 20:45:36.528564 iterlite-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-06-27 16:54:51.000000 iterlite-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 20:45:36.522546 iterlite-0.2.1/iterlite/
--rw-rw-rw-   0        0        0       80 2023-07-23 20:44:33.000000 iterlite-0.2.1/iterlite/__init__.py
--rw-rw-rw-   0        0        0     7261 2023-07-23 20:45:10.000000 iterlite-0.2.1/iterlite/enumerable.py
-drwxrwxrwx   0        0        0        0 2023-07-23 20:45:36.527435 iterlite-0.2.1/iterlite.egg-info/
--rw-rw-rw-   0        0        0     1968 2023-07-23 20:45:36.000000 iterlite-0.2.1/iterlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-23 20:45:36.000000 iterlite-0.2.1/iterlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 20:45:36.000000 iterlite-0.2.1/iterlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-23 20:45:36.000000 iterlite-0.2.1/iterlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 20:45:36.529576 iterlite-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-07-05 12:40:32.000000 iterlite-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:05:23.033982 iterlite-0.2.2/
+-rw-rw-rw-   0        0        0     1968 2023-07-28 13:05:23.032973 iterlite-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-06-27 16:54:51.000000 iterlite-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 13:05:23.018502 iterlite-0.2.2/iterlite/
+-rw-rw-rw-   0        0        0       80 2023-07-28 13:04:38.000000 iterlite-0.2.2/iterlite/__init__.py
+-rw-rw-rw-   0        0        0     8124 2023-07-28 12:50:46.000000 iterlite-0.2.2/iterlite/enumerable.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:05:23.031527 iterlite-0.2.2/iterlite.egg-info/
+-rw-rw-rw-   0        0        0     1968 2023-07-28 13:05:22.000000 iterlite-0.2.2/iterlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-28 13:05:22.000000 iterlite-0.2.2/iterlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:05:22.000000 iterlite-0.2.2/iterlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 13:05:22.000000 iterlite-0.2.2/iterlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:05:23.033982 iterlite-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-07-05 12:40:32.000000 iterlite-0.2.2/setup.py
```

### Comparing `iterlite-0.2.1/PKG-INFO` & `iterlite-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterlite
-Version: 0.2.1
+Version: 0.2.2
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `iterlite-0.2.1/README.md` & `iterlite-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `iterlite-0.2.1/iterlite/enumerable.py` & `iterlite-0.2.2/iterlite/enumerable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+import multiprocessing as mp
 from typing import *
 from collections import deque
 import itertools
 import functools
 from typing import Callable, Iterable
 
 T = TypeVar('T')
@@ -103,14 +104,26 @@
         return call(self)
     
     def thread_map(self, func: Callable[[T], R], threadpool_factory: Optional[Callable[[], ThreadPoolExecutor]] = None) -> Iter[R]:
         """
         WIP: map with automatic threading
         """
         return AsyncIter(self, func, threadpool_factory)
+    
+    def parallel(self, pool_factory: Optional[Callable[[], mp.Pool]] = None) -> ParIter[T]:
+        return ParIter(self, pool_factory)
+    
+    def par_map(self, func:Callable[[T], R], pool_factory: Optional[Callable[[], mp.Pool]] = None) -> ParIter[R]:
+        """
+        WIP: map with automatic threading
+        """
+        return self.parallel(pool_factory).map(func)
+    
+
+
 
 class IterCollection(Iter[T], Generic[T]):
     _collection = None
 
     def __init__(self, data: Collection[T]) -> None:
         if not isinstance(data, Collection):
             raise TypeError("iterator must be Collection!")
@@ -205,16 +218,26 @@
         return Iter(iter(super().keys()))
     def values(self) -> Iter[V]:
         return Iter(iter(super().values()))
     def items(self) -> Iter[tuple[K, V]]:
         return Iter(iter(super().items()))
 
 class AsyncIter(Iter[T]):
-    def __init__(self, iterator: Iterable[T], func:Callable[[T], R], threadpool_factory: Optional[Callable[[], ThreadPoolExecutor]] = None) -> None:
+    def __init__(self, iterator: Iterable[T], func:Callable[[T], R], factory: Optional[Callable[[], ThreadPoolExecutor]] = None) -> None:
         super().__init__(iterator)
         self.func = func
-        self.factory = lambda: ThreadPoolExecutor()
+        self.factory = factory if factory is not None else lambda: ThreadPoolExecutor()
     
     def __iter__(self) -> AsyncIter[R]:
         with self.factory() as _pool:
             _r = Iter(_pool.map(self.func, self._iter))
-        return Iter(_r)
+        return _r
+
+class ParIter(Iter[T]):
+    def __init__(self, iterator: Iterable[T], factory: Optional[Callable[[], mp.Pool]] = None) -> None:
+        super().__init__(iterator)
+        self.factory = factory if factory is not None else lambda: mp.Pool()
+    
+    def map(self, func: Callable[[T], R]) -> ParIter[R]:
+        with mp.Pool(4) as _pool:
+            _r = SList(_pool.map(func, self._iter))
+        return _r
```

### Comparing `iterlite-0.2.1/iterlite.egg-info/PKG-INFO` & `iterlite-0.2.2/iterlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterlite
-Version: 0.2.1
+Version: 0.2.2
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `iterlite-0.2.1/setup.py` & `iterlite-0.2.2/setup.py`

 * *Files identical despite different names*

