# Comparing `tmp/atro_args-0.2.2.tar.gz` & `tmp/atro_args-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_args-0.2.2.tar", max compression
+gzip compressed data, was "atro_args-0.2.3.tar", max compression
```

## Comparing `atro_args-0.2.2.tar` & `atro_args-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      963 2023-07-28 15:55:58.438531 atro_args-0.2.2/README.md
--rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/arg.py
--rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/arg_source.py
--rw-r--r--   0        0        0     1254 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/helpers.py
--rw-r--r--   0        0        0     8192 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/input_args.py
--rw-r--r--   0        0        0      407 2023-07-28 18:14:24.886698 atro_args-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 atro_args-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      963 2023-07-28 19:02:59.510131 atro_args-0.2.3/README.md
+-rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.3/atro_args/__init__.py
+-rw-r--r--   0        0        0     1699 2023-07-28 19:48:36.731517 atro_args-0.2.3/atro_args/arg.py
+-rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.3/atro_args/arg_source.py
+-rw-r--r--   0        0        0     1327 2023-07-28 19:46:54.751810 atro_args-0.2.3/atro_args/helpers.py
+-rw-r--r--   0        0        0     8472 2023-07-28 19:56:18.655100 atro_args-0.2.3/atro_args/input_args.py
+-rw-r--r--   0        0        0      411 2023-07-28 19:56:26.498381 atro_args-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 atro_args-0.2.3/PKG-INFO
```

### Comparing `atro_args-0.2.2/README.md` & `atro_args-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `atro_args-0.2.2/atro_args/arg.py` & `atro_args-0.2.3/atro_args/arg.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         accept_via_env_file (bool, optional): Whether the argument can be passed via ENV file. Defaults to True.
         accept_via_yaml_file (bool, optional): Whether the argument can be passed via Yaml file. Defaults to True.
         default (Any, optional): The default value of the argument. If set to None it is assumed there is no default (will fail on required=True). Defaults to None.
     """
 
     name: str
     other_names: str | list[str] = []
-    arg_type: type
-    help: str
+    arg_type: type = str
+    help: str = ""
     required: bool = True
     accept_via_env: bool = True
     accept_via_cli: bool = True
     accept_via_env_file: bool = True
     accept_via_yaml_file: bool = True
     default: Any = None
```

### Comparing `atro_args-0.2.2/atro_args/helpers.py` & `atro_args-0.2.3/atro_args/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import ast
 import json
 import logging
+from typing import Mapping, Sequence
 
 
-def load_as_py_type_from_string(s, arg_type):
-    logging.debug(f"If {s} is str return right away.")
-    if arg_type == str:
+def load_to_py_type(s, arg_type):
+    # If type is correct return as is
+    if type(s) == arg_type:
+        logging.debug(f"{s} is already of type {arg_type} no need to parse.")
         return s
 
-    logging.debug(f"If {s} is of simple type (int, float or bool), cast directly and return.")
-    if arg_type in [int, float, bool]:
-        try:
-            return arg_type(s)
-        except ValueError:
-            raise TypeError(f"Could not load {s} as {arg_type}.")
 
-    try:
-        logging.debug(f"Trying to load {s} as json.")
-        json_loaded = json.loads(s)
-        if isinstance(json_loaded, arg_type):
-            logging.debug(f"Loaded {s} as json, checking if type is {arg_type} if so returning.")
-            return json_loaded
-    except json.JSONDecodeError:
+    if arg_type in [Mapping, Sequence, list, dict]:
+        if not isinstance(s, str):
+            raise ValueError(f"Could not load {s} as {arg_type} because it is not clear how to load type {type(s)} into {arg_type}.")
+        
         try:
