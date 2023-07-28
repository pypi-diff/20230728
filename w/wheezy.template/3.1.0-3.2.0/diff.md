# Comparing `tmp/wheezy.template-3.1.0.tar.gz` & `tmp/wheezy.template-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.template-3.1.0.tar", last modified: Sat Apr 17 07:07:39 2021, max compression
+gzip compressed data, was "wheezy.template-3.2.0.tar", last modified: Fri Jul 28 08:28:53 2023, max compression
```

## Comparing `wheezy.template-3.1.0.tar` & `wheezy.template-3.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:39.007938 wheezy.template-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2021-04-17 07:07:39.007938 wheezy.template-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-17 07:07:39.007938 wheezy.template-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:39.003937 wheezy.template-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:39.003937 wheezy.template-3.1.0/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:39.007938 wheezy.template-3.1.0/src/wheezy/template/
--rw-r--r--   0 runner    (1001) docker     (121)      457 2021-04-17 07:07:37.000000 wheezy.template-3.1.0/src/wheezy/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     6681 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:39.007938 wheezy.template-3.1.0/src/wheezy/template/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/ext/code.py
--rw-r--r--   0 runner    (1001) docker     (121)    13548 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/ext/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/ext/determined.py
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/lexer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6486 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-04-17 07:07:29.000000 wheezy.template-3.1.0/src/wheezy/template/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 07:07:39.007938 wheezy.template-3.1.0/src/wheezy.template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      908 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-17 07:07:38.000000 wheezy.template-3.1.0/src/wheezy.template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/wheezy/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 08:28:51.000000 wheezy.template-3.2.0/src/wheezy/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.211234 wheezy.template-3.2.0/src/wheezy/template/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/ext/determined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-28 08:28:44.000000 wheezy.template-3.2.0/src/wheezy/template/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:53.207236 wheezy.template-3.2.0/src/wheezy.template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 08:28:53.000000 wheezy.template-3.2.0/src/wheezy.template.egg-info/top_level.txt
```

### Comparing `wheezy.template-3.1.0/LICENSE` & `wheezy.template-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/PKG-INFO` & `wheezy.template-3.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 Metadata-Version: 2.1
 Name: wheezy.template
