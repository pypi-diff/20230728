# Comparing `tmp/mlflow_extra-2023.3.tar.gz` & `tmp/mlflow_extra-2023.4.tar.gz`

## Comparing `mlflow_extra-2023.3.tar` & `mlflow_extra-2023.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/requirements.txt
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/source/conf.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/source/index.rst
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/source/mlflow_extra.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/source/modules.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/doc/source/readme.md
--rwxr-xr-x   0        0        0      777 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/scripts/install.sh
--rwxr-xr-x   0        0        0      740 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/scripts/install_and_run.sh
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/common.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/filter.py
--rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/merge.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/metadata.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/uri.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/src/mlflow_extra/version.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/LICENSE.txt
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/README.md
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/pyproject.toml
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 mlflow_extra-2023.3/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/requirements.txt
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/source/conf.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/source/index.rst
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/source/mlflow_extra.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/source/modules.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/doc/source/readme.md
+-rwxr-xr-x   0        0        0      777 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/scripts/install.sh
+-rwxr-xr-x   0        0        0      740 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/scripts/install_and_run.sh
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/common.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/filter.py
+-rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/merge.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/metadata.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/uri.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/src/mlflow_extra/version.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/LICENSE.txt
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/README.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/pyproject.toml
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mlflow_extra-2023.4/PKG-INFO
```

### Comparing `mlflow_extra-2023.3/doc/Makefile` & `mlflow_extra-2023.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/doc/make.bat` & `mlflow_extra-2023.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/doc/source/conf.py` & `mlflow_extra-2023.4/doc/source/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,14 +28,28 @@
 extensions = [
     'myst_parser',
     'sphinx.ext.autodoc',
     'sphinx.ext.linkcode',
     'sphinx.ext.napoleon',
     'sphinx.ext.todo'
 ]
+index_entries = [
+]
+
+
+def skip(_app, _what, name, _obj, would_skip, _options):  # pylint: disable=too-many-arguments
+    '''Customize autodoc member skipping.'''
+    if name == '__init__':
+        return False
+    return would_skip
+
+
+def setup(app):
+    '''Connect the skip function.'''
+    app.connect('autodoc-skip-member', skip)
 
 
 def linkcode_resolve(domain, info):
     '''Get source links for the linkcode extension.'''
     module = info['module']
     if domain != 'py' or not module:
         return None
```

### Comparing `mlflow_extra-2023.3/doc/source/mlflow_extra.rst` & `mlflow_extra-2023.4/doc/source/mlflow_extra.rst`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/scripts/install.sh` & `mlflow_extra-2023.4/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/scripts/install_and_run.sh` & `mlflow_extra-2023.4/scripts/install_and_run.sh`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/src/mlflow_extra/filter.py` & `mlflow_extra-2023.4/src/mlflow_extra/filter.py`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/src/mlflow_extra/merge.py` & `mlflow_extra-2023.4/src/mlflow_extra/merge.py`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/src/mlflow_extra/metadata.py` & `mlflow_extra-2023.4/src/mlflow_extra/metadata.py`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/src/mlflow_extra/uri.py` & `mlflow_extra-2023.4/src/mlflow_extra/uri.py`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/LICENSE.txt` & `mlflow_extra-2023.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/README.md` & `mlflow_extra-2023.4/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_extra-2023.3/pyproject.toml` & `mlflow_extra-2023.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ['hatchling', 'hatch-vcs', 'wheel']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'mlflow-extra'
 description = 'Utilities for MLflow'
-license = 'MIT'
+license = {file = 'LICENSE.txt'}
 dependencies = [
   'mlflow',
   'pyyaml'
 ]
 authors = [
   {name = 'Jan-Michael Rye', email = 'jan-michael.rye@inria.fr' }
 ]
```

### Comparing `mlflow_extra-2023.3/PKG-INFO` & `mlflow_extra-2023.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Metadata-Version: 2.1
 Name: mlflow-extra
-Version: 2023.3
+Version: 2023.4
 Summary: Utilities for MLflow
 Project-URL: Source, https://gitlab.inria.fr/jrye/mlflow-extra
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/mlflow-extra/
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
-License-Expression: MIT
+License: MIT License
+        
+        Copyright (c) 2022, Inria
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: mlflow
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
```

