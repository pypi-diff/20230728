# Comparing `tmp/sxpyr-0.0.3.tar.gz` & `tmp/sxpyr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sxpyr-0.0.3.tar", last modified: Fri Jun 24 01:24:52 2022, max compression
+gzip compressed data, was "sxpyr-0.0.4.tar", last modified: Thu Jul 27 23:26:58 2023, max compression
```

## Comparing `sxpyr-0.0.3.tar` & `sxpyr-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-06-24 01:24:52.711111 sxpyr-0.0.3/
--rw-r--r--   0 tom       (1000) tom       (1000)     1080 2022-05-01 01:55:47.000000 sxpyr-0.0.3/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     3790 2022-06-24 01:24:52.712111 sxpyr-0.0.3/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2671 2022-05-01 01:55:47.000000 sxpyr-0.0.3/README.org
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-06-24 01:24:52.709111 sxpyr-0.0.3/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)    22808 2022-05-01 01:55:47.000000 sxpyr-0.0.3/docs/chars.org
--rw-r--r--   0 tom       (1000) tom       (1000)    11500 2022-05-01 01:55:47.000000 sxpyr-0.0.3/docs/cross.org
--rw-r--r--   0 tom       (1000) tom       (1000)    65068 2022-05-01 01:55:47.000000 sxpyr-0.0.3/docs/paper.org
--rw-r--r--   0 tom       (1000) tom       (1000)    29592 2022-05-01 01:55:47.000000 sxpyr-0.0.3/docs/sexp.org
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2022-06-24 01:24:52.712111 sxpyr-0.0.3/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     2138 2022-06-24 01:24:50.000000 sxpyr-0.0.3/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-06-24 01:24:52.710111 sxpyr-0.0.3/sxpyr/
--rw-r--r--   0 tom       (1000) tom       (1000)       58 2022-05-02 23:29:11.000000 sxpyr-0.0.3/sxpyr/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      835 2022-05-01 01:55:47.000000 sxpyr-0.0.3/sxpyr/_exports.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5424 2022-05-01 01:55:47.000000 sxpyr-0.0.3/sxpyr/char.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3705 2022-06-08 07:14:58.000000 sxpyr-0.0.3/sxpyr/cli.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2870 2022-05-01 01:55:47.000000 sxpyr-0.0.3/sxpyr/introspect.py
--rw-r--r--   0 tom       (1000) tom       (1000)    72023 2022-06-08 07:14:58.000000 sxpyr-0.0.3/sxpyr/sxpyr.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17226 2022-05-01 01:55:47.000000 sxpyr-0.0.3/sxpyr/walks.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-06-24 01:24:52.711111 sxpyr-0.0.3/sxpyr.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     3790 2022-06-24 01:24:52.000000 sxpyr-0.0.3/sxpyr.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      543 2022-06-24 01:24:52.000000 sxpyr-0.0.3/sxpyr.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2022-06-24 01:24:52.000000 sxpyr-0.0.3/sxpyr.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       74 2022-06-24 01:24:52.000000 sxpyr-0.0.3/sxpyr.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        6 2022-06-24 01:24:52.000000 sxpyr-0.0.3/sxpyr.egg-info/top_level.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-06-24 01:24:52.711111 sxpyr-0.0.3/test/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-06-24 01:24:52.711111 sxpyr-0.0.3/test/data/
--rw-r--r--   0 tom       (1000) tom       (1000)      188 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/data/all.sxpr
--rw-r--r--   0 tom       (1000) tom       (1000)       12 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/data/even-smaller.sxpr
--rw-r--r--   0 tom       (1000) tom       (1000)      161 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/data/nested-splicing-unsyntax.rkt
--rw-r--r--   0 tom       (1000) tom       (1000)      192 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/data/plist-test.sxpr
--rw-r--r--   0 tom       (1000) tom       (1000)      116 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/data/small.sxpr
--rw-r--r--   0 tom       (1000) tom       (1000)       42 2022-05-01 01:55:47.000000 sxpyr-0.0.3/test/data/smaller.sxpr
--rw-r--r--   0 tom       (1000) tom       (1000)    38830 2022-06-24 01:24:50.000000 sxpyr-0.0.3/test/test_all.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-27 23:26:58.124370 sxpyr-0.0.4/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1080 2023-07-27 22:26:22.000000 sxpyr-0.0.4/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     3790 2023-07-27 23:26:58.124370 sxpyr-0.0.4/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2671 2023-07-27 22:26:22.000000 sxpyr-0.0.4/README.org
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-27 23:26:58.121370 sxpyr-0.0.4/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)    22808 2023-07-27 22:26:22.000000 sxpyr-0.0.4/docs/chars.org
+-rw-r--r--   0 tom       (1000) tom       (1000)    11500 2023-07-27 22:26:22.000000 sxpyr-0.0.4/docs/cross.org
+-rw-r--r--   0 tom       (1000) tom       (1000)    65068 2023-07-27 22:26:22.000000 sxpyr-0.0.4/docs/paper.org
+-rw-r--r--   0 tom       (1000) tom       (1000)    29592 2023-07-27 22:26:22.000000 sxpyr-0.0.4/docs/sexp.org
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2023-07-27 23:26:58.124370 sxpyr-0.0.4/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2133 2023-07-27 22:26:22.000000 sxpyr-0.0.4/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-27 23:26:58.122371 sxpyr-0.0.4/sxpyr/
+-rw-r--r--   0 tom       (1000) tom       (1000)       58 2023-07-27 22:26:22.000000 sxpyr-0.0.4/sxpyr/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      835 2023-07-27 22:26:22.000000 sxpyr-0.0.4/sxpyr/_exports.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5424 2023-07-27 22:26:22.000000 sxpyr-0.0.4/sxpyr/char.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3682 2023-07-27 22:26:22.000000 sxpyr-0.0.4/sxpyr/cli.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2870 2023-07-27 22:26:22.000000 sxpyr-0.0.4/sxpyr/introspect.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    72875 2023-07-27 22:28:47.000000 sxpyr-0.0.4/sxpyr/sxpyr.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17226 2023-07-27 22:26:22.000000 sxpyr-0.0.4/sxpyr/walks.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-27 23:26:58.123371 sxpyr-0.0.4/sxpyr.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3790 2023-07-27 23:26:57.000000 sxpyr-0.0.4/sxpyr.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      543 2023-07-27 23:26:57.000000 sxpyr-0.0.4/sxpyr.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-27 23:26:57.000000 sxpyr-0.0.4/sxpyr.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       59 2023-07-27 23:26:57.000000 sxpyr-0.0.4/sxpyr.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        6 2023-07-27 23:26:57.000000 sxpyr-0.0.4/sxpyr.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-27 23:26:58.123371 sxpyr-0.0.4/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-27 23:26:58.123371 sxpyr-0.0.4/test/data/
+-rw-r--r--   0 tom       (1000) tom       (1000)      188 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/data/all.sxpr
+-rw-r--r--   0 tom       (1000) tom       (1000)       12 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/data/even-smaller.sxpr
+-rw-r--r--   0 tom       (1000) tom       (1000)      161 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/data/nested-splicing-unsyntax.rkt
+-rw-r--r--   0 tom       (1000) tom       (1000)      192 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/data/plist-test.sxpr
+-rw-r--r--   0 tom       (1000) tom       (1000)      116 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/data/small.sxpr
+-rw-r--r--   0 tom       (1000) tom       (1000)       42 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/data/smaller.sxpr
+-rw-r--r--   0 tom       (1000) tom       (1000)    38830 2023-07-27 22:26:22.000000 sxpyr-0.0.4/test/test_all.py
```

### Comparing `sxpyr-0.0.3/LICENSE` & `sxpyr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/PKG-INFO` & `sxpyr-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sxpyr
-Version: 0.0.3
+Version: 0.0.4
 Summary: A flexible Lisp reader.
 Home-page: https://github.com/tgbugs/sxpyr
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: lisp reader edn clojure racket scheme elisp emacs sexp s-expression parser parsing
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sxpyr-0.0.3/README.org` & `sxpyr-0.0.4/README.org`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/docs/chars.org` & `sxpyr-0.0.4/docs/chars.org`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/docs/cross.org` & `sxpyr-0.0.4/docs/cross.org`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/docs/paper.org` & `sxpyr-0.0.4/docs/paper.org`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/docs/sexp.org` & `sxpyr-0.0.4/docs/sexp.org`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/setup.py` & `sxpyr-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 __version__ = find_version('sxpyr/sxpyr.py')
 
 with open('README.org', 'rt') as f:
     long_description = f.read()
 
-cli_requires = ['pyontutils']  # FIXME should be orthauth but haven't moved clifun yet
+cli_requires = ['clifn']  # FIXME should be orthauth but haven't moved clifun yet
 fuzz_requires = ['python-afl'] + cli_requires
 tests_require = ['pytest'] + cli_requires
                  
 setup(name='sxpyr',
       version=__version__,
       description='A flexible Lisp reader.',
       long_description=long_description,
```

