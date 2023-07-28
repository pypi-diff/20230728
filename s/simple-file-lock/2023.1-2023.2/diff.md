# Comparing `tmp/simple_file_lock-2023.1.tar.gz` & `tmp/simple_file_lock-2023.2.tar.gz`

## Comparing `simple_file_lock-2023.1.tar` & `simple_file_lock-2023.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/requirements.txt
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/source/conf.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/source/index.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/source/modules.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/source/readme.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/doc/source/simple_file_lock.rst
--rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/scripts/build_documentation.sh
--rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/scripts/test.sh
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/src/simple_file_lock/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/src/simple_file_lock/version.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/test/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/LICENSE.txt
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/pyproject.toml
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 simple_file_lock-2023.1/PKG-INFO
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/requirements.txt
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/source/conf.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/source/index.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/source/modules.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/source/readme.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/doc/source/simple_file_lock.rst
+-rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/scripts/build_documentation.sh
+-rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/scripts/test.sh
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/src/simple_file_lock/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/src/simple_file_lock/version.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/test/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/LICENSE.txt
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/pyproject.toml
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 simple_file_lock-2023.2/PKG-INFO
```

### Comparing `simple_file_lock-2023.1/doc/Makefile` & `simple_file_lock-2023.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/doc/make.bat` & `simple_file_lock-2023.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/doc/source/conf.py` & `simple_file_lock-2023.2/doc/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # pylint: disable=invalid-name,redefined-builtin
 
 import importlib
 import pathlib
 import sys
 
 source_code = '../../src'
-git_url = 'https://gitlab.inria.fr/jrye/simple-file_lock'
+git_url = 'https://gitlab.inria.fr/jrye/simple-file-lock'
 
 this_path = pathlib.Path(__file__).resolve()
 sys.path.insert(0, str((this_path.parent / source_code).resolve()))
 
 author = 'Jan-Michael Rye'
 copyright = '2023, Inria'
 project = 'Simple File Lock'
@@ -26,17 +26,19 @@
 extensions = [
     'myst_parser',
     'sphinx.ext.autodoc',
     'sphinx.ext.linkcode',
     'sphinx.ext.napoleon',
     'sphinx.ext.todo'
 ]
+index_entries = [
+]
 
 
-def skip(app, what, name, obj, would_skip, options):
+def skip(_app, _what, name, _obj, would_skip, _options):  # pylint: disable=too-many-arguments
     '''Customize autodoc member skipping.'''
     if name == '__init__':
         return False
     return would_skip
 
 
 def setup(app):
```

### Comparing `simple_file_lock-2023.1/scripts/build_documentation.sh` & `simple_file_lock-2023.2/scripts/build_documentation.sh`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/src/simple_file_lock/__init__.py` & `simple_file_lock-2023.2/src/simple_file_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/test/test.py` & `simple_file_lock-2023.2/test/test.py`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/LICENSE.txt` & `simple_file_lock-2023.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/README.md` & `simple_file_lock-2023.2/README.md`

 * *Files identical despite different names*

### Comparing `simple_file_lock-2023.1/pyproject.toml` & `simple_file_lock-2023.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ['hatchling', 'hatch-vcs', 'wheel']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'simple_file_lock'
 description = 'Context manager for simple file locking.'
-license = 'MIT'
+license = {file = 'LICENSE.txt'}
 dependencies = [
   'psutil'
 ]
 authors = [
   {name = 'Jan-Michael Rye', email = 'jan-michael.rye@inria.fr' }
 ]
 requires-python = '>=3.7'
```

### Comparing `simple_file_lock-2023.1/PKG-INFO` & `simple_file_lock-2023.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Metadata-Version: 2.1
 Name: simple_file_lock
-Version: 2023.1
+Version: 2023.2
 Summary: Context manager for simple file locking.
 Project-URL: Source, https://gitlab.inria.fr/jrye/simple-file-lock
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/simple-file-lock/
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
-License-Expression: MIT
+License: MIT License
+        
+        Copyright (c) 2023, Inria
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: psutil
 Description-Content-Type: text/markdown
```

