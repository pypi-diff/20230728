# Comparing `tmp/structio-1.3.5.tar.gz` & `tmp/structio-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.3.5.tar", last modified: Mon Jul 24 14:03:38 2023, max compression
+gzip compressed data, was "structio-1.3.6.tar", last modified: Fri Jul 28 03:55:32 2023, max compression
```

## Comparing `structio-1.3.5.tar` & `structio-1.3.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:38.704007 structio-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-24 14:03:38.704007 structio-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-24 14:03:17.000000 structio-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 14:03:17.000000 structio-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:03:38.704007 structio-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:38.704007 structio-1.3.5/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-24 14:03:17.000000 structio-1.3.5/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:55:32.121395 structio-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-28 03:55:32.121395 structio-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-28 03:55:16.000000 structio-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 03:55:16.000000 structio-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 03:55:32.121395 structio-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:55:32.121395 structio-1.3.6/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-28 03:55:32.000000 structio-1.3.6/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-28 03:55:32.000000 structio-1.3.6/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:55:32.000000 structio-1.3.6/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 03:55:32.000000 structio-1.3.6/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-28 03:55:16.000000 structio-1.3.6/structio.py
```

### Comparing `structio-1.3.5/PKG-INFO` & `structio-1.3.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -66,15 +66,15 @@
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
 
 **Struct(endian='little', encoding='utf-8', errors='ignore')**
 
-Creates a new *Struct* object with the provided arguments as defaults. The *endian* argument specifies the default endian that would be used by the object, should either be *'little'* or *'big'*.
+Creates a new *Struct* object with the provided arguments used as defaults.
 
 **unpack_bool(b)**
 
 Converts byte *b* into a boolean. Returns False if *b* is a null byte, otherwise returns True.
 
 **pack_bool(boolean)**
 
@@ -142,25 +142,25 @@
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
 **buffer**: the current content of the object (read only).
 
-**endian**: the default endian that would be used by the object (read only).
+**endian**: the default endian that would be used by the object.
 
-**encoding**: the default encoding used by string methods (read only).
+**encoding**: the default encoding used by string methods.
 
-**errors**: the default error handling behavior when encoding or decoding strings (read only).
+**errors**: the default error handling behavior when encoding or decoding strings.
 
 ### Methods
 
-**StructIO(b=b'', struct=_struct)**
+**StructIO(b=b'', endian='little', encoding='utf-8', errors='ignore')**
 
-Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
+Take bytes object *b* and returns a *StructIO* instance containing *b* with the provided arguments used as defaults.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
 
 **\_\_eq\_\_(other)**
 
@@ -365,22 +365,21 @@
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
 ```
 
 As well as the stream object:
 
 ```python
-extended_struct = ExtendedStruct()
-
 class ExtendedStructIO(StructIO):
-    def __init__(self, b=b'', struct=extended_struct):
-        super().__init__(b, struct)
+    def __init__(self, b=b'', endian='little'):
+        super().__init__(b)
+        self._struct = ExtendedStruct(endian)
         
     def copy(self):
-        return ExtendedStructIO(self.getvalue(), self._struct)
+        return ExtendedStructIO(self.getvalue(), self._struct.endian)
         
     def _get_7bstr_len(self):
         return self._struct._get_7bstr_len(self.getvalue(), start=self.tell())
         
     def read_7bstr(self):
         value, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell())
         self.seek(length, 1)
```

### Comparing `structio-1.3.5/README.md` & `structio-1.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
 
 **Struct(endian='little', encoding='utf-8', errors='ignore')**
 
-Creates a new *Struct* object with the provided arguments as defaults. The *endian* argument specifies the default endian that would be used by the object, should either be *'little'* or *'big'*.
+Creates a new *Struct* object with the provided arguments used as defaults.
 
 **unpack_bool(b)**
 
 Converts byte *b* into a boolean. Returns False if *b* is a null byte, otherwise returns True.
 
 **pack_bool(boolean)**
 
@@ -134,25 +134,25 @@
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
 **buffer**: the current content of the object (read only).
 
-**endian**: the default endian that would be used by the object (read only).
+**endian**: the default endian that would be used by the object.
 
-**encoding**: the default encoding used by string methods (read only).
+**encoding**: the default encoding used by string methods.
 
-**errors**: the default error handling behavior when encoding or decoding strings (read only).
+**errors**: the default error handling behavior when encoding or decoding strings.
 
 ### Methods
 
-**StructIO(b=b'', struct=_struct)**
+**StructIO(b=b'', endian='little', encoding='utf-8', errors='ignore')**
 
-Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
+Take bytes object *b* and returns a *StructIO* instance containing *b* with the provided arguments used as defaults.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
 
 **\_\_eq\_\_(other)**
 
