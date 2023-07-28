# Comparing `tmp/dataclasses_struct-0.6.0.tar.gz` & `tmp/dataclasses_struct-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_struct-0.6.0.tar", max compression
+gzip compressed data, was "dataclasses_struct-0.7.0.tar", max compression
```

## Comparing `dataclasses_struct-0.6.0.tar` & `dataclasses_struct-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/LICENSE
--rw-r--r--   0        0        0     4656 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/README.md
--rw-r--r--   0        0        0      676 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/__init__.py
--rw-r--r--   0        0        0     4114 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/dataclass.py
--rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/ext/__init__.py
--rw-r--r--   0        0        0     1781 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/ext/mypy_plugin.py
--rw-r--r--   0        0        0     4438 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/field.py
--rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/py.typed
--rw-r--r--   0        0        0      313 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/sizes.py
--rw-r--r--   0        0        0     1346 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/types.py
--rw-r--r--   0        0        0     1046 2023-07-26 00:01:22.832788 dataclasses_struct-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5487 1970-01-01 00:00:00.000000 dataclasses_struct-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5340 2023-07-28 03:31:38.580475 dataclasses_struct-0.7.0/README.md
+-rw-r--r--   0        0        0      706 2023-07-27 21:59:59.471071 dataclasses_struct-0.7.0/dataclasses_struct/__init__.py
+-rw-r--r--   0        0        0     8928 2023-07-28 03:31:38.580475 dataclasses_struct-0.7.0/dataclasses_struct/dataclass.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.7.0/dataclasses_struct/ext/__init__.py
+-rw-r--r--   0        0        0     1834 2023-07-28 03:31:38.580475 dataclasses_struct-0.7.0/dataclasses_struct/ext/mypy_plugin.py
+-rw-r--r--   0        0        0     4429 2023-07-27 22:31:52.560957 dataclasses_struct-0.7.0/dataclasses_struct/field.py
+-rw-r--r--   0        0        0      313 2023-07-27 22:18:30.718550 dataclasses_struct-0.7.0/dataclasses_struct/intsizes.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.7.0/dataclasses_struct/py.typed
+-rw-r--r--   0        0        0     1340 2023-07-27 21:05:55.445954 dataclasses_struct-0.7.0/dataclasses_struct/types.py
+-rw-r--r--   0        0        0     1046 2023-07-28 03:32:25.032358 dataclasses_struct-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6171 1970-01-01 00:00:00.000000 dataclasses_struct-0.7.0/PKG-INFO
```

### Comparing `dataclasses_struct-0.6.0/LICENSE` & `dataclasses_struct-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.6.0/README.md` & `dataclasses_struct-0.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,28 +14,41 @@
 ```python
 from typing import Annotated  # use typing_extensions on Python <3.9
 import dataclasses_struct as dcs
 
 @dcs.dataclass()
 class Test:
     x: int  # or dcs.I64, i.e., a signed 64-bit integer
-    y: float  # or dcs.Float64, i.e., a double-precision (64-bit) floating point
+    y: float  # or dcs.F64, i.e., a double-precision (64-bit) floating point
     z: dcs.U8  # unsigned 8-bit integer
     s: Annotated[bytes, 10]  # fixed-length byte array of length 10
+
+@dcs.dataclass()
+class Container:
+    test1: Test
+    test2: Test
 ```
 
 ```python
->>> t = Test(100, -0.25, 0xff, b'12345')
->>> t
+>>> dcs.is_dataclass_struct(Test)
+True
+>>> t1 = Test(100, -0.25, 0xff, b'12345')
+>>> dcs.is_dataclass_struct(t1)
+True
+>>> t1
 Test(x=100, y=-0.25, z=255, s=b'12345')
->>> packed = t.pack()
+>>> packed = t1.pack()
 >>> packed
 b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xd0\xbf\xff12345\x00\x00\x00\x00\x00'
 >>> Test.from_packed(packed)
 Test(x=100, y=-0.25, z=255, s=b'12345\x00\x00\x00\x00\x00')
+>>> t2 = Test(1, 100, 12, b'hello, world')
+>>> c = Container(t1, t2)
+>>> Container.from_packed(c.pack())
+Container(test1=Test(x=100, y=-0.25, z=255, s=b'12345\x00\x00\x00\x00\x00'), test2=Test(x=1, y=100.0, z=12, s=b'hello, wor'))
 ```
 
 ## Installation
 
 This package is available on pypi:
 
 ```
@@ -88,46 +101,57 @@
 
     # Only supported with NATIVE_ENDIAN_ALIGNED
     unsigned_size: dcs.Size
     signed_size: dcs.SSize
     pointer: dcs.Pointer
 
     # Floating point types
-    single_precision: dcs.Float32  # equivalent to float in C
-    double_precision: dcs.Float64  # equivalent to double in C
-    double_precision_alias: float  # alias for Float64
+    single_precision: dcs.F32  # equivalent to float in C
+    double_precision: dcs.F64  # equivalent to double in C
+    double_precision_alias: float  # alias for F64
 
     # Byte arrays: values shorter than size will be padded with b'\x00'
     array: Annotated[bytes, 100]  # an array of length 100
 
     # Pad bytes can be added before and after fields: a b'\x00' will be
     # inserted for each pad byte.
     pad_before: Annotated[int, dcs.PadBefore(4)]
     pad_after: Annotated[int, dcs.PadAfter(2)]
     pad_before_and_after: Annotated[int, dcs.PadBefore(3), dcs.PadAfter(2)]
+
+# Also supports nesting dataclass-structs
+@dcs.dataclass(endians[0])  # endianness of contained classes must match
+class Container:
+    contained1: Test
+
+    # supports PadBefore and PadAfter as well:
+    contained2: Annotated[Test, dcs.PadBefore(10)]
 ```
 
 Decorated classes are transformed to a standard Python
 [dataclass](https://docs.python.org/3/library/dataclasses.html) with boilerplate
 `__init__`, `__repr__`, `__eq__` etc. auto-generated. Additionally, two methods
 are added to the class: `pack`, a method for packing an instance of the class to
 `bytes`, and `from_packed`, a class method that returns a new instance of the
 class from its packed `bytes` representation.
 
-An additional class attribute, `__dataclass_struct__`, of type
-[`struct.Struct`](https://docs.python.org/3/library/struct.html#struct.Struct)
-is added. The [`struct` format
-string](https://docs.python.org/3/library/struct.html#format-strings) and packed
-size can be accessed like so:
+A class or object can be check to see if it is a dataclass-struct using the
+`is_dataclass_struct` function.
+
+An additional class attribute, `__dataclass_struct__`. The [`struct` format
+string](https://docs.python.org/3/library/struct.html#format-strings), packed
+size, and endianness can be accessed like so:
 
 ```python
 >>> Test.__dataclass_struct__.format
 '@cc??bBhHiIQqqNnPfdd100s4xqq2x3xq2x'
 >>> Test.__dataclass_struct__.size
 234
+>>> Test.__dataclass_struct__.endianness
+'@'
 ```
 
 Default attribute values will be validated against their expected type and
 allowable value range. For example,
 
 ```python3
 import dataclasses_struct as dcs
```

### Comparing `dataclasses_struct-0.6.0/dataclasses_struct/ext/mypy_plugin.py` & `dataclasses_struct-0.7.0/dataclasses_struct/ext/mypy_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         tvar_def=tvd,
         is_classmethod=True,
     )
     add_attribute_to_class(
         ctx.api,
         ctx.cls,
         '__dataclass_struct__',
-        ctx.api.named_type('struct.Struct'),
+        ctx.api.named_type(
+            'dataclasses_struct.dataclass._DataclassStructInternal'),
         is_classvar=True,
     )
 
     # Not sure if this is the right thing to do here... needed because
     # @dataclass_transform doesn't seem to work with mypy when using this
     # custom plugin.
     dataclass_class_maker_callback(ctx)
```

### Comparing `dataclasses_struct-0.6.0/dataclasses_struct/field.py` & `dataclasses_struct-0.7.0/dataclasses_struct/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from ctypes import c_size_t, c_ssize_t, c_void_p, sizeof
 from typing import Generic, Literal, Type, TypeVar
 
-from . import sizes as intsizes
+from . import intsizes
 
 T = TypeVar('T')
 
 
 class Field(abc.ABC, Generic[T]):
     native_only: bool = False
     type_: Type[T]
```

### Comparing `dataclasses_struct-0.6.0/dataclasses_struct/types.py` & `dataclasses_struct-0.7.0/dataclasses_struct/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Single char type
 Char = Annotated[bytes, field.CharField()]
 
 # Boolean type
 Bool = Annotated[bool, field.BoolField()]
 
-# Ieger types
+# Integer types
 I8 = Annotated[int, field.SignedIntField(1)]
 U8 = Annotated[int, field.UnsignedIntField(1)]
 I16 = Annotated[int, field.SignedIntField(2)]
 U16 = Annotated[int, field.UnsignedIntField(2)]
 I32 = Annotated[int, field.SignedIntField(4)]
 U32 = Annotated[int, field.UnsignedIntField(4)]
 I64 = Annotated[int, field.SignedIntField(8)]
@@ -20,16 +20,16 @@
 
 # Native size types
 Size = Annotated[int, field.UnsignedSizeField()]
 SSize = Annotated[int, field.SignedSizeField()]
 Pointer = Annotated[int, field.PointerField()]
 
 # Floating point types
-Float32 = Annotated[float, field.Float32Field()]
-Float64 = Annotated[float, field.Float64Field()]
+F32 = Annotated[float, field.Float32Field()]
+F64 = Annotated[float, field.Float64Field()]
 
 
 class _Padding:
     before: bool
 
     def __init__(self, size: int):
         if size < 0:
```

### Comparing `dataclasses_struct-0.6.0/pyproject.toml` & `dataclasses_struct-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-struct"
-version = "0.6.0"
+version = "0.7.0"
 description = "Converting dataclasses to and from fixed-length binary data using struct"
 authors = ["Harry Mander <harrymander96@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/harrymander/dataclasses-struct"
 repository = "https://github.com/harrymander/dataclasses-struct"
 documentation = "https://github.com/harrymander/dataclasses-struct/blob/main/README.md#usage"
```

### Comparing `dataclasses_struct-0.6.0/PKG-INFO` & `dataclasses_struct-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-struct
-Version: 0.6.0
+Version: 0.7.0
 Summary: Converting dataclasses to and from fixed-length binary data using struct
 Home-page: https://github.com/harrymander/dataclasses-struct
 License: MIT
 Author: Harry Mander
 Author-email: harrymander96@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -33,28 +33,41 @@
 ```python
 from typing import Annotated  # use typing_extensions on Python <3.9
 import dataclasses_struct as dcs
 
 @dcs.dataclass()
 class Test:
     x: int  # or dcs.I64, i.e., a signed 64-bit integer
-    y: float  # or dcs.Float64, i.e., a double-precision (64-bit) floating point
+    y: float  # or dcs.F64, i.e., a double-precision (64-bit) floating point
     z: dcs.U8  # unsigned 8-bit integer
     s: Annotated[bytes, 10]  # fixed-length byte array of length 10
+
+@dcs.dataclass()
+class Container:
+    test1: Test
+    test2: Test
 ```
 
 ```python
->>> t = Test(100, -0.25, 0xff, b'12345')
->>> t
+>>> dcs.is_dataclass_struct(Test)
+True
+>>> t1 = Test(100, -0.25, 0xff, b'12345')
+>>> dcs.is_dataclass_struct(t1)
+True
+>>> t1
 Test(x=100, y=-0.25, z=255, s=b'12345')
->>> packed = t.pack()
+>>> packed = t1.pack()
 >>> packed
 b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xd0\xbf\xff12345\x00\x00\x00\x00\x00'
 >>> Test.from_packed(packed)
 Test(x=100, y=-0.25, z=255, s=b'12345\x00\x00\x00\x00\x00')
+>>> t2 = Test(1, 100, 12, b'hello, world')
+>>> c = Container(t1, t2)
+>>> Container.from_packed(c.pack())
+Container(test1=Test(x=100, y=-0.25, z=255, s=b'12345\x00\x00\x00\x00\x00'), test2=Test(x=1, y=100.0, z=12, s=b'hello, wor'))
 ```
 
 ## Installation
 
 This package is available on pypi:
 
 ```
@@ -107,46 +120,57 @@
 
     # Only supported with NATIVE_ENDIAN_ALIGNED
     unsigned_size: dcs.Size
     signed_size: dcs.SSize
     pointer: dcs.Pointer
 
     # Floating point types
-    single_precision: dcs.Float32  # equivalent to float in C
-    double_precision: dcs.Float64  # equivalent to double in C
-    double_precision_alias: float  # alias for Float64
+    single_precision: dcs.F32  # equivalent to float in C
+    double_precision: dcs.F64  # equivalent to double in C
+    double_precision_alias: float  # alias for F64
 
     # Byte arrays: values shorter than size will be padded with b'\x00'
     array: Annotated[bytes, 100]  # an array of length 100
 
     # Pad bytes can be added before and after fields: a b'\x00' will be
     # inserted for each pad byte.
     pad_before: Annotated[int, dcs.PadBefore(4)]
     pad_after: Annotated[int, dcs.PadAfter(2)]
     pad_before_and_after: Annotated[int, dcs.PadBefore(3), dcs.PadAfter(2)]
+
+# Also supports nesting dataclass-structs
+@dcs.dataclass(endians[0])  # endianness of contained classes must match
+class Container:
+    contained1: Test
+
+    # supports PadBefore and PadAfter as well:
+    contained2: Annotated[Test, dcs.PadBefore(10)]
 ```
 
 Decorated classes are transformed to a standard Python
 [dataclass](https://docs.python.org/3/library/dataclasses.html) with boilerplate
 `__init__`, `__repr__`, `__eq__` etc. auto-generated. Additionally, two methods
 are added to the class: `pack`, a method for packing an instance of the class to
 `bytes`, and `from_packed`, a class method that returns a new instance of the
 class from its packed `bytes` representation.
 
-An additional class attribute, `__dataclass_struct__`, of type
-[`struct.Struct`](https://docs.python.org/3/library/struct.html#struct.Struct)
-is added. The [`struct` format
-string](https://docs.python.org/3/library/struct.html#format-strings) and packed
-size can be accessed like so:
+A class or object can be check to see if it is a dataclass-struct using the
+`is_dataclass_struct` function.
+
+An additional class attribute, `__dataclass_struct__`. The [`struct` format
+string](https://docs.python.org/3/library/struct.html#format-strings), packed
+size, and endianness can be accessed like so:
 
 ```python
 >>> Test.__dataclass_struct__.format
 '@cc??bBhHiIQqqNnPfdd100s4xqq2x3xq2x'
 >>> Test.__dataclass_struct__.size
 234
+>>> Test.__dataclass_struct__.endianness
+'@'
 ```
 
 Default attribute values will be validated against their expected type and
 allowable value range. For example,
 
 ```python3
 import dataclasses_struct as dcs
```

