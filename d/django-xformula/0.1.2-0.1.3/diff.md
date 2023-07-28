# Comparing `tmp/django_xformula-0.1.2.tar.gz` & `tmp/django_xformula-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_xformula-0.1.2.tar", max compression
+gzip compressed data, was "django_xformula-0.1.3.tar", max compression
```

## Comparing `django_xformula-0.1.2.tar` & `django_xformula-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1104 2022-10-24 16:31:45.723000 django_xformula-0.1.2/LICENSE
--rw-r--r--   0        0        0     1517 2022-11-13 22:58:43.377529 django_xformula-0.1.2/README.md
--rw-r--r--   0        0        0     1118 2022-11-13 23:05:40.947948 django_xformula-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      510 2022-11-13 22:46:12.854114 django_xformula-0.1.2/src/django_xformula/__init__.py
--rw-r--r--   0        0        0       56 2022-11-13 23:05:47.080351 django_xformula-0.1.2/src/django_xformula/__version__.py
--rw-r--r--   0        0        0      120 2022-11-13 22:46:13.120939 django_xformula-0.1.2/src/django_xformula/apps/__init__.py
--rw-r--r--   0        0        0      210 2022-11-13 22:46:13.222736 django_xformula-0.1.2/src/django_xformula/apps/django_xformula_config.py
--rw-r--r--   0        0        0        0 2022-11-13 22:46:13.323049 django_xformula-0.1.2/src/django_xformula/db/__init__.py
--rw-r--r--   0        0        0       76 2022-11-13 22:46:13.423473 django_xformula-0.1.2/src/django_xformula/db/lookups/__init__.py
--rw-r--r--   0        0        0      744 2022-11-13 22:46:13.531373 django_xformula-0.1.2/src/django_xformula/db/lookups/pure.py
--rw-r--r--   0        0        0      200 2022-11-13 22:46:13.656247 django_xformula-0.1.2/src/django_xformula/errors/__init__.py
--rw-r--r--   0        0        0      732 2022-11-13 22:46:13.767381 django_xformula-0.1.2/src/django_xformula/errors/forbidden_attribute.py
--rw-r--r--   0        0        0      886 2022-11-13 22:46:13.855421 django_xformula-0.1.2/src/django_xformula/errors/forbidden_call.py
--rw-r--r--   0        0        0      218 2022-11-13 22:46:13.945708 django_xformula-0.1.2/src/django_xformula/evaluator/__init__.py
--rw-r--r--   0        0        0    21936 2022-11-13 22:46:14.027933 django_xformula-0.1.2/src/django_xformula/evaluator/bidirectional_operator.py
--rw-r--r--   0        0        0    12425 2022-11-13 22:46:14.116980 django_xformula-0.1.2/src/django_xformula/evaluator/query_evaluator.py
--rw-r--r--   0        0        0      175 2022-11-13 22:46:14.185713 django_xformula-0.1.2/src/django_xformula/protocols/__init__.py
--rw-r--r--   0        0        0      244 2022-11-13 22:46:14.252843 django_xformula-0.1.2/src/django_xformula/protocols/attribute_getter.py
--rw-r--r--   0        0        0      329 2022-11-13 22:46:14.313215 django_xformula-0.1.2/src/django_xformula/protocols/caller.py
--rw-r--r--   0        0        0      124 2022-11-13 22:46:14.382095 django_xformula-0.1.2/src/django_xformula/tests/__init__.py
--rw-r--r--   0        0        0      159 2022-11-13 22:46:14.459241 django_xformula-0.1.2/src/django_xformula/tests/evaluator/__init__.py
--rw-r--r--   0        0        0      525 2022-11-13 22:46:14.537418 django_xformula-0.1.2/src/django_xformula/tests/evaluator/query_evaluator_test_case.py
--rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 django_xformula-0.1.2/setup.py
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 django_xformula-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1104 2022-10-24 16:31:45.723000 django_xformula-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1517 2022-11-13 22:58:43.377529 django_xformula-0.1.3/README.md
+-rw-r--r--   0        0        0     1112 2023-07-28 11:19:41.716173 django_xformula-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      510 2022-11-13 22:46:12.854114 django_xformula-0.1.3/src/django_xformula/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-28 11:17:53.666286 django_xformula-0.1.3/src/django_xformula/__version__.py
+-rw-r--r--   0        0        0      120 2022-11-13 22:46:13.120939 django_xformula-0.1.3/src/django_xformula/apps/__init__.py
+-rw-r--r--   0        0        0      210 2022-11-13 22:46:13.222736 django_xformula-0.1.3/src/django_xformula/apps/django_xformula_config.py
+-rw-r--r--   0        0        0        0 2022-11-13 22:46:13.323049 django_xformula-0.1.3/src/django_xformula/db/__init__.py
+-rw-r--r--   0        0        0       76 2022-11-13 22:46:13.423473 django_xformula-0.1.3/src/django_xformula/db/lookups/__init__.py
+-rw-r--r--   0        0        0      744 2022-11-13 22:46:13.531373 django_xformula-0.1.3/src/django_xformula/db/lookups/pure.py
+-rw-r--r--   0        0        0      200 2022-11-13 22:46:13.656247 django_xformula-0.1.3/src/django_xformula/errors/__init__.py
+-rw-r--r--   0        0        0      732 2022-11-13 22:46:13.767381 django_xformula-0.1.3/src/django_xformula/errors/forbidden_attribute.py
+-rw-r--r--   0        0        0      886 2022-11-13 22:46:13.855421 django_xformula-0.1.3/src/django_xformula/errors/forbidden_call.py
+-rw-r--r--   0        0        0      218 2022-11-13 22:46:13.945708 django_xformula-0.1.3/src/django_xformula/evaluator/__init__.py
+-rw-r--r--   0        0        0    21873 2023-07-28 11:17:34.002845 django_xformula-0.1.3/src/django_xformula/evaluator/bidirectional_operator.py
+-rw-r--r--   0        0        0    12425 2022-11-13 22:46:14.116980 django_xformula-0.1.3/src/django_xformula/evaluator/query_evaluator.py
+-rw-r--r--   0        0        0      175 2022-11-13 22:46:14.185713 django_xformula-0.1.3/src/django_xformula/protocols/__init__.py
+-rw-r--r--   0        0        0      244 2022-11-13 22:46:14.252843 django_xformula-0.1.3/src/django_xformula/protocols/attribute_getter.py
+-rw-r--r--   0        0        0      329 2022-11-13 22:46:14.313215 django_xformula-0.1.3/src/django_xformula/protocols/caller.py
+-rw-r--r--   0        0        0      124 2022-11-13 22:46:14.382095 django_xformula-0.1.3/src/django_xformula/tests/__init__.py
+-rw-r--r--   0        0        0      159 2022-11-13 22:46:14.459241 django_xformula-0.1.3/src/django_xformula/tests/evaluator/__init__.py
+-rw-r--r--   0        0        0      525 2022-11-13 22:46:14.537418 django_xformula-0.1.3/src/django_xformula/tests/evaluator/query_evaluator_test_case.py
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 django_xformula-0.1.3/PKG-INFO
```

### Comparing `django_xformula-0.1.2/LICENSE` & `django_xformula-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/README.md` & `django_xformula-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/pyproject.toml` & `django_xformula-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "django-xformula"
-version = "0.1.2"
+version = "0.1.3"
 description = "Django query evaluator, is built on top of XFormula language front-end."
 authors = ["Ertuğrul Keremoğlu <ertugkeremoglu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [
-	{include = "django_xformula", from = "src" },
-]
+packages = [{ include = "django_xformula", from = "src" }]
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 django = "*"
 xformula = "^0.1.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 commitizen = "^2.35.0"