-Version: 3.1.0
+Version: 3.2.0
 Summary: A lightweight template library
 Home-page: https://github.com/akornatskyy/wheezy.template
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.template
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.template.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.template)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.template/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.template?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezytemplate/badge/?version=latest)](https://wheezytemplate.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.template.svg)](https://badge.fury.io/py/wheezy.template)
-        
-        [wheezy.template](https://pypi.org/project/wheezy.template/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        is a lightweight template library. The design goals achived:
-        
-        - **Compact, Expressive, Clean:** Minimizes the number of keystrokes
-          required to build a template. Enables fast and well read coding. You
-          do not need to explicitly denote statement blocks within HTML
-          (unlike other template systems), the parser is smart enough to
-          understand your code. This enables a compact and expressive syntax
-          which is really clean and just pleasure to type.
-        - **Intuitive, No time to Learn:** Basic Python programming skills
-          plus HTML markup. You are productive just from start. Use full power
-          of Python with minimal markup required to denote python statements.
-        - **Do Not Repeat Yourself:** Master layout templates for inheritance;
-          include and import directives for maximum reuse.
-        - **Blazingly Fast:** Maximum rendering performance: ultimate speed
-          and context preprocessor features.
-        
-        Simple template:
-        
-        ```txt
-        @require(user, items)
-        Welcome, @user.name!
-        @if items:
-            @for i in items:
-                @i.name: @i.price!s.
-            @end
-        @else:
-            No items found.
-        @end
-        ```
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.template),
-          [examples](https://github.com/akornatskyy/wheezy.template/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.template/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.template)
-        - [documentation](https://wheezytemplate.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.template](https://pypi.org/project/wheezy.template/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of
-        operating system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.template/) site:
-        
-        ```sh
-        pip install -U wheezy.template
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.template).
-        
 Keywords: html markup template preprocessor
 Platform: any
 Classifier: Environment :: Web Environment
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
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.template
+
+[![tests](https://github.com/akornatskyy/wheezy.template/actions/workflows/tests.yml/badge.svg)](https://github.com/akornatskyy/wheezy.template/actions/workflows/tests.yml)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.template/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.template?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezytemplate/badge/?version=latest)](https://wheezytemplate.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.template.svg)](https://badge.fury.io/py/wheezy.template)
+
+[wheezy.template](https://pypi.org/project/wheezy.template/) is a
+[python](https://www.python.org) package written in pure Python code. It
+is a lightweight template library. The design goals achived:
+
+- **Compact, Expressive, Clean:** Minimizes the number of keystrokes
+  required to build a template. Enables fast and well read coding. You
+  do not need to explicitly denote statement blocks within HTML
+  (unlike other template systems), the parser is smart enough to
+  understand your code. This enables a compact and expressive syntax
+  which is really clean and just pleasure to type.
+- **Intuitive, No time to Learn:** Basic Python programming skills
+  plus HTML markup. You are productive just from start. Use full power
+  of Python with minimal markup required to denote python statements.
+- **Do Not Repeat Yourself:** Master layout templates for inheritance;
+  include and import directives for maximum reuse.
+- **Blazingly Fast:** Maximum rendering performance: ultimate speed
+  and context preprocessor features.
+
+Simple template:
+
+```txt
+@require(user, items)
+Welcome, @user.name!
+@if items:
+    @for i in items:
+        @i.name: @i.price!s.
+    @end
+@else:
+    No items found.
+@end
+```
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.template),
+  [examples](https://github.com/akornatskyy/wheezy.template/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.template/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.template)
+- [documentation](https://wheezytemplate.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.template](https://pypi.org/project/wheezy.template/) requires
+[python](https://www.python.org) version 3.8+. It is independent of
+operating system. You can install it from
+[pypi](https://pypi.org/project/wheezy.template/) site:
+
+```sh
+pip install -U wheezy.template
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.template).
```

### Comparing `wheezy.template-3.1.0/README.md` & `wheezy.template-3.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # wheezy.template
 
-[![Build Status](https://travis-ci.org/akornatskyy/wheezy.template.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.template)
+[![tests](https://github.com/akornatskyy/wheezy.template/actions/workflows/tests.yml/badge.svg)](https://github.com/akornatskyy/wheezy.template/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.template/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.template?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/wheezytemplate/badge/?version=latest)](https://wheezytemplate.readthedocs.io/en/latest/?badge=latest)
 [![pypi version](https://badge.fury.io/py/wheezy.template.svg)](https://badge.fury.io/py/wheezy.template)
 
 [wheezy.template](https://pypi.org/project/wheezy.template/) is a
 [python](https://www.python.org) package written in pure Python code. It
 is a lightweight template library. The design goals achived:
@@ -47,15 +47,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.template)
 - [documentation](https://wheezytemplate.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.template](https://pypi.org/project/wheezy.template/) requires
-[python](https://www.python.org) version 3.6+. It is independent of
+[python](https://www.python.org) version 3.8+. It is independent of
 operating system. You can install it from
 [pypi](https://pypi.org/project/wheezy.template/) site:
 
 ```sh
 pip install -U wheezy.template
 ```
```

### Comparing `wheezy.template-3.1.0/setup.py` & `wheezy.template-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,33 +34,33 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.template",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight template library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.template",
     author="Andriy Kornatskyy",
     author_email="andriy.kornatskyy@live.com",
     license="MIT",
     classifiers=[
         "Environment :: Web Environment",
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
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Widget Sets",
         "Topic :: Text Processing :: Markup :: HTML",
```

### Comparing `wheezy.template-3.1.0/src/wheezy/template/builder.py` & `wheezy.template-3.2.0/src/wheezy/template/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
             rules = extension.builder_rules
             for token, builder in rules:
                 builder_rules.setdefault(token, []).append(builder)
     return {"builder_rules": builder_rules}
 
 
 class BlockBuilder(Builder):
-
     __slots__ = ("rules", "indent", "lineno", "buf")
 
     def __init__(
         self,
         rules: typing.Dict[str, typing.List[BuilderRule]],
         indent: str = "",
         lineno: int = 0,
@@ -83,15 +82,14 @@
             )
 
     def to_string(self) -> str:
         return "\n".join(self.buf)
 
 
 class SourceBuilder(object):
-
     __slots__ = ("rules", "lineno")
 
     def __init__(
         self,
         builder_rules: typing.Dict[str, typing.List[BuilderRule]],
         builder_offset: int = 2,
         **ignore: typing.Any
```

### Comparing `wheezy.template-3.1.0/src/wheezy/template/compiler.py` & `wheezy.template-3.2.0/src/wheezy/template/compiler.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/console.py` & `wheezy.template-3.2.0/src/wheezy/template/console.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/engine.py` & `wheezy.template-3.2.0/src/wheezy/template/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import typing
 from types import ModuleType
 
 from wheezy.template.builder import SourceBuilder, builder_scan
 from wheezy.template.comp import allocate_lock  # type: ignore[attr-defined]
 from wheezy.template.compiler import Compiler
 from wheezy.template.lexer import Lexer, lexer_scan
@@ -40,15 +41,17 @@
         self.lock = allocate_lock()
         self.templates: typing.Dict[str, SupportsRender] = {}
         self.renders: typing.Dict[str, RenderTemplate] = {}
         self.modules: typing.Dict[str, ModuleType] = {}
         self.global_vars = {"_r": self.render, "_i": self.import_name}
         self.loader = loader
         self.template_class = template_class or Template
-        self.compiler = Compiler(self.global_vars, -2)
+        self.compiler = Compiler(
+            self.global_vars, sys.version_info >= (3, 11, 0) and -1 or -2
+        )
         self.lexer = Lexer(**lexer_scan(extensions))
         self.parser = Parser(**parser_scan(extensions))
         self.builder = SourceBuilder(**builder_scan(extensions))
 
     def get_template(self, name: str) -> SupportsRender:
         """Returns compiled template."""
         try:
@@ -62,15 +65,14 @@
         name: str,
         ctx: typing.Mapping[str, typing.Any],
         local_defs: typing.Mapping[str, typing.Any],
         super_defs: typing.Mapping[str, typing.Any],
     ) -> str:
         """Renders template by name in given context."""
         try:
-
             return self.renders[name](ctx, local_defs, super_defs)
         except KeyError:
             self.compile_template(name)
             return self.renders[name](ctx, local_defs, super_defs)
 
     def remove(self, name: str) -> None:
         """Removes given ``name`` from internal cache."""
```

### Comparing `wheezy.template-3.1.0/src/wheezy/template/ext/code.py` & `wheezy.template-3.2.0/src/wheezy/template/ext/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 # region: core extension
 
 
 class CodeExtension:
     """Includes support for embedded python code."""
 
     def __init__(self, token_start: str = "@") -> None:
-
         self.lexer_rules: typing.Mapping[int, LexerRule] = {
             300: (re.compile(r"\s*%s(?=\()" % token_start), code_token),
         }
 
     parser_rules: typing.Mapping[str, ParserRule] = {"code": parse_code}
 
     builder_rules: typing.List[typing.Tuple[str, typing.Any]] = [
```

### Comparing `wheezy.template-3.1.0/src/wheezy/template/ext/core.py` & `wheezy.template-3.2.0/src/wheezy/template/ext/core.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/ext/determined.py` & `wheezy.template-3.2.0/src/wheezy/template/ext/determined.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/lexer.py` & `wheezy.template-3.2.0/src/wheezy/template/lexer.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/loader.py` & `wheezy.template-3.2.0/src/wheezy/template/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
 
 class AutoReloadProxy(Engine):
     def __init__(self, engine: Engine):
         from warnings import warn
 
         self.engine = engine
-        self.names: typing.Dict[str, int] = {}
+        self.names: typing.Dict[str, float] = {}
         warn(
             "autoreload limitation: master (inherited), imported "
             "and preprocessed templates. It is recommended to use "
             "application server that supports file reload instead.",
             stacklevel=3,
         )
 
@@ -186,15 +186,15 @@
 
     def __getattr__(self, name: str) -> typing.Any:
         return getattr(self.engine, name)
 
     def file_changed(self, name: str) -> bool:
         try:
             last_known_stamp = self.names[name]
-            current_time = int(time.time())
+            current_time = time.time()
             if current_time - last_known_stamp <= 2:
                 return False
         except KeyError:
             last_known_stamp = 0
 
         loader = self.engine.loader
         abspath = loader.get_fullname(name)  # type: ignore[attr-defined]
```

### Comparing `wheezy.template-3.1.0/src/wheezy/template/parser.py` & `wheezy.template-3.2.0/src/wheezy/template/parser.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/preprocessor.py` & `wheezy.template-3.2.0/src/wheezy/template/preprocessor.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy/template/typing.py` & `wheezy.template-3.2.0/src/wheezy/template/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import sys
 import typing
 from abc import abstractmethod
 
-Token = typing.Tuple[int, str, str]
+if sys.version_info <= (3, 9, 0):  # pragma: nocover
+    Token = typing.Tuple[int, str, str]
+else:  # pragma: nocover
+    Token = tuple[int, str, str]  # type: ignore[misc]
 
 
 class Builder:
     lineno: int
 
     @abstractmethod
     def start_block(self) -> None:
```

### Comparing `wheezy.template-3.1.0/src/wheezy/template/utils.py` & `wheezy.template-3.2.0/src/wheezy/template/utils.py`

 * *Files identical despite different names*

### Comparing `wheezy.template-3.1.0/src/wheezy.template.egg-info/PKG-INFO` & `wheezy.template-3.2.0/src/wheezy.template.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 Metadata-Version: 2.1
 Name: wheezy.template
-Version: 3.1.0
+Version: 3.2.0
 Summary: A lightweight template library
 Home-page: https://github.com/akornatskyy/wheezy.template
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.template
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.template.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.template)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.template/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.template?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezytemplate/badge/?version=latest)](https://wheezytemplate.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.template.svg)](https://badge.fury.io/py/wheezy.template)
-        
-        [wheezy.template](https://pypi.org/project/wheezy.template/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        is a lightweight template library. The design goals achived:
-        
-        - **Compact, Expressive, Clean:** Minimizes the number of keystrokes
-          required to build a template. Enables fast and well read coding. You
-          do not need to explicitly denote statement blocks within HTML
-          (unlike other template systems), the parser is smart enough to
-          understand your code. This enables a compact and expressive syntax
-          which is really clean and just pleasure to type.
-        - **Intuitive, No time to Learn:** Basic Python programming skills
-          plus HTML markup. You are productive just from start. Use full power
-          of Python with minimal markup required to denote python statements.
-        - **Do Not Repeat Yourself:** Master layout templates for inheritance;
-          include and import directives for maximum reuse.
-        - **Blazingly Fast:** Maximum rendering performance: ultimate speed
-          and context preprocessor features.
-        
-        Simple template:
-        
-        ```txt
-        @require(user, items)
-        Welcome, @user.name!
-        @if items:
-            @for i in items:
-                @i.name: @i.price!s.
-            @end
-        @else:
-            No items found.
-        @end
-        ```
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.template),
-          [examples](https://github.com/akornatskyy/wheezy.template/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.template/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.template)
-        - [documentation](https://wheezytemplate.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.template](https://pypi.org/project/wheezy.template/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of
-        operating system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.template/) site:
-        
-        ```sh
-        pip install -U wheezy.template
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.template).
-        
 Keywords: html markup template preprocessor
 Platform: any
 Classifier: Environment :: Web Environment
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
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.template
+
+[![tests](https://github.com/akornatskyy/wheezy.template/actions/workflows/tests.yml/badge.svg)](https://github.com/akornatskyy/wheezy.template/actions/workflows/tests.yml)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.template/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.template?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezytemplate/badge/?version=latest)](https://wheezytemplate.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.template.svg)](https://badge.fury.io/py/wheezy.template)
+
+[wheezy.template](https://pypi.org/project/wheezy.template/) is a
+[python](https://www.python.org) package written in pure Python code. It
+is a lightweight template library. The design goals achived:
+
+- **Compact, Expressive, Clean:** Minimizes the number of keystrokes
+  required to build a template. Enables fast and well read coding. You
+  do not need to explicitly denote statement blocks within HTML
+  (unlike other template systems), the parser is smart enough to
+  understand your code. This enables a compact and expressive syntax
+  which is really clean and just pleasure to type.
+- **Intuitive, No time to Learn:** Basic Python programming skills
+  plus HTML markup. You are productive just from start. Use full power
+  of Python with minimal markup required to denote python statements.
+- **Do Not Repeat Yourself:** Master layout templates for inheritance;
+  include and import directives for maximum reuse.
+- **Blazingly Fast:** Maximum rendering performance: ultimate speed
+  and context preprocessor features.
+
+Simple template:
+
+```txt
+@require(user, items)
+Welcome, @user.name!
+@if items:
+    @for i in items:
+        @i.name: @i.price!s.
+    @end
+@else:
+    No items found.
+@end
+```
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.template),
+  [examples](https://github.com/akornatskyy/wheezy.template/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.template/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.template)
+- [documentation](https://wheezytemplate.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.template](https://pypi.org/project/wheezy.template/) requires
+[python](https://www.python.org) version 3.8+. It is independent of
+operating system. You can install it from
+[pypi](https://pypi.org/project/wheezy.template/) site:
+
+```sh
+pip install -U wheezy.template
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.template).
```

### Comparing `wheezy.template-3.1.0/src/wheezy.template.egg-info/SOURCES.txt` & `wheezy.template-3.2.0/src/wheezy.template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