-            logging.debug(f"Trying to load {s} as ast, as json.loads failed.")
-            ast_loaded = ast.literal_eval(s)
-            if isinstance(ast_loaded, arg_type):
-                logging.debug(f"Loaded {s} using ast, checking if type is {arg_type} if so returning.")
-                return ast_loaded
-        except (ValueError, SyntaxError):
-            raise ValueError(f"Could not load {s} as {arg_type}.")
+            logging.debug(f"Trying to load {s} as json.")
+            json_loaded = json.loads(s)
+            if isinstance(json_loaded, arg_type):
+                logging.debug(f"Loaded {s} as json, checking if type is {arg_type} if so returning.")
+                return json_loaded
+        except json.JSONDecodeError:
+            try:
+                logging.debug(f"Trying to load {s} as ast, as json.loads failed.")
+                ast_loaded = ast.literal_eval(s)
+                if isinstance(ast_loaded, arg_type):
+                    logging.debug(f"Loaded {s} using ast, checking if type is {arg_type} if so returning.")
+                    return ast_loaded
+            except (ValueError, SyntaxError):
+                raise ValueError(f"Could not load {s} as {arg_type}.")
 
-    raise TypeError(f"Could not load {s} as {arg_type}.")
+    return arg_type(s)
```

### Comparing `atro_args-0.2.2/atro_args/input_args.py` & `atro_args-0.2.3/atro_args/input_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 from argparse import ArgumentParser
 from collections.abc import Sequence
 from os import environ
 from pathlib import Path
-from typing import Any
+from typing import Any, Mapping
 
 import yaml
 from annotated_types import UpperCase
 from dotenv import load_dotenv
 from pydantic import BaseModel, field_validator
 
 from atro_args.arg import Arg
 from atro_args.arg_source import ArgSource
-from atro_args.helpers import load_as_py_type_from_string
+from atro_args.helpers import load_to_py_type
 
 
 class InputArgs(BaseModel):
     """InputArgs is a model that represents the input arguments of an application. After it is initialized the parse_args method can be called to parse the arguments and return them as a dictionary.
 
     Attributes:
         prefix (UpperCase): The prefix to use for environment variables. Defaults to "ATRO_ARGS". This means that the environment variable for the argument "name" will be "ATRO_ARGS_NAME" and the environment variable for the argument "other_names" will be "ATRO_ARGS_OTHER_NAMES".
@@ -41,15 +41,22 @@
     def add_arg(self, arg: Arg):
         self.args.append(arg)
 
     def get_cli_args(self, cli_input_args: Sequence[str] | None) -> dict[str, str]:
         parser = ArgumentParser()
         for arg in self.args:
             if arg.accept_via_cli:
-                parser.add_argument(f"--{arg.name}", *arg.other_names, type=str, help=arg.help, required=False)
+                # Making some adjustments
+                other_names = [f"-" + name for name in arg.other_names]
+                arg_type = arg.arg_type
+                if arg_type in [Sequence, Mapping, list, dict]:
+                    # loading a json as dict or list will fail in argparse, as it will load each element char by char, bypassing that issue by loading it as a string and then converting it to the desired type
+                    arg_type = str
+                
+                parser.add_argument(f"--{arg.name}", *other_names, type=arg_type, help=arg.help, required=False)
 
         return vars(parser.parse_args(cli_input_args or []))
 
     def get_env_args(self) -> dict[str, str]:
         envs: dict[str, str] = {}
         for arg in self.args:
             env = environ.get(f"{self.prefix}_{arg.name}".upper())
@@ -111,19 +118,15 @@
                 (arg,) = (arg for arg in self.args if arg.name == key)
 
                 if self.is_arg_source_accepted(arg, arg_source) is False:
                     logging.debug(f"'{key}' is not accepted via '{arg_source.value}', skipping.")
                     continue
 
                 logging.info(f"Setting '{key}' to be of value '{value}' from '{arg_source.value}'")
-                if type(value) == arg.arg_type:
-                    model[key] = value
-                else:
-                    logging.debug("Parsing {value} as {arg.arg_type}.")
-                    model[key] = load_as_py_type_from_string(value, arg.arg_type)
+                model[key] = load_to_py_type(value, arg.arg_type)
 
             else:
                 logging.debug(f"'{key}' has already been set.")
 
     def populated_model(self, model: dict[str, Any], cli_args: dict[str, str], env_args: dict[str, str], env_file_args: dict[str, str], yaml_file_args: dict[str, str]) -> dict[str, Any]:
         for arg_type in self.arg_priority:
             match arg_type:
```

### Comparing `atro_args-0.2.2/PKG-INFO` & `atro_args-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: atro-args
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: atropos
 Author-email: sv7n@pm.me
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 # Atro-Args
```

