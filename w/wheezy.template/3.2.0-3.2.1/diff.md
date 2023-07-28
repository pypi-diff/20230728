# Comparing `tmp/wheezy.template-3.2.0.tar.gz` & `tmp/wheezy.template-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.template-3.2.0.tar", last modified: Fri Jul 28 08:28:53 2023, max compression
+gzip compressed data, was "wheezy.template-3.2.1.tar", last modified: Fri Jul 28 14:10:58 2023, max compression
```

## Comparing `wheezy.template-3.2.0.tar` & `wheezy.template-3.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/wheezy/template/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 08:28:51.000000 wheezy.template-3.2.0/src/wheezy/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/comp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/src/wheezy/template/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/determined.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/wheezy.template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:58.227749 wheezy.template-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 14:10:58.227749 wheezy.template-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:10:58.227749 wheezy.template-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:58.223749 wheezy.template-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:58.223749 wheezy.template-3.2.1/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:58.227749 wheezy.template-3.2.1/src/wheezy/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 14:10:56.000000 wheezy.template-3.2.1/src/wheezy/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:58.227749 wheezy.template-3.2.1/src/wheezy/template/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/ext/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/ext/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/ext/determined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-28 14:10:43.000000 wheezy.template-3.2.1/src/wheezy/template/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:10:58.223749 wheezy.template-3.2.1/src/wheezy.template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 14:10:58.000000 wheezy.template-3.2.1/src/wheezy.template.egg-info/top_level.txt
```

### Comparing `wheezy.template-3.2.0/LICENSE` & `wheezy.template-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/PKG-INFO` & `wheezy.template-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheezy.template
-Version: 3.2.0
+Version: 3.2.1
 Summary: A lightweight template library
 Home-page: https://github.com/akornatskyy/wheezy.template
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
 Keywords: html markup template preprocessor
 Platform: any
```

### Comparing `wheezy.template-3.2.0/README.md` & `wheezy.template-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/setup.py` & `wheezy.template-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/builder.py` & `wheezy.template-3.2.1/src/wheezy/template/builder.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/compiler.py` & `wheezy.template-3.2.1/src/wheezy/template/compiler.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/console.py` & `wheezy.template-3.2.1/src/wheezy/template/console.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/engine.py` & `wheezy.template-3.2.1/src/wheezy/template/engine.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/ext/code.py` & `wheezy.template-3.2.1/src/wheezy/template/ext/code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import typing
 
+from wheezy.template.comp import Tuple
 from wheezy.template.typing import Builder, LexerRule, ParserRule, Token
 from wheezy.template.utils import find_balanced
 
 # region: lexer extensions
 
 
 def code_token(m: typing.Match[str]) -> Token:
@@ -50,10 +51,8 @@
     def __init__(self, token_start: str = "@") -> None:
         self.lexer_rules: typing.Mapping[int, LexerRule] = {
             300: (re.compile(r"\s*%s(?=\()" % token_start), code_token),
         }
 
     parser_rules: typing.Mapping[str, ParserRule] = {"code": parse_code}
 
-    builder_rules: typing.List[typing.Tuple[str, typing.Any]] = [
-        ("code", build_code)
-    ]
+    builder_rules: typing.List[Tuple[str, typing.Any]] = [("code", build_code)]
```

### Comparing `wheezy.template-3.2.0/src/wheezy/template/ext/core.py` & `wheezy.template-3.2.1/src/wheezy/template/ext/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import typing
 
+from wheezy.template.comp import Tuple
 from wheezy.template.typing import Builder, LexerRule, ParserConfig, Token
 from wheezy.template.utils import find_all_balanced
 
 # region: config
 
 end_tokens = ["end"]
 continue_tokens = ["else:", "elif "]
@@ -79,32 +80,32 @@
     return value.rstrip()[8:-1]
 
 
 def parse_include(value: str) -> str:
     return value.rstrip()[8:-1]
 
 
-def parse_import(value: str) -> typing.Tuple[str, str]:
+def parse_import(value: str) -> Tuple[str, str]:
     name, var = value[7:].rsplit(" as ", 1)
     return name, var
 
 
