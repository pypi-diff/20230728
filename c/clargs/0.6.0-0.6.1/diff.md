# Comparing `tmp/clargs-0.6.0.tar.gz` & `tmp/clargs-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clargs-0.6.0.tar", last modified: Thu Jul 27 10:38:46 2023, max compression
+gzip compressed data, was "clargs-0.6.1.tar", last modified: Fri Jul 28 18:38:40 2023, max compression
```

## Comparing `clargs-0.6.0.tar` & `clargs-0.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.693434 clargs-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.693434 clargs-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 10:38:36.000000 clargs-0.6.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 10:38:36.000000 clargs-0.6.0/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 10:38:36.000000 clargs-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 10:38:36.000000 clargs-0.6.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 10:38:46.697434 clargs-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-07-27 10:38:36.000000 clargs-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/0_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/1_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/2_show_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/3_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/4_parse_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20370 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/5_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/__generate_example_output__.sh
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 10:38:36.000000 clargs-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:38:46.697434 clargs-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.693434 clargs-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/src/clargs/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/aap_from_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/clargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/helper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/src/clargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-27 10:38:36.000000 clargs-0.6.0/test/test_docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-07-27 10:38:36.000000 clargs-0.6.0/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-27 10:38:36.000000 clargs-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 18:38:31.000000 clargs-0.6.1/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 18:38:31.000000 clargs-0.6.1/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 18:38:31.000000 clargs-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 18:38:31.000000 clargs-0.6.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-28 18:38:40.791039 clargs-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-07-28 18:38:31.000000 clargs-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/1_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/2_show_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/3_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/4_parse_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20370 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/5_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/__generate_example_output__.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 18:38:31.000000 clargs-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:38:40.791039 clargs-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/src/clargs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/aap_from_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/clargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/helper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/src/clargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 18:38:31.000000 clargs-0.6.1/test/test_docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-07-28 18:38:31.000000 clargs-0.6.1/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-28 18:38:31.000000 clargs-0.6.1/tox.ini
```

### Comparing `clargs-0.6.0/.github/workflows/run-tests.yml` & `clargs-0.6.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/.github/workflows/upload.yml` & `clargs-0.6.1/.github/workflows/upload.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/LICENCE.txt` & `clargs-0.6.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/PKG-INFO` & `clargs-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.6.0
+Version: 0.6.1
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clargs-0.6.0/README.md` & `clargs-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/0_basic.py` & `clargs-0.6.1/examples/0_basic.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/1_flags.py` & `clargs-0.6.1/examples/1_flags.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/2_show_defaults.py` & `clargs-0.6.1/examples/2_show_defaults.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/3_list.py` & `clargs-0.6.1/examples/3_list.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/4_parse_groups.py` & `clargs-0.6.1/examples/4_parse_groups.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/5_logging.py` & `clargs-0.6.1/examples/5_logging.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/examples/__generate_example_output__.sh` & `clargs-0.6.1/examples/__generate_example_output__.sh`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/pyproject.toml` & `clargs-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/src/clargs/__init__.py` & `clargs-0.6.1/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/src/clargs/aap_from_data.py` & `clargs-0.6.1/src/clargs/aap_from_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,16 @@
                     "default": self.param.default,
                 }
             )
 
             if self.arg_type_is_flag() and not aap.action:
                 aap = aap.with_fields({"required": False})
             else:
-                aap = aap.with_fields({"nargs": "?"})
+                if aap.nargs == clargs.NOT_SET:
+                    aap = aap.with_fields({"nargs": "?"})
         else:
             if (
                 self.arg_type_is_flag()
                 and not aap.action
                 and aap.nargs not in ["*", "?"]
             ):
                 aap = aap.with_fields({"required": True})
```

### Comparing `clargs-0.6.0/src/clargs/clargs.py` & `clargs-0.6.1/src/clargs/clargs.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/src/clargs/docsparser.py` & `clargs-0.6.1/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/src/clargs/helper_types.py` & `clargs-0.6.1/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/src/clargs.egg-info/PKG-INFO` & `clargs-0.6.1/src/clargs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.6.0
+Version: 0.6.1
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clargs-0.6.0/src/clargs.egg-info/SOURCES.txt` & `clargs-0.6.1/src/clargs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/test/test_docsparser.py` & `clargs-0.6.1/test/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.0/test/test_simple.py` & `clargs-0.6.1/test/test_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,56 @@
 
         parser = clargs.create_parser(function)
         args = parser.parse_args(["1", "2"])
         self.assertEqual(vars(args), {"_clargs_func_": function, "numbers": [1, 2]})
         args = parser.parse_args([])
         self.assertEqual(vars(args), {"_clargs_func_": function, "numbers": []})
 
+    def test_list_int_flag(self):
+        def function(foo: str, *, numbers: list[int]):
+            pass
+
+        parser = clargs.create_parser(function)
+        args = parser.parse_args(["bar", "--numbers", "1", "2"])
+        self.assertEqual(
+            vars(args), {"_clargs_func_": function, "foo": "bar", "numbers": [1, 2]}
+        )
+        args = parser.parse_args(["bar", "--numbers"])
+        self.assertEqual(
+            vars(args), {"_clargs_func_": function, "foo": "bar", "numbers": []}
+        )
+        args = parser.parse_args(
+            ["bar", "--numbers", "1", "2", "--numbers", "3", "--numbers", "4", "5"]
+        )
+        self.assertEqual(
+            vars(args),
+            {"_clargs_func_": function, "foo": "bar", "numbers": [1, 2, 3, 4, 5]},
+        )
+
+    def test_list_int_flag_with_default(self):
+        def function(foo: str, *, numbers: list[int] = []):
+            pass
+
+        parser = clargs.create_parser(function)
+        args = parser.parse_args(["bar", "--numbers", "1", "2"])
+        self.assertEqual(
+            vars(args), {"_clargs_func_": function, "foo": "bar", "numbers": [1, 2]}
+        )
+        args = parser.parse_args(["bar", "--numbers"])
+        self.assertEqual(
+            vars(args), {"_clargs_func_": function, "foo": "bar", "numbers": []}
+        )
+        args = parser.parse_args(
+            ["bar", "--numbers", "1", "2", "--numbers", "3", "--numbers", "4", "5"]
+        )
+        self.assertEqual(
+            vars(args),
+            {"_clargs_func_": function, "foo": "bar", "numbers": [1, 2, 3, 4, 5]},
+        )
+
     def test_list_int_literal(self):
         def function(numbers: t.List[t.Literal[1, 2, 3, 5, 7, 11]]):
             pass
 
         parser = clargs.create_parser(function)
         args = parser.parse_args(["1", "2", "11"])
         self.assertEqual(vars(args), {"_clargs_func_": function, "numbers": [1, 2, 11]})
```

### Comparing `clargs-0.6.0/tox.ini` & `clargs-0.6.1/tox.ini`

 * *Files identical despite different names*