### Comparing `sxpyr-0.0.3/sxpyr/_exports.py` & `sxpyr-0.0.4/sxpyr/_exports.py`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/sxpyr/char.py` & `sxpyr-0.0.4/sxpyr/char.py`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/sxpyr/cli.py` & `sxpyr-0.0.4/sxpyr/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Options:
     --fuzz
     -d --debug
 """
 
 import pathlib
-from pyontutils import clifun as clif
+import clifn
 from sxpyr import sxpyr as sxpyrmod
 from sxpyr._exports import *
 from sxpyr.walks import WalkRkt, WalkCl, WalkEl
 from sxpyr.sxpyr import (
     conf_read, Walk, conf_plist, WalkPl, plist_to_dict, PList, Ast,
     make_do_path,
     DispatchNotImplementedError)
@@ -39,26 +39,26 @@
     from select import select
     if stdin is None:
         from sys import stdin
     if select([stdin], [], [], 0.0)[0]:
         return stdin
 
 
-class Options(clif.Options):
+class Options(clifn.Options):
 
     @property
     def path(self):
         return [pathlib.Path(path).expanduser() for path in self._args['<path>']]
 
     #@property
     #def stdin(self):
         #return self._args['-']
 
 
-class Main(clif.Dispatcher):
+class Main(clifn.Dispatcher):
 
     def default(self):
         raise NotImplementedError('oops')
 
     def parse(self):
         # TODO guess dialect
         sxpyrmod.debug = self.options.debug  # FIXME sigh naming imports etc
```

### Comparing `sxpyr-0.0.3/sxpyr/introspect.py` & `sxpyr-0.0.4/sxpyr/introspect.py`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/sxpyr/sxpyr.py` & `sxpyr-0.0.4/sxpyr/sxpyr.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,70 +4,87 @@
 
 # TODO attach source char and line to the syntax objects
 # TODO issues with ambiguity of #word(list 1 2 3)
 # TODO feature expressions aka wraps next n, the impl must be
 # chainable and local because n must be defined, practically this ends
 # up being a wraps next that transitions the state to a wraps next
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 from io import TextIOWrapper
 from ast import literal_eval
 from json import dumps
 from types import GeneratorType
 
 debug = False
 
 
 class SxpyrError(Exception): pass
 class UnknownStateError(SxpyrError): pass
 class DispatchNotImplementedError(SxpyrError): pass
 
 
-def python_to_sxpr(blob):
+def python_to_sxpr(blob, str_as_string=False):
     # maybe json to sxpr to be safe? use the json normalization that we have?
     # blob to sxpr?
 
     # racket has jsexprs but that is peculiar to racket's syntax
     # and makes uses of verbatim atoms for keys so that it is possible
     # to have leading colons in keys etc. we can't do that with plists
     # and be able to use these in common lisp due to the ::symbol issue
     if isinstance(blob, dict):
-        return PList([e for k, v in blob.items() for e in [Keyword(k)._set_bounds(), python_to_sxpr(v)]])
-    elif isinstance(blob, list):
-        return List([python_to_sxpr(v) for v in blob])
+        return PList(
+            [e for k, v in blob.items()
+             for e in [Keyword(k)._set_bounds(),
+                       python_to_sxpr(v, str_as_string=str_as_string)]])
+    elif isinstance(blob, list) or isinstance(blob, tuple):
+        return List(
+            [python_to_sxpr(v, str_as_string=str_as_string)
+             for v in blob])
+    elif str_as_string and isinstance(blob, str):
+        return String(blob)
     elif blob is None:
         return List([])
     else:
         return blob
 
 
-def print_plist(ast_dt):
-    if isinstance(ast_dt, LLike):
-        if ast_dt.value:
-            #if Keyword in [type(v) for v in ast_dt.value]:
-                #return '(\n', ')\n'
-            #else:
-            return '(', ')\n'
-        else:
-            return '()'
-    elif isinstance(ast_dt, Keyword):
-        return '\n:'
-    elif isinstance(ast_dt, str):
-        bad = '()[]{} \n\t\'\"'
-        if [c for c in bad if c in ast_dt]:
+def configure_print_plist(newline_keyword=True):
+    def print_plist(ast_dt, last=False):
+        """print function for plists, returns begining or begining + end"""
+        if isinstance(ast_dt, LLike):
+            if ast_dt.value:
+                #if Keyword in [type(v) for v in ast_dt.value]:
+                    #return '(\n', ')\n'
+                #else:
+                return '(', (')' + ('' if last else '\n'))
+            else:
+                return '()'
+        elif isinstance(ast_dt, Keyword):
+            return '\n:' if newline_keyword else ':'
+        elif isinstance(ast_dt, String):
+            # explicit String always dumps
             return dumps(ast_dt)
+        elif isinstance(ast_dt, str):
+            bad = '()[]{} \n\t\'\"'
+            if [c for c in bad if c in ast_dt]:
+                return dumps(ast_dt)
+            else:
+                # make it a symbol
+                return ast_dt
+        elif isinstance(ast_dt, int):
+            return str(ast_dt)
         else:
-            # make it a symbol
-            return ast_dt
-    elif isinstance(ast_dt, int):
-        return str(ast_dt)
-    else:
-        breakpoint()
-        raise NotImplementedError(type(ast_dt))
+            breakpoint()
+            raise NotImplementedError(type(ast_dt))
+
+    return print_plist
+
+
+print_plist = configure_print_plist()
 
 
 def make_do_path(do, chunksize=4096):
     """ along the way to load """
     #parse = configure(**kwargs)  # FIXME pass in parse
     #read = conf_read(parse, mawp)  # FIXME
     def do_path(path_or_fd):
@@ -284,16 +301,16 @@
         self = cls(''.join(collect))
         self.collect = collect
         return self
 
     def __init__(self, value):
         self.value = value
 
-    def _print(self, pf):
-        beg = pf(self)
+    def _print(self, pf, last=False):
+        beg = pf(self, last=last)
         return beg + self.value
 
 
 class EKeyword(Keyword):
 
     __eq__ = _m.eq_collect
 
@@ -643,21 +660,22 @@
 
     def __repr__(self, depth=0, **kwargs):
         # already have a printer for this in protcur
         # FIXME recursion errors for deeply nested structures
         r = '\n'.join(repr(_) for _ in self.value)
         return self.o + r + self.c
 
-    def _print(self, pf):
-        beg, end = pf(self)
-        return beg + ' '.join([c._print(pf)
+    def _print(self, pf, last=False):
+        beg, end = pf(self, last=last)
+        lend = len(self.value) - 1
+        return beg + ' '.join([c._print(pf, last=(i == lend))
                                # FIXME sigh type inhomogenaity in the IR ...
                                if hasattr(c, '_print') else
-                               pf(c)
-                               for c in self.value]) + end
+                               pf(c, last=(i == len))
+                               for i, c in enumerate(self.value)]) + end
 
 
 class List(LLike):
     """ Usually a mutable singly linked list. """
 
     o, c = '()'
```

### Comparing `sxpyr-0.0.3/sxpyr/walks.py` & `sxpyr-0.0.4/sxpyr/walks.py`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/sxpyr.egg-info/PKG-INFO` & `sxpyr-0.0.4/sxpyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sxpyr
-Version: 0.0.3
+Version: 0.0.4
 Summary: A flexible Lisp reader.
 Home-page: https://github.com/tgbugs/sxpyr
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: lisp reader edn clojure racket scheme elisp emacs sexp s-expression parser parsing
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sxpyr-0.0.3/sxpyr.egg-info/SOURCES.txt` & `sxpyr-0.0.4/sxpyr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sxpyr-0.0.3/test/test_all.py` & `sxpyr-0.0.4/test/test_all.py`

 * *Files identical despite different names*

