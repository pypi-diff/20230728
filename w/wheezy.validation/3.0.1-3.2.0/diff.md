# Comparing `tmp/wheezy.validation-3.0.1.tar.gz` & `tmp/wheezy.validation-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.validation-3.0.1.tar", last modified: Sat Dec 19 19:01:37 2020, max compression
+gzip compressed data, was "wheezy.validation-3.2.0.tar", last modified: Fri Jul 28 10:58:31 2023, max compression
```

## Comparing `wheezy.validation-3.0.1.tar` & `wheezy.validation-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 19:01:37.364560 wheezy.validation-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2873 2020-12-19 19:01:37.364560 wheezy.validation-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1588 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-19 19:01:37.364560 wheezy.validation-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2033 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 19:01:37.360560 wheezy.validation-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 19:01:37.360560 wheezy.validation-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 19:01:37.364560 wheezy.validation-3.0.1/src/wheezy/validation/
--rw-r--r--   0 runner    (1001) docker     (116)      266 2020-12-19 19:01:36.000000 wheezy.validation-3.0.1/src/wheezy/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2240 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/checker.py
--rw-r--r--   0 runner    (1001) docker     (116)      182 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/comp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/i18n.py
--rw-r--r--   0 runner    (1001) docker     (116)     1663 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/mixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     7887 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/model.py
--rw-r--r--   0 runner    (1001) docker     (116)      936 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/patches.py
--rw-r--r--   0 runner    (1001) docker     (116)    24362 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (116)     2084 2020-12-19 19:01:26.000000 wheezy.validation-3.0.1/src/wheezy/validation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 19:01:37.360560 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2873 2020-12-19 19:01:37.000000 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      627 2020-12-19 19:01:37.000000 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-19 19:01:37.000000 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-19 19:01:37.000000 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-19 19:01:37.000000 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-19 19:01:37.000000 wheezy.validation-3.0.1/src/wheezy.validation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/src/wheezy/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-28 10:58:29.000000 wheezy.validation-3.2.0/src/wheezy/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24362 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-28 10:58:19.000000 wheezy.validation-3.2.0/src/wheezy/validation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:31.576810 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-28 10:58:31.000000 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-28 10:58:31.000000 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:31.000000 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:31.000000 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:31.000000 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:31.000000 wheezy.validation-3.2.0/src/wheezy.validation.egg-info/top_level.txt
```

### Comparing `wheezy.validation-3.0.1/LICENSE` & `wheezy.validation-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/PKG-INFO` & `wheezy.validation-3.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 Metadata-Version: 2.1
 Name: wheezy.validation
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight object validation library
 Home-page: https://github.com/akornatskyy/wheezy.validation
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.validation
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.validation.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.validation)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.validation/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.validation?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyvalidation/badge/?version=latest)](https://wheezyvalidation.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.validation.svg)](https://badge.fury.io/py/wheezy.validation)
-        
-        [wheezy.validation](https://pypi.org/project/wheezy.validation/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        provides python object validation.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.validation)
-          and [issues](https://github.com/akornatskyy/wheezy.validation/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.validation)
-        - [documentation](https://wheezyvalidation.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.validation](https://pypi.org/project/wheezy.validation/)
-        requires [python](https://www.python.org) version 3.6+. It is independent of
-        operating system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.validation/):
-        
-        ```sh
-        pip install -U wheezy.validation
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyywheezy.validation).
-        
 Keywords: validation rules model
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.validation
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.validation.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.validation)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.validation/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.validation?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyvalidation/badge/?version=latest)](https://wheezyvalidation.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.validation.svg)](https://badge.fury.io/py/wheezy.validation)
+
+[wheezy.validation](https://pypi.org/project/wheezy.validation/) is a
+[python](https://www.python.org) package written in pure Python code. It
+provides python object validation.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.validation)
+  and [issues](https://github.com/akornatskyy/wheezy.validation/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.validation)
+- [documentation](https://wheezyvalidation.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.validation](https://pypi.org/project/wheezy.validation/)
+requires [python](https://www.python.org) version 3.8+. It is independent of
+operating system. You can install it from
+[pypi](https://pypi.org/project/wheezy.validation/):
+
+```sh
+pip install -U wheezy.validation
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyywheezy.validation).
```

### Comparing `wheezy.validation-3.0.1/README.md` & `wheezy.validation-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.validation)
 - [documentation](https://wheezyvalidation.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.validation](https://pypi.org/project/wheezy.validation/)
-requires [python](https://www.python.org) version 3.6+. It is independent of
+requires [python](https://www.python.org) version 3.8+. It is independent of
 operating system. You can install it from
 [pypi](https://pypi.org/project/wheezy.validation/):
 
 ```sh
 pip install -U wheezy.validation
 ```
```

### Comparing `wheezy.validation-3.0.1/setup.py` & `wheezy.validation-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,32 +31,32 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.validation",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight object validation library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.validation",
     author="Andriy Kornatskyy",
     author_email="andriy.kornatskyy@live.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="validation rules model",
     packages=["wheezy", "wheezy.validation"],
     package_dir={"": "src"},
```

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/checker.py` & `wheezy.validation-3.2.0/src/wheezy/validation/checker.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/i18n.py` & `wheezy.validation-3.2.0/src/wheezy/validation/i18n.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/mixin.py` & `wheezy.validation-3.2.0/src/wheezy/validation/mixin.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/model.py` & `wheezy.validation-3.2.0/src/wheezy/validation/model.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/patches.py` & `wheezy.validation-3.2.0/src/wheezy/validation/patches.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/rules.py` & `wheezy.validation-3.2.0/src/wheezy/validation/rules.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy/validation/validator.py` & `wheezy.validation-3.2.0/src/wheezy/validation/validator.py`

 * *Files identical despite different names*

### Comparing `wheezy.validation-3.0.1/src/wheezy.validation.egg-info/PKG-INFO` & `wheezy.validation-3.2.0/src/wheezy.validation.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 Metadata-Version: 2.1
 Name: wheezy.validation
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight object validation library
 Home-page: https://github.com/akornatskyy/wheezy.validation
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.validation
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.validation.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.validation)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.validation/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.validation?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyvalidation/badge/?version=latest)](https://wheezyvalidation.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.validation.svg)](https://badge.fury.io/py/wheezy.validation)
-        
-        [wheezy.validation](https://pypi.org/project/wheezy.validation/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        provides python object validation.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.validation)
-          and [issues](https://github.com/akornatskyy/wheezy.validation/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.validation)
-        - [documentation](https://wheezyvalidation.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.validation](https://pypi.org/project/wheezy.validation/)
-        requires [python](https://www.python.org) version 3.6+. It is independent of
-        operating system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.validation/):
-        
-        ```sh
-        pip install -U wheezy.validation
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyywheezy.validation).
-        
 Keywords: validation rules model
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.validation
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.validation.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.validation)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.validation/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.validation?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyvalidation/badge/?version=latest)](https://wheezyvalidation.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.validation.svg)](https://badge.fury.io/py/wheezy.validation)
+
+[wheezy.validation](https://pypi.org/project/wheezy.validation/) is a
+[python](https://www.python.org) package written in pure Python code. It
+provides python object validation.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.validation)
+  and [issues](https://github.com/akornatskyy/wheezy.validation/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.validation)
+- [documentation](https://wheezyvalidation.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.validation](https://pypi.org/project/wheezy.validation/)
+requires [python](https://www.python.org) version 3.8+. It is independent of
+operating system. You can install it from
+[pypi](https://pypi.org/project/wheezy.validation/):
+
+```sh
+pip install -U wheezy.validation
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyywheezy.validation).
```

### Comparing `wheezy.validation-3.0.1/src/wheezy.validation.egg-info/SOURCES.txt` & `wheezy.validation-3.2.0/src/wheezy.validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