-def parse_from(value: str) -> typing.Tuple[str, str, str]:
+def parse_from(value: str) -> Tuple[str, str, str]:
     name, var = value[5:].rsplit(" import ", 1)
     s = var.rsplit(" as ", 1)
     if len(s) == 2:
         var, alias = s
     else:
         alias = var
     return name, var, alias
 
 
 def parse_var(
     value: str,
-) -> typing.Tuple[str, typing.Optional[typing.List[str]]]:
+) -> Tuple[str, typing.Optional[typing.List[str]]]:
     if "!!" not in value:
         return value, None
     var, var_filter = value.rsplit("!!", 1)
     return var, var_filter.strip().split("!")
 
 
 # region: block_builders
@@ -140,27 +141,27 @@
     for lineno, token, value in nodes:
         if token == "def ":
             builder.build_token(lineno, token, value)
     return True
 
 
 def build_import(
-    builder: Builder, lineno: int, token: str, value: typing.Tuple[str, str]
+    builder: Builder, lineno: int, token: str, value: Tuple[str, str]
 ) -> bool:
     assert token == "import "
     name, var = value
     builder.add(lineno, var + " = _i(" + name + ")")
     return True
 
 
 def build_from(
     builder: Builder,
     lineno: int,
     token: str,
-    value: typing.Tuple[str, str, str],
+    value: Tuple[str, str, str],
 ) -> bool:
     assert token == "from "
     name, var, alias = value
     builder.add(
         lineno, alias + " = _i(" + name + ").local_defs['" + var + "']"
     )
     return True
```

### Comparing `wheezy.template-3.2.0/src/wheezy/template/ext/determined.py` & `wheezy.template-3.2.1/src/wheezy/template/ext/determined.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import typing
 
+from wheezy.template.comp import Tuple
 from wheezy.template.utils import find_balanced
 
 RE_ARGS = re.compile(r'\s*(?P<expr>(([\'"]).*?\3|.+?))\s*\,')
 RE_KWARGS = re.compile(
     r'\s*(?P<name>\w+)\s*=\s*(?P<expr>([\'"].*?[\'"]|.+?))\s*\,'
 )
 RE_STR_VALUE = re.compile(r'^[\'"](?P<value>.+)[\'"]$')
@@ -113,15 +114,15 @@
     for m in RE_ARGS.finditer(text + ","):
         args.append(m.group("expr"))
     return args
 
 
 def parse_params(
     text: str,
-) -> typing.Tuple[typing.List[str], typing.Mapping[str, str]]:
+) -> Tuple[typing.List[str], typing.Mapping[str, str]]:
     """Parses function parameters.
 
     >>> parse_params('')
     ([], {})
     >>> parse_params('id=item.id')
     ([], {'id': 'item.id'})
     >>> parse_params('"default"')
```

### Comparing `wheezy.template-3.2.0/src/wheezy/template/lexer.py` & `wheezy.template-3.2.1/src/wheezy/template/lexer.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/loader.py` & `wheezy.template-3.2.1/src/wheezy/template/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import os.path
 import stat
 import time
 import typing
 
+from wheezy.template.comp import Tuple
 from wheezy.template.engine import Engine
 from wheezy.template.typing import Loader, SupportsRender
 
 
 class FileLoader(Loader):
     """Loads templates from file system.
 
@@ -23,15 +24,15 @@
             abspath = os.path.abspath(path)
             assert os.path.exists(abspath)
             assert os.path.isdir(abspath)
             searchpath.append(abspath)
         self.searchpath = searchpath
         self.encoding = encoding
 
-    def list_names(self) -> typing.Tuple[str, ...]:
+    def list_names(self) -> Tuple[str, ...]:
         """Return a list of names relative to directories. Ignores any files
         and directories that start with dot.
         """
         names = []
         for path in self.searchpath:
             pathlen = len(path) + 1
             for dirpath, dirnames, filenames in os.walk(path):
