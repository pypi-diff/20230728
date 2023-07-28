# Comparing `tmp/slist-0.1.6.tar.gz` & `tmp/slist-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slist-0.1.6.tar", max compression
+gzip compressed data, was "slist-0.1.7.tar", max compression
```

## Comparing `slist-0.1.6.tar` & `slist-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-01-31 17:25:36.800173 slist-0.1.6/LICENSE
--rw-r--r--   0        0        0     2689 2023-01-31 17:25:36.800173 slist-0.1.6/README.md
--rw-r--r--   0        0        0     1823 2023-01-31 17:25:36.800173 slist-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    22791 2023-01-31 17:25:36.800173 slist-0.1.6/slist/__init__.py
--rw-r--r--   0        0        0        0 2023-01-31 17:25:36.800173 slist-0.1.6/slist/py.typed
--rw-r--r--   0        0        0     1415 2023-01-31 17:25:36.800173 slist-0.1.6/slist/pydantic_compat.py
--rw-r--r--   0        0        0        0 2023-01-31 17:25:36.800173 slist-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0      429 2023-01-31 17:25:36.800173 slist-0.1.6/tests/test_docs.py
--rw-r--r--   0        0        0      519 2023-01-31 17:25:36.800173 slist-0.1.6/tests/test_mypy.py
--rw-r--r--   0        0        0     4647 2023-01-31 17:25:36.800173 slist-0.1.6/tests/test_slist.py
--rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 slist-0.1.6/setup.py
--rw-r--r--   0        0        0     3721 1970-01-01 00:00:00.000000 slist-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-28 06:29:36.928313 slist-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2689 2023-07-28 06:29:36.928313 slist-0.1.7/README.md
+-rw-r--r--   0        0        0     1823 2023-07-28 06:29:36.928313 slist-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    23183 2023-07-28 06:29:36.928313 slist-0.1.7/slist/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:29:36.928313 slist-0.1.7/slist/py.typed
+-rw-r--r--   0        0        0     1415 2023-07-28 06:29:36.928313 slist-0.1.7/slist/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:29:36.928313 slist-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0      429 2023-07-28 06:29:36.928313 slist-0.1.7/tests/test_docs.py
+-rw-r--r--   0        0        0      519 2023-07-28 06:29:36.928313 slist-0.1.7/tests/test_mypy.py
+-rw-r--r--   0        0        0     4826 2023-07-28 06:29:36.928313 slist-0.1.7/tests/test_slist.py
+-rw-r--r--   0        0        0     3571 1970-01-01 00:00:00.000000 slist-0.1.7/PKG-INFO
```

### Comparing `slist-0.1.6/LICENSE` & `slist-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slist-0.1.6/README.md` & `slist-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `slist-0.1.6/pyproject.toml` & `slist-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "slist"
-version = "0.1.6"
+version = "0.1.7"
 homepage = "https://github.com/thejaminator/slist"
 description = "A typesafe list with more method chaining!"
 authors = ["James Chua <chuajamessh@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `slist-0.1.6/slist/__init__.py` & `slist-0.1.7/slist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,27 @@
     @property
     def first_option(self) -> Optional[A]:
         try:
             return self.__getitem__(0)
         except IndexError:
             return None
 
+    @property
+    def mode_option(self) -> Optional[A]:
+        try:
+            return statistics.mode(self)
+        except statistics.StatisticsError:
+            return None
+
+    def mode_or_raise(self, exception: Exception = RuntimeError("List is empty")) -> A:
+        try:
+            return statistics.mode(self)
+        except statistics.StatisticsError:
+            raise exception
+
     def first_or_raise(self, exception: Exception = RuntimeError("List is empty")) -> A:
         try:
             return self.__getitem__(0)
         except IndexError:
             raise exception
 
     def last_or_raise(self, exception: Exception = RuntimeError("List is empty")) -> A:
```

### Comparing `slist-0.1.6/slist/pydantic_compat.py` & `slist-0.1.7/slist/pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `slist-0.1.6/tests/test_mypy.py` & `slist-0.1.7/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `slist-0.1.6/tests/test_slist.py` & `slist-0.1.7/tests/test_slist.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,29 +97,39 @@
     assert test_list.window(size=2) == Slist()
 
 
 def test_window_too_small_list():
     test_list = Slist([1])
     assert test_list.window(size=2) == Slist()
 
+
 def test_median():
     numbers = Slist([2, 3, 4, 5, 6, 7, 8, 9, 1])
     assert numbers.median_by(identity) == 5
 
+
 def test_percentile():
     numbers = Slist([2, 3, 4, 5, 6, 7, 8, 9, 1])
     assert numbers.percentile_by(identity, 0.5) == 5
     assert numbers.percentile_by(identity, 0.25) == 3
     assert numbers.percentile_by(identity, 0.75) == 7
 
 
 def test_max_by():
     numbers = Slist([2, 3, 4, 5, 6, 7, 8, 9, 1])
     assert numbers.max_by(identity) == 9
     empty = Slist([])
     assert empty.max_by(identity) is None
 
+
 def test_min_by():
     numbers = Slist([2, 3, 4, 5, 6, 7, 8, 9, 1])
     assert numbers.min_by(identity) == 1
     empty = Slist([])
     assert empty.min_by(identity) is None
+
+
+def test_mode_option():
+    numbers = Slist([1, 1, 2, 3, 4, 5, 6, 7, 8, 9, 1])
+    assert numbers.mode_option == 1
+    empty = Slist([])
+    assert empty.mode_option is None
```

### Comparing `slist-0.1.6/PKG-INFO` & `slist-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slist
-Version: 0.1.6
+Version: 0.1.7
 Summary: A typesafe list with more method chaining!
 Home-page: https://github.com/thejaminator/slist
 License: MIT
 Author: James Chua
 Author-email: chuajamessh@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,17 +13,14 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Slist
```

