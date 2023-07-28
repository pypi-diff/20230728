# Comparing `tmp/bstk_datatables-0.2.1.tar.gz` & `tmp/bstk_datatables-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.2.1.tar", max compression
+gzip compressed data, was "bstk_datatables-0.2.2.tar", max compression
```

## Comparing `bstk_datatables-0.2.1.tar` & `bstk_datatables-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     4244 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/README.md
--rw-r--r--   0        0        0     2358 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3522 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/merge.py
--rw-r--r--   0        0        0     9455 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-07-27 11:20:42.281086 bstk_datatables-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/README.md
+-rw-r--r--   0        0        0     2497 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3522 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     9807 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/table.py
+-rw-r--r--   0        0        0     1680 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/validators/luhn.py
+-rw-r--r--   0        0        0      669 2023-07-28 06:44:08.318630 bstk_datatables-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.2/PKG-INFO
```

### Comparing `bstk_datatables-0.2.1/README.md` & `bstk_datatables-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.1/bstk_datatables/__init__.py` & `bstk_datatables-0.2.2/bstk_datatables/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import re
 import typing
 
 from marshmallow import Schema as MarshmallowSchema
 from marshmallow import fields as marshmallow_fields
 from marshmallow.validate import Regexp as RegexpValidator
 
+from bstk_datatables.validators.luhn import LuhnValidator
+
 """
 Simple mapping from schemafield types to marshmallow field classes
 """
 SCHEMAFIELD_MAP: typing.Dict[typing.AnyStr, typing.Callable] = {
     "bool": marshmallow_fields.Boolean,
     "datetime": marshmallow_fields.AwareDateTime,
     "email": marshmallow_fields.Email,
@@ -18,14 +20,15 @@
     "ip": marshmallow_fields.IPInterface,
     "mac_address": marshmallow_fields.String,
     "number": marshmallow_fields.Number,
     "phone": marshmallow_fields.String,
     "text": marshmallow_fields.String,
     "blob": marshmallow_fields.String,
     "url": marshmallow_fields.Url,
+    "luhn": marshmallow_fields.String,
 }
 
 """
 Any "default" params that should be injected into the marshmallow field constructor
 """
 SCHEMAFIELD_EXTATTR: typing.Dict[
     typing.AnyStr,
@@ -38,14 +41,15 @@
         ),
     },
     "phone": {
         "validate": RegexpValidator(
             regex=r"^([\(]?[\+0-9]{1,}[)]?)?([0-9 \(\)\.\-]{6,})$"
         )
     },
+    "luhn": {"validate": LuhnValidator},
 }
 
 
 def export(
     model: typing.Union[Entry, Enum, Schema, Table]  # noqa: F821
 ) -> typing.Dict[typing.AnyStr, typing.Any]:
     """
```

### Comparing `bstk_datatables-0.2.1/bstk_datatables/entry.py` & `bstk_datatables-0.2.2/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.1/bstk_datatables/enum.py` & `bstk_datatables-0.2.2/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.1/bstk_datatables/merge.py` & `bstk_datatables-0.2.2/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.1/bstk_datatables/schema.py` & `bstk_datatables-0.2.2/bstk_datatables/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 import copy
 import typing
 from dataclasses import dataclass, field
 
 from marshmallow import Schema as MarshmallowSchema
 from marshmallow import fields as marshmallow_fields
 
-from . import SCHEMAFIELD_EXTATTR, SCHEMAFIELD_MAP, name_to_code, schema_to_marshmallow
+from . import (
+    SCHEMAFIELD_EXTATTR,
+    SCHEMAFIELD_MAP,
+    RegexpValidator,
+    name_to_code,
+    re,
+    schema_to_marshmallow,
+)
 from .enum import Enum, PyEnum
 
 
 class NestedSchemaField(marshmallow_fields.Field):
     """
     A little helper class to use if you're nesting a Schema as a field within another marshmallow schema.
     """
@@ -183,14 +190,15 @@
     values: typing.Optional[typing.Any] = None
     default_value: typing.Optional[typing.Any] = None
     lookup: typing.Optional[typing.Any] = None
     required: typing.Optional[bool] = field(default=False)
     readonly: typing.Optional[bool] = field(default=False)
     many: typing.Optional[bool] = field(default=False)
     markup: typing.Optional[typing.Dict] = field(default=None)
+    validator: typing.Optional[typing.AnyStr] = field(default=None)
     _field: marshmallow_fields.Field = field(init=False, default=None)
     _missing_lookup: bool = field(init=False, default=False)
 
     def __post_init__(self):
         self._generate_marshmallow_field()
 
     def attach_lookup(
@@ -205,14 +213,15 @@
             "values",
             "default_value",
             "lookup",
             "required",
             "readonly",
             "many",
             "markup",
+            "validator",
         ]
         rtn = {}
         for _exportfield in _fields:
             if _exportfield == "lookup" and isinstance(
                 self.__dict__[_exportfield], Enum
             ):
                 rtn[_exportfield] = self.__dict__[_exportfield].code
@@ -223,15 +232,15 @@
 
     def _get_mapped_fieldclass(self) -> typing.Callable:
         if self.type in SCHEMAFIELD_MAP:
             return SCHEMAFIELD_MAP[self.type]
 
         raise ValueError(f"Field format type `{self.type}` is invalid")
 
-    def _get_field_params(self) -> typing.Union[None, typing.Dict]:
+    def _get_field_params(self) -> typing.Union[None, typing.Dict]:  # noqa: C901
         _field_params = {}
 
         if self.required is not None:
             _field_params["required"] = self.required
 
         if self.readonly is True:
             _field_params["dump_only"] = True
@@ -251,14 +260,19 @@
                     _field_params["enum"]
                 )
 
         if self.type != "enum":
             if self.default_value is not None:
                 _field_params["dump_default"] = self.default_value
 
+        if self.validator and self.validator[:5] == "regex":
+            _field_params["validate"] = RegexpValidator(
+                regex=self.validator[6:], flags=re.IGNORECASE
+            )
+
         if self.type not in SCHEMAFIELD_EXTATTR:
             return _field_params
 
         return {**_field_params, **SCHEMAFIELD_EXTATTR[self.type]}
 
     def _process_enum_default(self, enum_data: Enum):
         if not self.default_value:
```

### Comparing `bstk_datatables-0.2.1/bstk_datatables/table.py` & `bstk_datatables-0.2.2/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.1/pyproject.toml` & `bstk_datatables-0.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.2.1"
+version = "0.2.2"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.2.1/PKG-INFO` & `bstk_datatables-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.2.1
+Version: 0.2.2
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

