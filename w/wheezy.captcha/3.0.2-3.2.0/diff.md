# Comparing `tmp/wheezy.captcha-3.0.2.tar.gz` & `tmp/wheezy.captcha-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.captcha-3.0.2.tar", last modified: Wed Jul  7 06:10:05 2021, max compression
+gzip compressed data, was "wheezy.captcha-3.2.0.tar", last modified: Fri Jul 28 10:58:39 2023, max compression
```

## Comparing `wheezy.captcha-3.0.2.tar` & `wheezy.captcha-3.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 06:10:05.838630 wheezy.captcha-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-07-07 06:10:05.838630 wheezy.captcha-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-07 06:10:05.838630 wheezy.captcha-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 06:10:05.834630 wheezy.captcha-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 06:10:05.838630 wheezy.captcha-3.0.2/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 06:10:05.838630 wheezy.captcha-3.0.2/src/wheezy/captcha/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-07-07 06:10:04.000000 wheezy.captcha-3.0.2/src/wheezy/captcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/src/wheezy/captcha/bezier.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/src/wheezy/captcha/comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4635 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/src/wheezy/captcha/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     5623 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/src/wheezy/captcha/image.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2021-07-07 06:09:54.000000 wheezy.captcha-3.0.2/src/wheezy/captcha/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 06:10:05.838630 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-07 06:10:05.000000 wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:39.457051 wheezy.captcha-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-28 10:58:39.457051 wheezy.captcha-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:39.457051 wheezy.captcha-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:39.453050 wheezy.captcha-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:39.457051 wheezy.captcha-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:39.457051 wheezy.captcha-3.2.0/src/wheezy/captcha/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 10:58:38.000000 wheezy.captcha-3.2.0/src/wheezy/captcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/src/wheezy/captcha/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/src/wheezy/captcha/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/src/wheezy/captcha/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/src/wheezy/captcha/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-28 10:58:27.000000 wheezy.captcha-3.2.0/src/wheezy/captcha/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:39.457051 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:39.000000 wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/top_level.txt
```

### Comparing `wheezy.captcha-3.0.2/LICENSE` & `wheezy.captcha-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.captcha-3.0.2/PKG-INFO` & `wheezy.captcha-3.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 Metadata-Version: 2.1
 Name: wheezy.captcha
