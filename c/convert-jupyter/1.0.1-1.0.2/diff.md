# Comparing `tmp/convert_jupyter-1.0.1.tar.gz` & `tmp/convert_jupyter-1.0.2.tar.gz`

## Comparing `convert_jupyter-1.0.1.tar` & `convert_jupyter-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/.flake8
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/.pylintrc
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/Makefile
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/lint.sh
--rw-r--r--   0        0        0    46737 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/poetry.lock
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/upload.sh
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/__init__.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/__main__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/clean.py
--rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/code.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/constans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/test_clean.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/test_code.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/test_main.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/convert.py
--rw-r--r--   0        0        0    84335 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/test_jupyter.ipynb
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/test_jupyter_clean.ipynb
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/tmp.ipynb
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/tmp.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try.ipynb
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try3.ipynb
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try3.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/LICENSE.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/README.md
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/.flake8
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/.pylintrc
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/Makefile
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/lint.sh
+-rw-r--r--   0        0        0    46737 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/poetry.lock
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/upload.sh
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/__init__.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/__main__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/clean.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/code.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/constans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/test_clean.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/test_code.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/test_main.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/convert.py
+-rw-r--r--   0        0        0    84335 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/test_jupyter.ipynb
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/test_jupyter_clean.ipynb
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/tmp.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/tmp.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try3.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try3.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/README.md
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/PKG-INFO
```

### Comparing `convert_jupyter-1.0.1/.pylintrc` & `convert_jupyter-1.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/lint.sh` & `convert_jupyter-1.0.2/lint.sh`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/poetry.lock` & `convert_jupyter-1.0.2/poetry.lock`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/convert_jupyter/__main__.py` & `convert_jupyter-1.0.2/convert_jupyter/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         sys.argv[1:],
         "hVfo:i:c:",
         ["help", "version", "force", "=output", "=input", "=command"],
     )
 except getopt.GetoptError:
     print(short_help_info)
     sys.exit(2)
-print(opts, args)
 
 command, in_file = None, None
 
 for opt, arg in opts:
     if opt in ("-f", "--force"):
         force = True
     elif opt in ("-o", "--output"):
@@ -95,21 +94,25 @@
     elif opt in ("-h", "--help"):
         print(help_info)
         sys.exit(2)
     elif opt in ("-V", "--version"):
         print(get_project_version())
         sys.exit(2)
 
-if command is None:
-    if in_file is None:
-        in_file = args[1]
-    command = args[0]
-else:
-    if in_file is None:
-        in_file = args[0]
+try:
+    if command is None:
+        if in_file is None:
+            in_file = args[1]
+        command = args[0]
+    else:
+        if in_file is None:
+            in_file = args[0]
+except IndexError:
+    print(short_help_info)
+    sys.exit(2)
 
 
 command, in_file = args
 
 
 if out_file is None:
     out_file = ".".join([*in_file.split(".")[:-1], "ipynb"])
```

### Comparing `convert_jupyter-1.0.1/convert_jupyter/clean.py` & `convert_jupyter-1.0.2/convert_jupyter/clean.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/convert_jupyter/code.py` & `convert_jupyter-1.0.2/convert_jupyter/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from os.path import exists
 from typing import Any, Dict, Union
 
 from .constans import CELL_SEPARATOR, MARKDOWN_BEGIN, MARKDOWN_END
 
 
 def jupyter2py(
-    f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False
+    f_in_name: str,
+    f_out_name: Union[str, None] = None,
+    force: bool = False,
 ) -> None:
     """Function convert .ipynb to .py file.
 
     Function convert .ipynb to .py file.
     All cells after convert are separate to possible is revert convert.
     Markdown cells are commented.
 
@@ -48,15 +50,17 @@
                     sep="",
                     file=f_out,
                     end="",
                 )
 
 
 def py2jupyter(
-    f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False
+    f_in_name: str,
+    f_out_name: Union[str, None] = None,
+    force: bool = False,
 ) -> None:
     """Function convert .py to .ipynb file.
 
     Function convert .py to .ipynb file.
     Cells separator is {CELL_SEPARATOR}.
     Markdown cells starts by {MARKDOWN_BEGIN} end end by {MARKDOWN_END}
```

### Comparing `convert_jupyter-1.0.1/tests/test_clean.py` & `convert_jupyter-1.0.2/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/test_code.py` & `convert_jupyter-1.0.2/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/test_main.py` & `convert_jupyter-1.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/code/convert.py` & `convert_jupyter-1.0.2/tests/code/convert.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/code/test_jupyter.ipynb` & `convert_jupyter-1.0.2/tests/code/test_jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/code/test_jupyter_clean.ipynb` & `convert_jupyter-1.0.2/tests/code/test_jupyter_clean.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/code/tmp.ipynb` & `convert_jupyter-1.0.2/tests/code/tmp.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/code/try.ipynb` & `convert_jupyter-1.0.2/tests/code/try.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/tests/code/try3.ipynb` & `convert_jupyter-1.0.2/tests/code/try3.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/LICENSE.md` & `convert_jupyter-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.1/pyproject.toml` & `convert_jupyter-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert-jupyter"
-version = "1.0.1"
+version = "1.0.2"
 description = "Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
 
 authors = ["Bartłomiej Chwiłkowski <bartekchwilkowski@gmail.com>"]
 packages = [{include = "convert_jupyter"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -24,15 +24,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "convert-jupyter"
-version = "1.0.1"
+version = "1.0.2"
 authors = [    
   { name="Bartłomiej Chwiłkowski", email="bartekchwilkowski@gmail.com" },
   ]
 description = "Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `convert_jupyter-1.0.1/PKG-INFO` & `convert_jupyter-1.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-jupyter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts
 Project-URL: Homepage, https://github.com/chwilko/convert_jupyter
 Author-email: Bartłomiej Chwiłkowski <bartekchwilkowski@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -19,24 +19,53 @@
     - clean output jupyter
 
 
 ## autors
 Bartłomiej Chwiłkowski (github: chwilko)
 
 
+# Usage:
+python3 -m convert_jupyter [options] <command> <input_file>
+
+commands:
+  jupyter2py                Convert jupyter file to python file.
+  py2jupyter                Convert python file to jupyter file.
+  clean                     Clean set jupyter file outputs.
+  clean_all                 Clean all jupyter files outputs from the set folder and child folders
+
+input_file -- name of input file to convert or clean.
+
+General options:
+  -o, --output              Set the output file name. By default, it is the input file name with a valid extension.
+  -i, --input               Set input file directly.
+  -c, --command             Set command directly.
+  -f, --force               If file with output name exists overwrite them. By default raise error.
+  -h, --help                Show help and exit.
+  -V, --version             Show version and exit.
+
+
 # Structure
 convert_jupyter:
     - file with functions
 
+tests:
+    - tests
+
 
 ## Functions 
 
-jupyter2py(f_in_name: str, f_out_name: str = None)
+jupyter2py(
+    f_in_name: str,
+    f_out_name: Union[str, None] = None,
+    force: bool = False
+)
+    Convert jupyter file f_in_name to python file f_out_name.
 
 py2jupyter(f_in_name: str, f_out_name: str = None)
+    Convert python file f_in_name to jupyter file f_out_name.
 
 clean(path: str)
     Function clean jupyter file output.
 
 clean_all(path: str)
     The function recursively finds all jupyter files and clears their output.
```

