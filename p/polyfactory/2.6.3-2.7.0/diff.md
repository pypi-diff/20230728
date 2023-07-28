# Comparing `tmp/polyfactory-2.6.3.tar.gz` & `tmp/polyfactory-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.6.3.tar", max compression
+gzip compressed data, was "polyfactory-2.7.0.tar", max compression
```

## Comparing `polyfactory-2.6.3.tar` & `polyfactory-2.7.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1092 2023-07-21 15:24:49.338390 polyfactory-2.6.3/LICENSE
--rw-r--r--   0        0        0    24136 2023-07-21 15:24:49.338390 polyfactory-2.6.3/docs/PYPI_README.md
--rw-r--r--   0        0        0      425 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/__init__.py
--rw-r--r--   0        0        0     2525 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/collection_extender.py
--rw-r--r--   0        0        0      912 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    33713 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1912 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2751 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2192 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    14047 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1699 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     8621 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/py.typed
--rw-r--r--   0        0        0     2850 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3908 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3764 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     1948 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1885 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13429 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      433 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      440 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      446 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3635 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6172 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6914 2023-07-21 15:24:49.342390 polyfactory-2.6.3/pyproject.toml
--rw-r--r--   0        0        0    26109 1970-01-01 00:00:00.000000 polyfactory-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-28 17:24:54.344977 polyfactory-2.7.0/LICENSE
+-rw-r--r--   0        0        0    24136 2023-07-28 17:24:54.344977 polyfactory-2.7.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0     2525 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/collection_extender.py
+-rw-r--r--   0        0        0      912 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0     2147 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/attrs_factory.py
+-rw-r--r--   0        0        0    33713 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1912 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2751 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    14595 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1699 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8697 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3909 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3764 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3635 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6875 2023-07-28 17:24:54.348977 polyfactory-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    26133 1970-01-01 00:00:00.000000 polyfactory-2.7.0/PKG-INFO
```

### Comparing `polyfactory-2.6.3/LICENSE` & `polyfactory-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/docs/PYPI_README.md` & `polyfactory-2.7.0/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/collection_extender.py` & `polyfactory-2.7.0/polyfactory/collection_extender.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/constants.py` & `polyfactory-2.7.0/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/decorators.py` & `polyfactory-2.7.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/exceptions.py` & `polyfactory-2.7.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/factories/base.py` & `polyfactory-2.7.0/polyfactory/factories/base.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.7.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.7.0/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.7.0/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.7.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.7.0/polyfactory/factories/pydantic_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     MIN_COLLECTION_LENGTH,
     RANDOMIZE_COLLECTION_LENGTH,
 )
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type, unwrap_optional
-from polyfactory.utils.predicates import is_optional_union, is_safe_subclass
+from polyfactory.utils.predicates import is_optional_union, is_safe_subclass, is_union
 
 try:
     from pydantic import VERSION, BaseModel
     from pydantic.fields import FieldInfo
 except ImportError as e:
     raise MissingDependencyException("pydantic is not installed") from e
 
@@ -76,41 +76,53 @@
         :returns: A PydanticFieldMeta instance.
         """
         if callable(field_info.default_factory):
             default_value = field_info.default_factory()
         else:
             default_value = field_info.default if field_info.default is not Undefined else Null
 
-        name = field_info.alias if field_info.alias and use_alias else field_name
-
         annotation = unwrap_new_type(field_info.annotation)
+        children: list[FieldMeta,] | None = None
+        constraints: Constraints = {}
+        name = field_info.alias if field_info.alias and use_alias else field_name
 
-        if is_optional_union(field_info.annotation):
-            # pydantic v2 do not propagate metadata for Union types #[?]
-            # hence we cannot acquire any constraints w/ straightforward approach
+        # pydantic v2 do not propagate metadata for Union types
+        if is_optional_union(annotation):
             field_info = FieldInfo.from_annotation(unwrap_optional(annotation))
+        elif is_union(annotation):
+            children = [
+                cls.from_field_info(
+                    field_info=FieldInfo.from_annotation(arg),
+                    field_name=field_name,
+                    max_collection_length=max_collection_length,
+                    min_collection_length=min_collection_length,
+                    random=random,
+                    randomize_collection_length=randomize_collection_length,
+                    use_alias=use_alias,
+                )
+                for arg in get_args(annotation)
+            ]
 
         if metadata := [v for v in field_info.metadata if v is not None]:
             constraints = cls.parse_constraints(metadata=metadata)
-        else:
-            constraints = {}
 
         if "url" in constraints:
             # pydantic uses a sentinel value for url constraints
             annotation = str
 
         return PydanticFieldMeta.from_type(
-            name=name,
-            random=random or DEFAULT_RANDOM,
             annotation=annotation,
-            default=default_value,
+            children=children,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
-            randomize_collection_length=randomize_collection_length,
-            min_collection_length=min_collection_length,
+            default=default_value,
             max_collection_length=max_collection_length,
+            min_collection_length=min_collection_length,
+            name=name,
+            random=random or DEFAULT_RANDOM,
+            randomize_collection_length=randomize_collection_length,
         )
 
     @classmethod
     def from_model_field(  # pragma: no cover
         cls,
         model_field: ModelField,  # pyright: ignore
         use_alias: bool,
```

### Comparing `polyfactory-2.6.3/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.7.0/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/field_meta.py` & `polyfactory-2.7.0/polyfactory/field_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         random: Random = DEFAULT_RANDOM,
         name: str = "",
         default: Any = Null,
         constraints: Constraints | None = None,
         randomize_collection_length: bool = RANDOMIZE_COLLECTION_LENGTH,
         min_collection_length: int = MIN_COLLECTION_LENGTH,
         max_collection_length: int = MAX_COLLECTION_LENGTH,
+        children: list[FieldMeta] | None = None,
     ) -> Self:
         """Builder method to create a FieldMeta from a type annotation.
 
         :param annotation: A type annotation.
         :param random: An instance of random.Random.
         :param name: Field name
         :param default: Default value, if any.