@@ -79,15 +80,15 @@
     ``templates`` - a dict where key corresponds to template name and
     value to template content.
     """
 
     def __init__(self, templates: typing.Mapping[str, str]) -> None:
         self.templates = templates
 
-    def list_names(self) -> typing.Tuple[str, ...]:
+    def list_names(self) -> Tuple[str, ...]:
         """List all keys from internal dict."""
         return tuple(sorted(self.templates.keys()))
 
     def load(self, name: str) -> typing.Optional[str]:
         """Returns template by name."""
         if name not in self.templates:
             return None
@@ -96,15 +97,15 @@
 
 class ChainLoader(Loader):
     """Loads templates from ``loaders`` until first succeed."""
 
     def __init__(self, loaders: typing.List[Loader]) -> None:
         self.loaders = loaders
 
-    def list_names(self) -> typing.Tuple[str, ...]:
+    def list_names(self) -> Tuple[str, ...]:
         """Returns as list of names from all loaders."""
         names = set()
         for loader in self.loaders:
             names |= set(loader.list_names())
         return tuple(sorted(names))
 
     def load(self, name: str) -> typing.Optional[str]:
@@ -123,15 +124,15 @@
         self,
         engine: Engine,
         ctx: typing.Optional[typing.Mapping[str, typing.Any]] = None,
     ) -> None:
         self.engine = engine
         self.ctx = ctx or {}
 
-    def list_names(self) -> typing.Tuple[str, ...]:
+    def list_names(self) -> Tuple[str, ...]:
         return self.engine.loader.list_names()
 
     def load(self, name: str) -> str:
         return self.engine.render(name, self.ctx, {}, {})
 
 
 def autoreload(engine: Engine, enabled: bool = True) -> Engine:
```

### Comparing `wheezy.template-3.2.0/src/wheezy/template/parser.py` & `wheezy.template-3.2.1/src/wheezy/template/parser.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/preprocessor.py` & `wheezy.template-3.2.1/src/wheezy/template/preprocessor.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy/template/typing.py` & `wheezy.template-3.2.1/src/wheezy/template/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import sys
 import typing
 from abc import abstractmethod
 
-if sys.version_info <= (3, 9, 0):  # pragma: nocover
-    Token = typing.Tuple[int, str, str]
-else:  # pragma: nocover
-    Token = tuple[int, str, str]  # type: ignore[misc]
+from wheezy.template.comp import List, Tuple
+
+Token = Tuple[int, str, str]
 
 
 class Builder:
     lineno: int
 
     @abstractmethod
     def start_block(self) -> None:
@@ -34,34 +32,34 @@
         token: str,
         value: typing.Union[str, typing.Iterable[Token]],
     ) -> None:
         ...  # pragma: nocover
 
 
 Tokenizer = typing.Callable[[typing.Match], Token]
-LexerRule = typing.Tuple[typing.Pattern, Tokenizer]
+LexerRule = Tuple[typing.Pattern, Tokenizer]
 PreProcessorRule = typing.Callable[[str], str]
-PostProcessorRule = typing.Callable[[typing.List[Token]], str]
+PostProcessorRule = typing.Callable[[List[Token]], str]
 BuilderRule = typing.Callable[
     [
         Builder,
         int,
         str,
-        typing.Union[str, typing.List[str], typing.Iterable[Token]],
+        typing.Union[str, List[str], typing.Iterable[Token]],
     ],
     bool,
 ]
-ParserRule = typing.Callable[[str], typing.Union[str, typing.List[str]]]
+ParserRule = typing.Callable[[str], typing.Union[str, List[str]]]
 
 
 class ParserConfig:
-    end_tokens: typing.List[str]
-    continue_tokens: typing.List[str]
-    compound_tokens: typing.List[str]
-    out_tokens: typing.List[str]
+    end_tokens: List[str]
+    continue_tokens: List[str]
+    compound_tokens: List[str]
+    out_tokens: List[str]
 
 
 RenderTemplate = typing.Callable[
     [
         typing.Mapping[str, typing.Any],
         typing.Mapping[str, typing.Any],
         typing.Mapping[str, typing.Any],
@@ -77,13 +75,13 @@
 
 
 TemplateClass = typing.Callable[[str, RenderTemplate], SupportsRender]
 
 
 class Loader:
     @abstractmethod
-    def list_names(self) -> typing.Tuple[str, ...]:
+    def list_names(self) -> Tuple[str, ...]:
         ...  # pragma: nocover
 
     @abstractmethod
     def load(self, name: str) -> typing.Optional[str]:
         ...  # pragma: nocover
```

### Comparing `wheezy.template-3.2.0/src/wheezy/template/utils.py` & `wheezy.template-3.2.1/src/wheezy/template/utils.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.2.0/src/wheezy.template.egg-info/PKG-INFO` & `wheezy.template-3.2.1/src/wheezy.template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheezy.template
-Version: 3.2.0
+Version: 3.2.1
 Summary: A lightweight template library
 Home-page: https://github.com/akornatskyy/wheezy.template
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
 Keywords: html markup template preprocessor
 Platform: any
```

### Comparing `wheezy.template-3.2.0/src/wheezy.template.egg-info/SOURCES.txt` & `wheezy.template-3.2.1/src/wheezy.template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