-Version: 3.0.2
+Version: 3.2.0
 Summary: A lightweight captcha library
 Home-page: https://github.com/akornatskyy/wheezy.captcha
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.captcha
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.captcha.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.captcha)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.captcha/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.captcha?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezycaptcha/badge/?version=latest)](https://wheezycaptcha.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.captcha.svg)](https://badge.fury.io/py/wheezy.captcha)
-        
-        [wheezy.captcha](https://pypi.org/project/wheezy.captcha/) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight captcha library that provides integration with (one of
-        below must be installed):
-        
-        - [PIL](http://www.pythonware.com/products/pil/) - Python Imaging
-          Library 1.1.7.
-        - [Pillow](https://pypi.python.org/pypi/Pillow) - Python Imaging
-          Library (fork).
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.captcha),
-          [examples](https://github.com/akornatskyy/wheezy.captcha/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.captcha/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.captcha)
-        - [documentation](https://wheezycaptcha.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.captcha](https://pypi.org/project/wheezy.captcha/) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.captcha/) site (you need specify
-        extra requirements per imaging library of your choice):
-        
-        ```sh
-        pip install wheezy.captcha
-        pip install wheezy.captcha[PIL]
-        pip install wheezy.captcha[Pillow]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.captcha).
-        
 Keywords: wsgi http captcha
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
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: PIL
 Provides-Extra: Pillow
+License-File: LICENSE
+
+# wheezy.captcha
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.captcha.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.captcha)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.captcha/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.captcha?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezycaptcha/badge/?version=latest)](https://wheezycaptcha.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.captcha.svg)](https://badge.fury.io/py/wheezy.captcha)
+
+[wheezy.captcha](https://pypi.org/project/wheezy.captcha/) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight captcha library that provides integration with (one of
+below must be installed):
+
+- [PIL](http://www.pythonware.com/products/pil/) - Python Imaging
+  Library 1.1.7.
+- [Pillow](https://pypi.python.org/pypi/Pillow) - Python Imaging
+  Library (fork).
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.captcha),
+  [examples](https://github.com/akornatskyy/wheezy.captcha/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.captcha/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.captcha)
+- [documentation](https://wheezycaptcha.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.captcha](https://pypi.org/project/wheezy.captcha/) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.captcha/) site (you need specify
+extra requirements per imaging library of your choice):
+
+```sh
+pip install wheezy.captcha
+pip install wheezy.captcha[PIL]
+pip install wheezy.captcha[Pillow]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.captcha).
```

### Comparing `wheezy.captcha-3.0.2/README.md` & `wheezy.captcha-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.captcha)
 - [documentation](https://wheezycaptcha.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.captcha](https://pypi.org/project/wheezy.captcha/) requires
-[python](http://www.python.org) version 3.6+. It is independent of operating
+[python](http://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from
 [pypi](https://pypi.org/project/wheezy.captcha/) site (you need specify
 extra requirements per imaging library of your choice):
 
 ```sh
 pip install wheezy.captcha
 pip install wheezy.captcha[PIL]
```

### Comparing `wheezy.captcha-3.0.2/setup.py` & `wheezy.captcha-3.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,33 +38,33 @@
     import uuid  # noqa
 except ImportError:
     install_requires.append("uuid")
 
 setup(
     name="wheezy.captcha",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight captcha library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.captcha",
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
         "Topic :: Internet :: WWW/HTTP :: WSGI",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
```

### Comparing `wheezy.captcha-3.0.2/src/wheezy/captcha/bezier.py` & `wheezy.captcha-3.2.0/src/wheezy/captcha/bezier.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     try:
         return beziers[n]
     except KeyError:
         combinations = pascal_row(n - 1)
         result = []
         for t in tsequence:
-            tpowers = (t ** i for i in range(n))
+            tpowers = (t**i for i in range(n))
             upowers = ((1 - t) ** i for i in range(n - 1, -1, -1))
             coefs = [
                 c * a * b for c, a, b in zip(combinations, tpowers, upowers)
             ]
             result.append(coefs)
         beziers[n] = result
         return result
```

### Comparing `wheezy.captcha-3.0.2/src/wheezy/captcha/http.py` & `wheezy.captcha-3.2.0/src/wheezy/captcha/http.py`

 * *Files identical despite different names*

### Comparing `wheezy.captcha-3.0.2/src/wheezy/captcha/image.py` & `wheezy.captcha-3.2.0/src/wheezy/captcha/image.py`

 * *Files identical despite different names*

### Comparing `wheezy.captcha-3.0.2/src/wheezy/captcha/mixin.py` & `wheezy.captcha-3.2.0/src/wheezy/captcha/mixin.py`

 * *Files identical despite different names*

### Comparing `wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/PKG-INFO` & `wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 Metadata-Version: 2.1
 Name: wheezy.captcha
-Version: 3.0.2
+Version: 3.2.0
 Summary: A lightweight captcha library
 Home-page: https://github.com/akornatskyy/wheezy.captcha
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.captcha
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.captcha.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.captcha)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.captcha/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.captcha?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezycaptcha/badge/?version=latest)](https://wheezycaptcha.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.captcha.svg)](https://badge.fury.io/py/wheezy.captcha)
-        
-        [wheezy.captcha](https://pypi.org/project/wheezy.captcha/) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight captcha library that provides integration with (one of
-        below must be installed):
-        
-        - [PIL](http://www.pythonware.com/products/pil/) - Python Imaging
-          Library 1.1.7.
-        - [Pillow](https://pypi.python.org/pypi/Pillow) - Python Imaging
-          Library (fork).
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.captcha),
-          [examples](https://github.com/akornatskyy/wheezy.captcha/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.captcha/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.captcha)
-        - [documentation](https://wheezycaptcha.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.captcha](https://pypi.org/project/wheezy.captcha/) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.captcha/) site (you need specify
-        extra requirements per imaging library of your choice):
-        
-        ```sh
-        pip install wheezy.captcha
-        pip install wheezy.captcha[PIL]
-        pip install wheezy.captcha[Pillow]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.captcha).
-        
 Keywords: wsgi http captcha
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
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: PIL
 Provides-Extra: Pillow
+License-File: LICENSE
+
+# wheezy.captcha
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.captcha.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.captcha)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.captcha/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.captcha?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezycaptcha/badge/?version=latest)](https://wheezycaptcha.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.captcha.svg)](https://badge.fury.io/py/wheezy.captcha)
+
+[wheezy.captcha](https://pypi.org/project/wheezy.captcha/) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight captcha library that provides integration with (one of
+below must be installed):
+
+- [PIL](http://www.pythonware.com/products/pil/) - Python Imaging
+  Library 1.1.7.
+- [Pillow](https://pypi.python.org/pypi/Pillow) - Python Imaging
+  Library (fork).
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.captcha),
+  [examples](https://github.com/akornatskyy/wheezy.captcha/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.captcha/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.captcha)
+- [documentation](https://wheezycaptcha.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.captcha](https://pypi.org/project/wheezy.captcha/) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.captcha/) site (you need specify
+extra requirements per imaging library of your choice):
+
+```sh
+pip install wheezy.captcha
+pip install wheezy.captcha[PIL]
+pip install wheezy.captcha[Pillow]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.captcha).
```

### Comparing `wheezy.captcha-3.0.2/src/wheezy.captcha.egg-info/SOURCES.txt` & `wheezy.captcha-3.2.0/src/wheezy.captcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