@@ -140,19 +141,19 @@
             annotation = container[get_args(annotation)]  # type: ignore
 
         field = cls(
             annotation=annotation,
             random=random,
             name=name,
             default=default,
-            children=None,
+            children=children,
             constraints=constraints,
         )
 
-        if field.type_args:
+        if field.type_args and not field.children:
             if randomize_collection_length:
                 number_of_args = random.randint(min_collection_length, max_collection_length)
             else:
                 number_of_args = 1
 
             extended_type_args = CollectionExtender.extend_type_args(field.annotation, field.type_args, number_of_args)
             field.children = [
```

### Comparing `polyfactory-2.6.3/polyfactory/fields.py` & `polyfactory-2.7.0/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/persistence.py` & `polyfactory-2.7.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/pytest_plugin.py` & `polyfactory-2.7.0/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/utils/helpers.py` & `polyfactory-2.7.0/polyfactory/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """Unwraps optional union types - recursively.
 
     :param annotation: A type annotation, possibly an optional union.
 
     :returns: A type annotation
     """
     while is_optional_union(annotation):
-        annotation = [arg for arg in get_args(annotation) if arg not in (type(None), None)][0]
+        annotation = next(arg for arg in get_args(annotation) if arg not in (type(None), None))
     return annotation
 
 
 def unwrap_annotation(annotation: Any, random: Random) -> Any:
     """Unwraps an annotation.
 
     :param annotation: A type annotation.
```

### Comparing `polyfactory-2.6.3/polyfactory/utils/predicates.py` & `polyfactory-2.7.0/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/complex_types.py` & `polyfactory-2.7.0/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.7.0/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.7.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.7.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.7.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/primitives.py` & `polyfactory-2.7.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/polyfactory/value_generators/regex.py` & `polyfactory-2.7.0/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.3/pyproject.toml` & `polyfactory-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.6.3"
+version = "2.7.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
@@ -16,27 +16,19 @@
 ]
 license = "MIT"
 readme = "docs/PYPI_README.md"
 homepage = "https://github.com/litestar-org/polyfactory"
 repository = "https://github.com/litestar-org/polyfactory"
 documentation = "https://github.com/litestar-org/polyfactory"
 keywords = [
-    "beanie",
     "dataclasses",
     "factory",
-    "faker",
-    "litestar",
-    "mock",
     "msgspec",
-    "odmantic",
     "pydantic",
-    "pytest",
-    "tdd",
     "testing",
-    "typeddict",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -60,14 +52,15 @@
 python = ">=3.8,<4.0"
 beanie = { version = "*", optional = true }
 faker = "*"
 msgspec = { version = "*", optional = true }
 odmantic = { version = "*", optional = true }
 pydantic = { version = "*", optional = true, extras = ["email"] }
 typing-extensions = "*"
+attrs = { version = "*", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "*"
 mongomock-motor = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
@@ -94,19 +87,21 @@
 sourcery = "*"
 
 [tool.poetry.extras]
 pydantic = ["pydantic"]
 msgspec = ["msgspec"]
 odmantic = ["odmantic", "pydantic"]
 beanie = ["beanie", "pydantic"]
+attrs = ["attrs"]
 full = [
     "pydantic",
     "odmantic",
     "msgspec",
     "beanie",
+    "attrs",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `polyfactory-2.6.3/PKG-INFO` & `polyfactory-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.6.3
+Version: 2.7.0
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
-Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
+Keywords: dataclasses,factory,msgspec,pydantic,testing
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
 Maintainer-email: nhirschfeld@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -25,19 +25,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Provides-Extra: attrs
 Provides-Extra: beanie
 Provides-Extra: full
 Provides-Extra: msgspec
 Provides-Extra: odmantic
 Provides-Extra: pydantic
+Requires-Dist: attrs ; extra == "attrs" or extra == "full"
 Requires-Dist: beanie ; extra == "beanie" or extra == "full"
 Requires-Dist: faker
 Requires-Dist: msgspec ; extra == "msgspec" or extra == "full"
 Requires-Dist: odmantic ; extra == "odmantic" or extra == "full"
 Requires-Dist: pydantic[email] ; extra == "pydantic" or extra == "odmantic" or extra == "beanie" or extra == "full"
 Requires-Dist: typing-extensions
 Project-URL: Documentation, https://github.com/litestar-org/polyfactory
```

