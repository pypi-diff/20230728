# Comparing `tmp/regfile-0.1.2.tar.gz` & `tmp/regfile-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regfile-0.1.2.tar", max compression
+gzip compressed data, was "regfile-0.1.3.tar", max compression
```

## Comparing `regfile-0.1.2.tar` & `regfile-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    16725 2023-01-29 20:29:35.121639 regfile-0.1.2/LICENSE
--rw-r--r--   0        0        0      807 2023-03-25 19:07:48.807733 regfile-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      876 2023-03-25 18:49:46.671035 regfile-0.1.2/src/regfile/__init__.py
--rw-r--r--   0        0        0      159 2023-03-19 20:14:14.267422 regfile-0.1.2/src/regfile/common.py
--rwxr-xr-x   0        0        0     5813 2023-03-25 18:49:46.671035 regfile-0.1.2/src/regfile/main.py
--rw-r--r--   0        0        0     1521 2023-03-19 20:14:14.267422 regfile-0.1.2/src/regfile/mime.py
--rw-r--r--   0        0        0     1831 2023-03-25 18:49:46.671035 regfile-0.1.2/src/regfile/postprocessing.py
--rw-r--r--   0        0        0     9944 2023-03-25 19:04:13.748329 regfile-0.1.2/src/regfile/types.py
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 regfile-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-01-29 20:29:35.121639 regfile-0.1.3/LICENSE
+-rw-r--r--   0        0        0      807 2023-07-28 19:04:54.073083 regfile-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      948 2023-07-28 19:02:15.211267 regfile-0.1.3/src/regfile/__init__.py
+-rw-r--r--   0        0        0     7142 2023-07-28 19:02:15.212267 regfile-0.1.3/src/regfile/ast.py
+-rw-r--r--   0        0        0      159 2023-03-19 20:14:14.267422 regfile-0.1.3/src/regfile/common.py
+-rw-r--r--   0        0        0     4357 2023-07-28 19:02:15.212267 regfile-0.1.3/src/regfile/lineprocessing.py
+-rwxr-xr-x   0        0        0     5339 2023-07-28 19:02:15.212267 regfile-0.1.3/src/regfile/main.py
+-rw-r--r--   0        0        0     1521 2023-06-06 11:05:33.753325 regfile-0.1.3/src/regfile/mime.py
+-rw-r--r--   0        0        0    10902 2023-07-28 19:02:15.212267 regfile-0.1.3/src/regfile/types.py
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 regfile-0.1.3/PKG-INFO
```

### Comparing `regfile-0.1.2/LICENSE` & `regfile-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `regfile-0.1.2/pyproject.toml` & `regfile-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "regfile"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["fnrir"]
 license = "MPL-2.0"
 #readme = "README.md"
 repository = "https://gitlab.com/fnrir/regfile"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `regfile-0.1.2/src/regfile/__init__.py` & `regfile-0.1.3/src/regfile/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,52 +7,56 @@
     REG_ENCODING,
 )
 from .mime import (
     MIME,
     MIMEExact,
     MIMEQuoted
 )
