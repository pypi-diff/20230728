# Comparing `tmp/wheezy.html-3.0.1.tar.gz` & `tmp/wheezy.html-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wheezy.html-3.0.1.tar", last modified: Wed Dec  2 15:14:42 2020, max compression
+gzip compressed data, was "wheezy.html-3.2.0.tar", last modified: Fri Jul 28 10:58:27 2023, max compression
```

## Comparing `wheezy.html-3.0.1.tar` & `wheezy.html-3.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 15:14:42.686606 wheezy.html-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3694 2020-12-02 15:14:42.686606 wheezy.html-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1927 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-02 15:14:42.686606 wheezy.html-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3794 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 15:14:42.682606 wheezy.html-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 15:14:42.682606 wheezy.html-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 15:14:42.686606 wheezy.html-3.0.1/src/wheezy/html/
--rw-r--r--   0 runner    (1001) docker     (116)       31 2020-12-02 15:14:41.000000 wheezy.html-3.0.1/src/wheezy/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4216 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/boost.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 15:14:42.686606 wheezy.html-3.0.1/src/wheezy/html/ext/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6321 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (116)    12598 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/lexer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3551 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/mako.py
--rw-r--r--   0 runner    (1001) docker     (116)     3747 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     4105 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/template.py
--rw-r--r--   0 runner    (1001) docker     (116)     3978 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/ext/tenjin.py
--rw-r--r--   0 runner    (1001) docker     (116)     4196 2020-12-02 15:14:28.000000 wheezy.html-3.0.1/src/wheezy/html/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 15:14:42.686606 wheezy.html-3.0.1/src/wheezy.html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3694 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      629 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      109 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-02 15:14:42.000000 wheezy.html-3.0.1/src/wheezy.html.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.029271 wheezy.html-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 10:58:27.029271 wheezy.html-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:27.029271 wheezy.html-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.025272 wheezy.html-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.025272 wheezy.html-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.029271 wheezy.html-3.2.0/src/wheezy/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 10:58:25.000000 wheezy.html-3.2.0/src/wheezy/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/boost.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.029271 wheezy.html-3.2.0/src/wheezy/html/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/mako.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/ext/tenjin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-28 10:58:15.000000 wheezy.html-3.2.0/src/wheezy/html/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.029271 wheezy.html-3.2.0/src/wheezy.html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 10:58:26.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 10:58:27.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:26.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:26.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:26.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 10:58:26.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:26.000000 wheezy.html-3.2.0/src/wheezy.html.egg-info/top_level.txt
```

### Comparing `wheezy.html-3.0.1/LICENSE` & `wheezy.html-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/PKG-INFO` & `wheezy.html-3.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 Metadata-Version: 2.1
 Name: wheezy.html
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight html rendering library
 Home-page: https://github.com/akornatskyy/wheezy.html
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.html
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.html.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.html)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.html/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.html?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyhtml/badge/?version=latest)](https://wheezyhtml.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.html.svg)](https://badge.fury.io/py/wheezy.html)
-        
-        [wheezy.html](https://pypi.org/project/wheezy.html) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight html widget library. Integrates with the following
-        template systems:
-        
-        - [Jinja2 Templates](http://jinja.pocoo.org)
-        - [Mako Templates](http://www.makotemplates.org)
-        - [Tenjin Templates](http://www.kuwata-lab.com/tenjin/)
-        - [Wheezy Templates](http://pypi.python.org/pypi/wheezy.template/)
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/src) and
-          [issues](https://github.com/akornatskyy/wheezy.html/issues) tracker are
-          available on [github](https://github.com/akornatskyy/wheezy.html)
-        - [documentation](https://wheezyhtml.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.html](https://pypi.org/project/wheezy.html) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.html)
-        site:
-        
-        ```sh
-        pip install -U wheezy.html
-        ```
-        
-        If you would like take a benefit of template preprocessing for Mako,
-        Jinja2, Tenjin or Wheezy.Template engines specify extra requirements:
-        
-        ```sh
-        pip install wheezy.html[wheezy.template]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.html/issues).
-        
 Keywords: html widget markup mako jinja2 tenjin wheezy.template preprocessor
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
 Provides-Extra: mako
 Provides-Extra: tenjin
 Provides-Extra: jinja2
 Provides-Extra: wheezy.template
+License-File: LICENSE
+
+# wheezy.html
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.html.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.html)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.html/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.html?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyhtml/badge/?version=latest)](https://wheezyhtml.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.html.svg)](https://badge.fury.io/py/wheezy.html)
+
+[wheezy.html](https://pypi.org/project/wheezy.html) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight html widget library. Integrates with the following
+template systems:
+
+- [Jinja2 Templates](http://jinja.pocoo.org)
+- [Mako Templates](http://www.makotemplates.org)
+- [Tenjin Templates](http://www.kuwata-lab.com/tenjin/)
+- [Wheezy Templates](http://pypi.python.org/pypi/wheezy.template/)
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/src) and
+  [issues](https://github.com/akornatskyy/wheezy.html/issues) tracker are
+  available on [github](https://github.com/akornatskyy/wheezy.html)
+- [documentation](https://wheezyhtml.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.html](https://pypi.org/project/wheezy.html) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.html)
+site:
+
+```sh
+pip install -U wheezy.html
+```
+
+If you would like take a benefit of template preprocessing for Mako,
+Jinja2, Tenjin or Wheezy.Template engines specify extra requirements:
+
+```sh
+pip install wheezy.html[wheezy.template]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.html/issues).
```

### Comparing `wheezy.html-3.0.1/README.md` & `wheezy.html-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   [issues](https://github.com/akornatskyy/wheezy.html/issues) tracker are
   available on [github](https://github.com/akornatskyy/wheezy.html)
 - [documentation](https://wheezyhtml.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.html](https://pypi.org/project/wheezy.html) requires
-[python](http://www.python.org) version 3.6+. It is independent of operating
+[python](http://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from [pypi](https://pypi.org/project/wheezy.html)
 site:
 
 ```sh
 pip install -U wheezy.html
 ```
```

### Comparing `wheezy.html-3.0.1/setup.py` & `wheezy.html-3.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,33 +71,33 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.html",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight html rendering library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.html",
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

### Comparing `wheezy.html-3.0.1/src/wheezy/html/boost.c` & `wheezy.html-3.2.0/src/wheezy/html/boost.c`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy/html/ext/jinja2.py` & `wheezy.html-3.2.0/src/wheezy/html/ext/jinja2.py`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy/html/ext/lexer.py` & `wheezy.html-3.2.0/src/wheezy/html/ext/lexer.py`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy/html/ext/mako.py` & `wheezy.html-3.2.0/src/wheezy/html/ext/mako.py`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy/html/ext/parser.py` & `wheezy.html-3.2.0/src/wheezy/html/ext/parser.py`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy/html/ext/template.py` & `wheezy.html-3.2.0/src/wheezy/html/ext/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 @if %(value)s:
 <span%(attrs)s>%(info)s</span>\\
 @end
 """
 
 
 class WidgetExtension(object):
-
     preprocessors = [WheezyPreprocessor()]
 
 
 whitespace_preprocessor = WhitespacePreprocessor(
     rules=[
         (re.compile(r"^ [ \t]+", re.MULTILINE), r""),
         (re.compile(r">\s+<", re.MULTILINE), r"><"),
@@ -136,15 +135,14 @@
         lineno, token, value = tokens[i]
         if token == "markup":
             value = whitespace_preprocessor(value)
             tokens[i] = (lineno, token, value)
 
 
 class WhitespaceExtension(object):
-
     preprocessors = [
         WhitespacePreprocessor(
             rules=[(re.compile(r"\s+$", re.MULTILINE), r"")]
         )
     ]
 
     postprocessors = [whitespace_postprocessor]
```

### Comparing `wheezy.html-3.0.1/src/wheezy/html/ext/tenjin.py` & `wheezy.html-3.2.0/src/wheezy/html/ext/tenjin.py`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy/html/utils.py` & `wheezy.html-3.2.0/src/wheezy/html/utils.py`

 * *Files identical despite different names*

### Comparing `wheezy.html-3.0.1/src/wheezy.html.egg-info/PKG-INFO` & `wheezy.html-3.2.0/src/wheezy.html.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 Metadata-Version: 2.1
 Name: wheezy.html
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight html rendering library
 Home-page: https://github.com/akornatskyy/wheezy.html
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.html
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.html.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.html)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.html/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.html?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyhtml/badge/?version=latest)](https://wheezyhtml.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.html.svg)](https://badge.fury.io/py/wheezy.html)
-        
-        [wheezy.html](https://pypi.org/project/wheezy.html) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight html widget library. Integrates with the following
-        template systems:
-        
-        - [Jinja2 Templates](http://jinja.pocoo.org)
-        - [Mako Templates](http://www.makotemplates.org)
-        - [Tenjin Templates](http://www.kuwata-lab.com/tenjin/)
-        - [Wheezy Templates](http://pypi.python.org/pypi/wheezy.template/)
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/src) and
-          [issues](https://github.com/akornatskyy/wheezy.html/issues) tracker are
-          available on [github](https://github.com/akornatskyy/wheezy.html)
-        - [documentation](https://wheezyhtml.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.html](https://pypi.org/project/wheezy.html) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.html)
-        site:
-        
-        ```sh
-        pip install -U wheezy.html
-        ```
-        
-        If you would like take a benefit of template preprocessing for Mako,
-        Jinja2, Tenjin or Wheezy.Template engines specify extra requirements:
-        
-        ```sh
-        pip install wheezy.html[wheezy.template]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.html/issues).
-        
 Keywords: html widget markup mako jinja2 tenjin wheezy.template preprocessor
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
 Provides-Extra: mako
 Provides-Extra: tenjin
 Provides-Extra: jinja2
 Provides-Extra: wheezy.template
+License-File: LICENSE
+
+# wheezy.html
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.html.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.html)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.html/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.html?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyhtml/badge/?version=latest)](https://wheezyhtml.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.html.svg)](https://badge.fury.io/py/wheezy.html)
+
+[wheezy.html](https://pypi.org/project/wheezy.html) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight html widget library. Integrates with the following
+template systems:
+
+- [Jinja2 Templates](http://jinja.pocoo.org)
+- [Mako Templates](http://www.makotemplates.org)
+- [Tenjin Templates](http://www.kuwata-lab.com/tenjin/)
+- [Wheezy Templates](http://pypi.python.org/pypi/wheezy.template/)
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/src) and
+  [issues](https://github.com/akornatskyy/wheezy.html/issues) tracker are
+  available on [github](https://github.com/akornatskyy/wheezy.html)
+- [documentation](https://wheezyhtml.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.html](https://pypi.org/project/wheezy.html) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.html)
+site:
+
+```sh
+pip install -U wheezy.html
+```
+
+If you would like take a benefit of template preprocessing for Mako,
+Jinja2, Tenjin or Wheezy.Template engines specify extra requirements:
+
+```sh
+pip install wheezy.html[wheezy.template]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.html/issues).
```

### Comparing `wheezy.html-3.0.1/src/wheezy.html.egg-info/SOURCES.txt` & `wheezy.html-3.2.0/src/wheezy.html.egg-info/SOURCES.txt`

 * *Files identical despite different names*