-django-stubs = {extras = ["compatible-mypy"], version = "^1.13.0"}
+django-stubs = { extras = ["compatible-mypy"], version = "^1.13.0" }
 isort = "^5.10.1"
 mypy = "^0.982"
 pycln = "^2.1.1"
 
 
 [tool.poetry.group.rel.dependencies]
 build = "^0.8.0"
@@ -44,15 +42,12 @@
 	"pyproject.toml:tool.poetry.version",
 	"src/django_xformula/__version__.py:__version__",
 ]
 
 
 [tool.isort]
 profile = "black"
-known_first_party = [
-	"django_xformula",
-	"django_xformula_unittests",
-]
+known_first_party = ["django_xformula", "django_xformula_unittests"]
 
 
 [tool.pycln]
 all = true
```

### Comparing `django_xformula-0.1.2/src/django_xformula/db/lookups/pure.py` & `django_xformula-0.1.3/src/django_xformula/db/lookups/pure.py`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/src/django_xformula/errors/forbidden_attribute.py` & `django_xformula-0.1.3/src/django_xformula/errors/forbidden_attribute.py`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/src/django_xformula/errors/forbidden_call.py` & `django_xformula-0.1.3/src/django_xformula/errors/forbidden_call.py`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/src/django_xformula/evaluator/bidirectional_operator.py` & `django_xformula-0.1.3/src/django_xformula/evaluator/bidirectional_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -748,21 +748,21 @@
                 return lhs != rhs
             return lhs is not rhs
 
         lhs = cls.ensure_py_object(lhs)
         rhs = cls.ensure_py_object(rhs)
 
         if lhs is None and rhs is None:
-            return IsNull(Value(None), Value(False))
+            return IsNull(Value(None), False)
 
         if lhs is None and rhs is not None:
-            return IsNull(rhs, Value(False))
+            return IsNull(rhs, False)
 
         if lhs is not None and rhs is None:
-            return IsNull(lhs, Value(False))
+            return IsNull(lhs, False)
 
         lhs = cls.ensure_if_combinable(lhs)
         rhs = cls.ensure_if_combinable(rhs)
 
         return Exact(Exact(lhs, rhs), Value(False))
 
     @classmethod
@@ -776,21 +776,21 @@
                 return lhs == rhs
             return lhs is rhs
 
         lhs = cls.ensure_py_object(lhs)
         rhs = cls.ensure_py_object(rhs)
 
         if lhs is None and rhs is None:
-            return IsNull(Value(None), Value(True))
+            return IsNull(Value(None), True)
 
         if lhs is None and rhs is not None:
-            return IsNull(rhs, Value(True))
+            return IsNull(rhs, True)
 
         if lhs is not None and rhs is None:
-            return IsNull(lhs, Value(True))
+            return IsNull(lhs, True)
 
         lhs = cls.ensure_if_combinable(lhs)
         rhs = cls.ensure_if_combinable(rhs)
 
         return Exact(lhs, rhs)
 
     @classmethod
@@ -887,21 +887,21 @@
         if not cls.any_queryable(lhs, rhs):
             return lhs == rhs
 
         lhs = cls.ensure_py_object(lhs)
         rhs = cls.ensure_py_object(rhs)
 
         if lhs is None and rhs is None:
-            return IsNull(Value(None), Value(True))
+            return IsNull(Value(None), True)
 
         if lhs is None and rhs is not None:
-            return IsNull(rhs, Value(True))
+            return IsNull(rhs, True)
 
         if lhs is not None and rhs is None:
-            return IsNull(lhs, Value(True))
+            return IsNull(lhs, True)
 
         lhs = cls.ensure_if_combinable(lhs)
         rhs = cls.ensure_if_combinable(rhs)
 
         return Exact(lhs, rhs)
 
     @classmethod
```

### Comparing `django_xformula-0.1.2/src/django_xformula/evaluator/query_evaluator.py` & `django_xformula-0.1.3/src/django_xformula/evaluator/query_evaluator.py`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/src/django_xformula/tests/evaluator/query_evaluator_test_case.py` & `django_xformula-0.1.3/src/django_xformula/tests/evaluator/query_evaluator_test_case.py`

 * *Files identical despite different names*

### Comparing `django_xformula-0.1.2/PKG-INFO` & `django_xformula-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-xformula
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django query evaluator, is built on top of XFormula language front-end.
 License: MIT
 Author: Ertuğrul Keremoğlu
 Author-email: ertugkeremoglu@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