-from .postprocessing import (
+from .lineprocessing import (
     linelimit,
-    PostProcessor,
-    PPNone,
-    PPLinelimit,
+    text_to_nvpair,
+    NVLine,
+    LineProcessor,
+    LPNone,
+    LPLinelimit,
 )
 from .types import (
     RegPath,
     Value,
     REG_DWORD,
     REG_QWORD,
     REG_SZ,
     REG_BINARY,
     REG_EXPAND_SZ,
     REG_MULTI_SZ,
     mimemap,
-    value_from_str,
+    value_from_token,
     Key,
 )
 from .main import (
     RegFile,
 )
 
 __all__ = [
     "REG_ENCODING",
     "MIME",
     "MIMEExact",
     "MIMEQuoted",
     "linelimit",
-    "PostProcessor",
-    "PPNone",
-    "PPLinelimit",
+    "text_to_nvpair",
+    "NVLine",
+    "LineProcessor",
+    "LPNone",
+    "LPLinelimit",
     "RegPath",
     "Value",
     "REG_DWORD",
     "REG_QWORD",
     "REG_SZ",
     "REG_BINARY",
     "REG_EXPAND_SZ",
     "REG_MULTI_SZ",
     "mimemap",
-    "value_from_str",
+    "value_from_token",
     "Key",
     "RegFile",
 ]
```

### Comparing `regfile-0.1.2/src/regfile/main.py` & `regfile-0.1.3/src/regfile/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from dataclasses import dataclass
 from pathlib import Path
 from os import (
     PathLike,
     fspath,
 )
 from typing import (
-    Any,
     ClassVar,
     Optional,
     Sequence,
 )
 
+from .ast import (
+    TComment,
+    TKey,
+    RegAst,
+)
 from .common import REG_ENCODING
 from .types import (
     escape,
     RegPath,
-    Value,
-    value_from_str,
     Key,
 )
 
 
 @dataclass
 class RegFileHeader:
     version: str
@@ -62,63 +64,51 @@
 class RegFile:
     header: RegFileHeader
     keys: list[Key]
     root_key: Optional[RegPath]
 
     @classmethod
     def from_str(cls, data: str) -> "RegFile":
-        lines: list[str] = data.replace("\\\n  ", "").split("\n")
+        tokens = RegAst.from_str(data)
         keys: list[Key] = []
-        current_key: Optional[Key] = None
-        header_str: str = ""
+        header_str = ""
         header: Optional[RegFileHeader] = None
         root_key: Optional[Key] = None
-        for line in lines:
-            if line == "":
-                continue
-            if line.startswith("["):
-                path = RegPath.from_str(line[1:-1])
-                key = Key(path)
-                if current_key is None:
-                    header = RegFileHeader.from_str(header_str)
-                current_key = key
-                # The parent key always appears before its child
+        for token in tokens:
+            if isinstance(token, TComment):
+                header_str += token.text + "\n"
+            elif isinstance(token, TKey):
+                key = Key.from_token(token)
                 if key.parent is None:
                     keys.append(key)
                     continue
                 if not keys:
                     # Otherwhise it's a partial reg file
                     if not root_key:
                         root_key = key
                         continue
                     if len(key.parent) == len(root_key.path):
                         root_key.add_subkey(key)
                         continue
+                parent_found = False
                 root_keys = keys.copy()
                 if root_key:
                     root_keys += [root_key]
-                parent_found = False
                 for sub_root_key in root_keys:
                     srk_path = sub_root_key.path
                     if not key.parent.startswith(srk_path):
                         continue
                     parent_key = sub_root_key.find_key(key.parent.path)
                     parent_key.add_subkey(key)
                     parent_found = True
                     break
                 if parent_found:
                     continue
                 raise ValueError(f"{escape(key.name)}'s parent not found'")
-            if current_key is None:
-                header_str += line + "\n"
-                continue
-            value: Value[Any] = value_from_str(line)
-            current_key.add_value(value)
-        if header is None:
-            raise ValueError("Header not found")
+        header = RegFileHeader.from_str(header_str)
         # Add missing keys
         root_path = None
         if root_key:
             tmp = root_key
             tmp_parent: Key
             while tmp.parent:
                 tmp_parent = Key(tmp.parent)
```

### Comparing `regfile-0.1.2/src/regfile/mime.py` & `regfile-0.1.3/src/regfile/mime.py`

 * *Files identical despite different names*

### Comparing `regfile-0.1.2/src/regfile/types.py` & `regfile-0.1.3/src/regfile/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,25 +17,30 @@
     Type,
     TypeVar,
 )
 from typing_extensions import (
     SupportsIndex,
 )
 
+from .ast import (
+    TValue,
+    TKey,
+)
 from .common import (
     REG_ENCODING,
     escape,
 )
 from .mime import (
     MIMEExact,
     MIMEQuoted,
 )
