# Comparing `tmp/datarails-0.0.2.tar.gz` & `tmp/datarails-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.0.2.tar", last modified: Tue Jul 25 04:16:02 2023, max compression
+gzip compressed data, was "datarails-0.2.0.tar", last modified: Fri Jul 28 12:38:36 2023, max compression
```

## Comparing `datarails-0.0.2.tar` & `datarails-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.009071 datarails-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 04:16:02.009071 datarails-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 04:15:54.000000 datarails-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.005071 datarails-0.0.2/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 04:15:54.000000 datarails-0.0.2/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/databox.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.005071 datarails-0.0.2/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-25 04:16:02.000000 datarails-0.0.2/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 04:15:54.000000 datarails-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 04:16:02.009071 datarails-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-25 04:15:13.000000 datarails-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.005071 datarails-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-25 04:15:13.000000 datarails-0.0.2/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-25 04:15:13.000000 datarails-0.0.2/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-25 04:15:13.000000 datarails-0.0.2/tests/test_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.001070 datarails-0.0.2/venv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.009071 datarails-0.0.2/venv/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      639 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      838 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2man.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      827 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:38:36.865119 datarails-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 12:38:36.861119 datarails-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 12:38:17.000000 datarails-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:38:36.861119 datarails-0.2.0/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 12:38:17.000000 datarails-0.2.0/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 12:38:17.000000 datarails-0.2.0/datarails/databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 12:38:17.000000 datarails-0.2.0/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-28 12:38:17.000000 datarails-0.2.0/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 12:38:17.000000 datarails-0.2.0/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:38:36.861119 datarails-0.2.0/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 12:38:36.000000 datarails-0.2.0/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-28 12:38:36.000000 datarails-0.2.0/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:38:36.000000 datarails-0.2.0/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 12:38:36.000000 datarails-0.2.0/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 12:38:36.000000 datarails-0.2.0/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 12:38:17.000000 datarails-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:38:36.865119 datarails-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 12:38:17.000000 datarails-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:38:36.861119 datarails-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 12:38:17.000000 datarails-0.2.0/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-28 12:38:17.000000 datarails-0.2.0/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 12:38:17.000000 datarails-0.2.0/tests/test_step.py
```

### Comparing `datarails-0.0.2/datarails/databox.py` & `datarails-0.2.0/datarails/databox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+from typing import List
+
 from datarails.type_vars import DataFrame
 
 
 class DataBox:
     def __init__(self, **kwargs) -> None:
         for k, v in kwargs.items():
             setattr(self, k, v)
 
+    def __str__(self) -> str:
+        return f"DataBox({self.list_contents()})"
+
     def get_df(self, name: str) -> DataFrame:
         return getattr(self, name)
 
     def add_df(self, name: str, df: DataFrame) -> None:
         setattr(self, name, df)
 
     def pop_df(self, name: str) -> DataFrame:
         df = self.get_df(name)
         delattr(self, name)
         return df
 
     def delete_df(self, name: str) -> None:
         delattr(self, name)
+
+    def list_contents(self) -> List[str]:
+        return [k for k in vars(self).keys()]
```

### Comparing `datarails-0.0.2/datarails/runner.py` & `datarails-0.2.0/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.2/datarails/step.py` & `datarails-0.2.0/datarails/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     ) -> None:
         self.dbx = dbx
         self.step_method_name_generator = None
         self.on_entry_callback = on_entry_callback
         self.on_exit_callback = on_exit_callback
         self.reset()
 
+    def __str__(self) -> str:
+        return self.__class__.__name__
+
     def reset(self) -> None:
         self.step_method_name_generator = iter(self.step_methods)
 
     def run_steps(self) -> DataBox:
         if self.on_entry_callback:
             self.on_entry_callback()
```

### Comparing `datarails-0.0.2/pyproject.toml` & `datarails-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.0.2"
+version = "0.2.0"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.0.2/tests/test_databox.py` & `datarails-0.2.0/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.2/tests/test_runner.py` & `datarails-0.2.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.2/tests/test_step.py` & `datarails-0.2.0/tests/test_step.py`

 * *Files identical despite different names*

