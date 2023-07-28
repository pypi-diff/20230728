# Comparing `tmp/keyof-0.2.0.tar.gz` & `tmp/keyof-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyof-0.2.0.tar", max compression
+gzip compressed data, was "keyof-0.3.0.tar", max compression
```

## Comparing `keyof-0.2.0.tar` & `keyof-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-26 06:50:31.381683 keyof-0.2.0/LICENSE
--rw-r--r--   0        0        0     1034 2023-07-26 12:37:09.376172 keyof-0.2.0/README.md
--rw-r--r--   0        0        0      352 2023-07-26 12:33:39.801574 keyof-0.2.0/keyof/__init__.py
--rw-r--r--   0        0        0       58 2023-07-26 07:33:10.064397 keyof-0.2.0/keyof/compat.py
--rw-r--r--   0        0        0     2530 2023-07-26 12:36:08.413708 keyof-0.2.0/keyof/mypy_plugin.py
--rw-r--r--   0        0        0        0 2023-07-26 06:50:01.388419 keyof-0.2.0/keyof/py.typed
--rw-r--r--   0        0        0     2164 2023-07-26 12:37:23.725054 keyof-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 keyof-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 06:50:31.381683 keyof-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1678 2023-07-28 06:21:43.946275 keyof-0.3.0/README.md
+-rw-r--r--   0        0        0      974 2023-07-28 06:08:21.488849 keyof-0.3.0/keyof/__init__.py
+-rw-r--r--   0        0        0      123 2023-07-28 05:59:12.275609 keyof-0.3.0/keyof/compat.py
+-rw-r--r--   0        0        0     3039 2023-07-28 06:08:21.566648 keyof-0.3.0/keyof/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:50:01.388419 keyof-0.3.0/keyof/py.typed
+-rw-r--r--   0        0        0     2164 2023-07-28 06:22:22.897460 keyof-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 keyof-0.3.0/PKG-INFO
```

### Comparing `keyof-0.2.0/LICENSE` & `keyof-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keyof-0.2.0/keyof/mypy_plugin.py` & `keyof-0.3.0/keyof/mypy_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,16 +13,24 @@
     TypedDictType,
     TypeOfAny,
     UnboundType,
     UnionType,
 )
 
 _MIN_MYPY_VERSION = (1, 0, 1)
-_TYPE_NAME: Final = "KeyOf"
-_TYPES_TO_ANALYZE: Final = frozenset(["keyof.KeyOf", "keyof.compat.KeyOf"])
+_TYPES_TO_ANALYZE: Final = frozenset(
+    [
+        "keyof.KeyOf",
+        "keyof.RequiredKeyOf",
+        "keyof.NotRequiredKeyOf",
+        "keyof.compat.KeyOf",
+        "keyof.compat.RequiredKeyOf",
+        "keyof.compat.NotRequiredKeyOf",
+    ]
+)
 
 
 def _create_string_literal(value: str, api: TypeAnalyzerPluginInterface) -> LiteralType:
     return LiteralType(value, api.named_type("builtins.str", []))
 
 
 def _default_type_analysis(api: TypeAnalyser, type_: UnboundType) -> Type:
@@ -33,42 +41,52 @@
     if isinstance(node, TypeInfo):
         return api.analyze_type_with_type_info(node, type_.args, type_)
     return AnyType(TypeOfAny.special_form)
 
 
 def _analyze_typed_dict_key(ctx: AnalyzeTypeContext) -> Type:
     api = cast(TypeAnalyser, ctx.api)
+    type_name = ctx.type.name
     if (args_len := len(ctx.type.args)) != 1:
         api.fail(
-            f'"{_TYPE_NAME}" expects 1 type argument, but {args_len} given',
+            f'"{type_name}" expects 1 type argument, but {args_len} given',
             ctx.context,
             code=TYPE_ARG,
         )
         return _default_type_analysis(api, ctx.type)
     argument = ctx.type.args[0]
     analyzed: Type | None = ctx.api.analyze_type(argument)
     if isinstance(analyzed, TypeAliasType):
         analyzed = analyzed.expand_all_if_possible()
     if not isinstance(analyzed, TypedDictType):
         api.fail(
-            f'Argument 1 to "{_TYPE_NAME}" has incompatible type "{analyzed}"; expected "TypedDict"',
+            f'Argument 1 to "{type_name}" has incompatible type "{analyzed}"; expected "TypedDict"',
             ctx.context,
         )
         return _default_type_analysis(api, ctx.type)
-    return UnionType.make_union([_create_string_literal(value, api) for value in analyzed.items])
+    match type_name:
+        case "KeyOf":
+            keys = set(analyzed.items.keys())
+        case "RequiredKeyOf":
+            keys = analyzed.required_keys
+        case "NotRequiredKeyOf":
+            keys = set(analyzed.items.keys()) - analyzed.required_keys
+        case _:
+            raise RuntimeError(f"Unexpected type name: {type_name!r}")
+    return UnionType.make_union([_create_string_literal(key, api) for key in keys])
 
 
-class CustomPlugin(Plugin):
+class KeyOfPlugin(Plugin):
     def get_type_analyze_hook(self, fullname: str) -> Callable[[AnalyzeTypeContext], Type] | None:
         if fullname in _TYPES_TO_ANALYZE:
             return _analyze_typed_dict_key
         return None
 
 
 def _version_str_to_tuple(version: str) -> tuple[int, ...]:
     return tuple(int(part) for part in version.partition("+")[0].split("."))
 
 
 def plugin(version: str) -> type[Plugin]:
     if _version_str_to_tuple(version) >= _MIN_MYPY_VERSION:
-        return CustomPlugin
+        return KeyOfPlugin
     return Plugin
```

### Comparing `keyof-0.2.0/pyproject.toml` & `keyof-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keyof"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Viliam Valent <keyof@valent.email>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ViliamV/keyof"
 homepage = "https://github.com/ViliamV/keyof"
 packages = [{include = "keyof"}]
```

### Comparing `keyof-0.2.0/PKG-INFO` & `keyof-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyof
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/ViliamV/keyof
 License: MIT
 Author: Viliam Valent
 Author-email: keyof@valent.email
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,23 @@
 (for example `pyproject.toml`)
 
 ```toml
 [tool.mypy]
 plugins = ["keyof.mypy_plugin"]
 ```
 
+## Features
+
+✅ `KeyOf`, `RequiredKeyOf`, and `NotRequiredKeyOf` types
+✅ Supports inheritance
+✅ Plays nicely with other types, e.g. `KeyOf[Foo] | Literal["bar"]`
+✅ compatibility module for `Pylance` and `Pyright`
+
+❌ Generic `TypeVar` arguments
+
 ## Usage
 
 ```python
 from typing import TypedDict
 
 from keyof import KeyOf
 
@@ -56,11 +65,17 @@
     return data[key]
 
 
 data = Data(version=1, command="foo")
 
 get_data(data, "version")  # OK
 
-get_data(data, "not_existing_key") # error
-# Argument 2 to "get_data" has incompatible type "Literal['not_existing_key']"; expected "Literal['version', 'command']"
+get_data(data, "foo")
+# mypy catches the error:
+# error: Argument 2 to "get_data" has incompatible type "Literal['foo']"; expected "Literal['version', 'command']"
 ```
 
+### Usage with other type checkers
+
+Since [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) and [Pyright](https://microsoft.github.io/pyright/#/) don't support plugins
+and cannot correctly handle subclassing of `Any` (new in Python 3.11) there is compatibility module `keyof.compat` that exports the same types but they are only `TypeAlias` for `Any`.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

