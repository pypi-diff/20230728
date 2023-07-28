# Comparing `tmp/ftmq-0.1.4.tar.gz` & `tmp/ftmq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.1.4.tar", max compression
+gzip compressed data, was "ftmq-0.1.5.tar", max compression
```

## Comparing `ftmq-0.1.4.tar` & `ftmq-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.4/LICENSE
--rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-07-27 08:29:13.876418 ftmq-0.1.4/ftmq/__init__.py
--rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.4/ftmq/cli.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.4/ftmq/exceptions.py
--rw-r--r--   0        0        0     5115 2023-06-14 18:50:42.961409 ftmq-0.1.4/ftmq/filters.py
--rw-r--r--   0        0        0     2151 2023-07-26 18:11:21.346315 ftmq-0.1.4/ftmq/io.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.4/ftmq/query.py
--rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.4/ftmq/types.py
--rw-r--r--   0        0        0      973 2023-06-14 20:07:15.762203 ftmq-0.1.4/ftmq/util.py
--rw-r--r--   0        0        0     1388 2023-07-27 08:29:13.876418 ftmq-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5646 1970-01-01 00:00:00.000000 ftmq-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 05:11:44.990689 ftmq-0.1.5/ftmq/__init__.py
+-rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.5/ftmq/cli.py
+-rw-r--r--   0        0        0      287 2023-07-27 16:03:41.306274 ftmq-0.1.5/ftmq/enums.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.5/ftmq/exceptions.py
+-rw-r--r--   0        0        0     4982 2023-07-28 04:09:12.400103 ftmq-0.1.5/ftmq/filters.py
+-rw-r--r--   0        0        0     2151 2023-07-26 18:11:21.346315 ftmq-0.1.5/ftmq/io.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.5/ftmq/query.py
+-rw-r--r--   0        0        0      556 2023-07-28 05:01:23.599175 ftmq-0.1.5/ftmq/types.py
+-rw-r--r--   0        0        0      973 2023-07-28 04:58:52.872628 ftmq-0.1.5/ftmq/util.py
+-rw-r--r--   0        0        0     1415 2023-07-28 05:11:44.990689 ftmq-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5652 1970-01-01 00:00:00.000000 ftmq-0.1.5/PKG-INFO
```

### Comparing `ftmq-0.1.4/LICENSE` & `ftmq-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.4/README.md` & `ftmq-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.4/ftmq/cli.py` & `ftmq-0.1.5/ftmq/cli.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.4/ftmq/filters.py` & `ftmq-0.1.5/ftmq/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from banal import as_bool, ensure_list
 from followthemoney import model
 from followthemoney.property import Property
 from followthemoney.schema import Schema
 from nomenklatura.dataset import Dataset
 from nomenklatura.entity import CE
 
+from .enums import Operators, Properties, Schemata
 from .exceptions import ValidationError
 from .types import Value
 from .util import StrEnum, make_dataset
 
 
 class BaseFilter:
     instance: Dataset | Schema | Property | None = None
@@ -54,15 +55,15 @@
         if isinstance(value, str):
             value = make_dataset(value)
         return value
 
 
 class SchemaFilter(BaseFilter):
     instance: Schema = None
-    options = StrEnum("Schemata", [k for k in model.schemata.keys()])
+    options = Schemata
 
     def __init__(
         self,
         schema: str | Schema,
         include_descendants: bool = False,
         include_matchable: bool = False,
     ):
@@ -86,17 +87,14 @@
             value = model.get(value)
         return value
 
     def get_str_value(self) -> str:
         return self.instance.name
 
 
-Operators = StrEnum("Operators", ["in", "null", "gt", "gte", "lt", "lte"])
-
-
 class Operator:
     def __init__(self, operator: Operators, value: str | None = None):
         self.operator = self.get_operator(operator)
         self.value = value
 
     def get_value(self):
         if self.operator == "in":
@@ -125,15 +123,15 @@
             return value < parsed_value
         if self.operator == "lte":
             return value <= parsed_value
 
 
 class PropertyFilter(BaseFilter):
     instance: Property = None
-    options = StrEnum("Properties", [n for n in {p.name for p in model.properties}])
+    options = Properties
     value: Value = None
     operator: Operator = None
 
     def __init__(self, prop: Property, value: Value, operator: str | None = None):
         super().__init__(prop)
         self.value = value
         if operator is not None:
```

### Comparing `ftmq-0.1.4/ftmq/io.py` & `ftmq-0.1.5/ftmq/io.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.4/ftmq/query.py` & `ftmq-0.1.5/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.4/ftmq/util.py` & `ftmq-0.1.5/ftmq/util.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.4/pyproject.toml` & `ftmq-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.1.4"
+version = "0.1.5"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -24,15 +24,15 @@
 "Bug Tracker" = "https://github.com/investigativedata/ftmq/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 banal = "^1.0.6"
 followthemoney = "^3.4.0"
-nomenklatura = "<3"
+nomenklatura = "2.14.1"
 orjson = "^3.9.1"
 PyICU = "^2.11"
 smart-open = {version = "6.3.0", extras = ["all"]}
 click = "^8.1.3"
 click-default-group = "^1.2.2"
 cryptography = ">=41.0.2"
 certifi = ">=2023.07.22"
@@ -45,12 +45,13 @@
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pre-commit = "^3.3.3"
 flake8 = "^6.0.0"
 moto = "^4.1.11"
 ipdb = "^0.13.13"
 bump2version = "^1.0.1"
+cloudpickle = "^2.2.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ftmq-0.1.4/PKG-INFO` & `ftmq-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.1.4
+Version: 0.1.5
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Requires-Dist: PyICU (>=2.11,<3.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: certifi (>=2023.07.22)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: cryptography (>=41.0.2)
 Requires-Dist: followthemoney (>=3.4.0,<4.0.0)
-Requires-Dist: nomenklatura (<3)
+Requires-Dist: nomenklatura (==2.14.1)
 Requires-Dist: orjson (>=3.9.1,<4.0.0)
 Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: smart-open[all] (==6.3.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
 Description-Content-Type: text/markdown
```