@@ -357,22 +357,21 @@
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
 ```
 
 As well as the stream object:
 
 ```python
-extended_struct = ExtendedStruct()
-
 class ExtendedStructIO(StructIO):
-    def __init__(self, b=b'', struct=extended_struct):
-        super().__init__(b, struct)
+    def __init__(self, b=b'', endian='little'):
+        super().__init__(b)
+        self._struct = ExtendedStruct(endian)
         
     def copy(self):
-        return ExtendedStructIO(self.getvalue(), self._struct)
+        return ExtendedStructIO(self.getvalue(), self._struct.endian)
         
     def _get_7bstr_len(self):
         return self._struct._get_7bstr_len(self.getvalue(), start=self.tell())
         
     def read_7bstr(self):
         value, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell())
         self.seek(length, 1)
```

### Comparing `structio-1.3.5/structio.egg-info/PKG-INFO` & `structio-1.3.6/structio.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -66,15 +66,15 @@
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
 
 **Struct(endian='little', encoding='utf-8', errors='ignore')**
 
-Creates a new *Struct* object with the provided arguments as defaults. The *endian* argument specifies the default endian that would be used by the object, should either be *'little'* or *'big'*.
+Creates a new *Struct* object with the provided arguments used as defaults.
 
 **unpack_bool(b)**
 
 Converts byte *b* into a boolean. Returns False if *b* is a null byte, otherwise returns True.
 
 **pack_bool(boolean)**
 
@@ -142,25 +142,25 @@
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
 **buffer**: the current content of the object (read only).
 
-**endian**: the default endian that would be used by the object (read only).
+**endian**: the default endian that would be used by the object.
 
-**encoding**: the default encoding used by string methods (read only).
+**encoding**: the default encoding used by string methods.
 
-**errors**: the default error handling behavior when encoding or decoding strings (read only).
+**errors**: the default error handling behavior when encoding or decoding strings.
 
 ### Methods
 
-**StructIO(b=b'', struct=_struct)**
+**StructIO(b=b'', endian='little', encoding='utf-8', errors='ignore')**
 
-Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
+Take bytes object *b* and returns a *StructIO* instance containing *b* with the provided arguments used as defaults.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
 
 **\_\_eq\_\_(other)**
 
@@ -365,22 +365,21 @@
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
 ```
 
 As well as the stream object:
 
 ```python
-extended_struct = ExtendedStruct()
-
 class ExtendedStructIO(StructIO):
-    def __init__(self, b=b'', struct=extended_struct):
-        super().__init__(b, struct)
+    def __init__(self, b=b'', endian='little'):
+        super().__init__(b)
+        self._struct = ExtendedStruct(endian)
         
     def copy(self):
-        return ExtendedStructIO(self.getvalue(), self._struct)
+        return ExtendedStructIO(self.getvalue(), self._struct.endian)
         
     def _get_7bstr_len(self):
         return self._struct._get_7bstr_len(self.getvalue(), start=self.tell())
         
     def read_7bstr(self):
         value, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell())
         self.seek(length, 1)
```

### Comparing `structio-1.3.5/structio.py` & `structio-1.3.6/structio.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,52 +127,62 @@
         while number > 127:
             b += self.pack_int(number & 0b01111111 | 0b10000000, 1) 
             number >>= 7
             
         b += self.pack_int(number, 1)
         return b
         
-_struct = Struct()
-
 class StructIO(io.BytesIO):
-    def __init__(self, b=b'', struct=_struct):
+    def __init__(self, b=b'', endian='little', encoding='utf-8', errors='ignore'):
         super().__init__(b)
-        self._struct = struct
+        self._struct = Struct(endian, encoding, errors)
         
     @property
     def buffer(self):
         return self.getvalue()
         
     @property
     def endian(self):
         return self._struct.endian
         
+    @endian.setter
+    def endian(self, value):
+        self._struct.endian = value
+        
     @property
     def encoding(self):
         return self._struct.encoding
         
+    @encoding.setter
+    def encoding(self, value):
+        self._struct.encoding = value
+        
     @property
     def errors(self):
         return self._struct.errors
         
+    @errors.setter
+    def errors(self, value):
+        self._struct.errors = value
+        
     def __len__(self):
         return len(self.getvalue())
         
     def __eq__(self, other):
         return self.getvalue() == other.getvalue()
         
     def is_eof(self):
         if self.read(1) == b'':
             return True
         else:
             self.seek(-1, 1)
             return False
             
     def copy(self):
-        return StructIO(self.getvalue(), self._struct)
+        return StructIO(self.getvalue(), self._struct.endian, self._struct.encoding, self._struct.errors)
         
     def read_all(self):
         self.seek(0)
         return self.getvalue()
         
     def write_all(self, buffer):
         self.seek(0)
```