-from .postprocessing import (
-    PPNone,
-    PPLinelimit,
+from .lineprocessing import (
+    NVLine,
+    LPNone,
+    LPLinelimit,
 )
 
 
 @dataclass
 class RegPath(Iterable):
     """
     A path to a registry key.
@@ -85,46 +90,62 @@
         return self.path.__len__()
 
 
 T = TypeVar("T")
 
 
 @dataclass
-class Value(MIMEExact, PPNone, ABC, Generic[T]):
+class Value(MIMEExact, LPNone, ABC, Generic[T]):
     """
     Generic value of a registry key.
     """
     name: str
     value: T
     name_quoted: bool = False
 
     @property
     def typeof(self) -> str:
         return self.__class__.__name__
 
     @classmethod
-    def from_str(cls, name: str, value: str):
+    def from_token(cls, token: TValue) -> "Value":
+        (name, value) = cls.preprocess(tuple(token))
+        name_quoted = False
+        if name.startswith("\""):
+            name = name[1:-1]
+            name_quoted = True
+        value = cls.mime_remove(value)
+        return cls(name, cls.val_conv(value), name_quoted)
+
+    @classmethod
+    def from_line(cls, line: NVLine):
         """
         Create a Value from a string.
 
         Args:
             name: The name of the value.
             value: The value of the value.
 
         Returns:
             A Value.
         """
+        line.process(cls)
+        (name, value) = line
         name_quoted = False
         if name.startswith("\""):
             name = name[1:-1]
             name_quoted = True
         value = cls.mime_remove(value)
         return cls(name, cls.val_conv(value), name_quoted)
 
     @classmethod
+    def from_str(cls, text: str):
+        return cls.from_line(NVLine.from_str(text))
+
+    @classmethod
     @abstractmethod
     def val_conv(cls, value: str) -> T:
         """
         Convert a string to the appropriate type.
 
         Args:
             value: The string to convert.
@@ -142,27 +163,32 @@
         Args:
             value: The value to convert.
 
         Returns:
             The converted string.
         """
 
-    def to_str(self) -> str:
+    def to_line(self) -> NVLine:
         """
         Convert the value to a string.
 
         Returns:
             The converted string
         """
         name = self.name
         if self.name_quoted:
             name = escape(name)
         value = self.val_deconv(self.value)
         value = self.mime_add(value)
-        return self.postprocess(f"{name}={value}")
+        line = NVLine(name, value, self.__class__)
+        line.deprocess()
+        return line
+
+    def to_str(self) -> str:
+        return self.to_line().to_str()
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{self.name}: {self.typeof} = {self.value}"
 
@@ -215,15 +241,15 @@
         return value
 
     @classmethod
     def val_deconv(cls, value: str) -> str:
         return value
 
 
-class REG_BINARY(PPLinelimit, Value):
+class REG_BINARY(LPLinelimit, Value):
     "Binary data in any form."
     value: bytes
     mime: str = "hex"
 
     @classmethod
     def val_conv(cls, value: str) -> bytes:
         vsplit = value.replace(",", "")
@@ -231,15 +257,15 @@
 
     @classmethod
     def val_deconv(cls, value: bytes) -> str:
         vsplit = wrap(value.hex(), 2)
         return ",".join(vsplit)
 
 
-class REG_EXPAND_SZ(PPLinelimit, Value):
+class REG_EXPAND_SZ(LPLinelimit, Value):
     """
     A null-terminated string that contains unexpanded references to environment
     variables, for example, %PATH%. It's either a Unicode or an ANSI string,
     depending on whether you use the Unicode or ANSI functions. To expand the
     environment variable references, use the
     [ExpandEnvironmentStrings](https://learn.microsoft.com/en-us/windows/win32/api/processenv/nf-processenv-expandenvironmentstringsa)
     function.
@@ -254,15 +280,15 @@
 
     @classmethod
     def val_deconv(cls, value: str) -> str:
         vbytes = bytes(value, encoding=REG_ENCODING)
         return REG_BINARY.val_deconv(vbytes)
 
 
-class REG_MULTI_SZ(PPLinelimit, Value):
+class REG_MULTI_SZ(LPLinelimit, Value):
     """
     A sequence of null-terminated strings, terminated by an empty string (\\0).
     The following is an example:
     String1\\0String2\\0String3\\0LastString\\0\\0.
     The first \\0 terminates the first string,
     the second-from-last \\0 terminates the last string,
     and the final \\0 terminates the sequence.
@@ -328,31 +354,28 @@
     REG_EXPAND_SZ,
     REG_MULTI_SZ,
     REG_BINARY,
     REG_SZ,
 ]
 
 
-def value_from_str(text: str) -> Value:
+def value_from_token(line: TValue) -> Value:
     """
     Returns a Value object from a string.
 
     Raises:
         TypeError: If the string value type could not be determined.
     """
-    name: str = text.split("=")[0]
-    value: str = text.split("=")[1]
     reg_type: Type[Value]
     for reg_type in mimemap:
-        if not reg_type.is_type_of(value):
+        if not reg_type.is_type_of(line.value):
             continue
-        res = reg_type.from_str(name, value)
-        assert res is not None  # NOTE: This is a hack
+        res = reg_type.from_token(line)
         return res
-    raise TypeError(f"Unknown type for line:\n{escape(text)}")
+    raise TypeError(f"Unknown type for line:\n{line}")
 
 
 @dataclass
 class Key:
     path: RegPath
     subkeys: list["Key"] = field(default_factory=list)
     values: list[Value] = field(default_factory=list)
@@ -361,33 +384,53 @@
     def name(self) -> str:
         return self.path[-1]
 
     @property
     def parent(self) -> Optional[RegPath]:
         return self.path.parent
 
+    @classmethod
+    def from_token(cls, token: TKey) -> "Key":
+        return cls(
+            RegPath.from_str(token.name),
+            values=[
+                value_from_token(vtok)
+                for vtok in token.values
+            ]
+        )
+
     def add_subkey(self, key: "Key"):
         self.subkeys.append(key)
 
     def __getitem__(self, name: str) -> "Key":
         for key in self.subkeys:
             if key.name == name:
                 return key
         raise KeyError(name)
 
     def add_value(self, value: Value):
         self.values.append(value)
 
-    def get_value(self, name: str) -> Optional[Value]:
+    def get_value(self, name: str) -> Value:
+        """
+        Returns a Value with the given name.
+
+        Raises:
+            KeyError: If the value could not be found.
+        """
         for value in self.values:
             if value.name == name:
                 return value
-        return None
+        raise KeyError(name)
 
-    def find_key(self, path: RegPath | Sequence[str] | str, skip_parent_check = False) -> "Key":
+    def find_key(
+        self,
+        path: RegPath | Sequence[str] | str,
+        skip_parent_check=False
+    ) -> "Key":
         if isinstance(path, RegPath):
             path = path.path
         if isinstance(path, str):
             path = path.split("\\")
         if not skip_parent_check and not RegPath(list(path)).startswith(self.path):
             pathstr = "\\".join(path)
             raise KeyError(f"{self.path} is not the parent of {pathstr}")
```

### Comparing `regfile-0.1.2/PKG-INFO` & `regfile-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regfile
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://gitlab.com/fnrir/regfile
 License: MPL-2.0
 Author: fnrir
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved
```

