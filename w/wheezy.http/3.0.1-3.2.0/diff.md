# Comparing `tmp/wheezy.http-3.0.1.tar.gz` & `tmp/wheezy.http-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.http-3.0.1.tar", last modified: Wed Dec 30 08:47:59 2020, max compression
+gzip compressed data, was "wheezy.http-3.2.0.tar", last modified: Fri Jul 28 10:58:22 2023, max compression
```

## Comparing `wheezy.http-3.0.1.tar` & `wheezy.http-3.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 08:47:59.179291 wheezy.http-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3510 2020-12-30 08:47:59.175291 wheezy.http-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1706 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-30 08:47:59.179291 wheezy.http-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 08:47:59.175291 wheezy.http-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 08:47:59.175291 wheezy.http-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 08:47:59.175291 wheezy.http-3.0.1/src/wheezy/http/
--rw-r--r--   0 runner    (1001) docker     (116)     1545 2020-12-30 08:47:57.000000 wheezy.http-3.0.1/src/wheezy/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2006 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/application.py
--rw-r--r--   0 runner    (1001) docker     (116)     1342 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/authorization.py
--rw-r--r--   0 runner    (1001) docker     (116)     4193 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     8002 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/cachepolicy.py
--rw-r--r--   0 runner    (1001) docker     (116)     5711 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/cacheprofile.py
--rw-r--r--   0 runner    (1001) docker     (116)      442 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2523 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/cookie.py
--rw-r--r--   0 runner    (1001) docker     (116)    13975 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/functional.py
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/method.py
--rw-r--r--   0 runner    (1001) docker     (116)     7055 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/middleware.py
--rw-r--r--   0 runner    (1001) docker     (116)     1582 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/parse.py
--rw-r--r--   0 runner    (1001) docker     (116)     3380 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/request.py
--rw-r--r--   0 runner    (1001) docker     (116)     7074 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2196 2020-12-30 08:47:46.000000 wheezy.http-3.0.1/src/wheezy/http/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 08:47:59.175291 wheezy.http-3.0.1/src/wheezy.http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3510 2020-12-30 08:47:58.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      769 2020-12-30 08:47:59.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-30 08:47:58.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-30 08:47:58.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-30 08:47:58.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       21 2020-12-30 08:47:58.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-30 08:47:58.000000 wheezy.http-3.0.1/src/wheezy.http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:22.206438 wheezy.http-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-28 10:58:22.206438 wheezy.http-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:22.206438 wheezy.http-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:22.198439 wheezy.http-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:22.198439 wheezy.http-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:22.206438 wheezy.http-3.2.0/src/wheezy/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-28 10:58:21.000000 wheezy.http-3.2.0/src/wheezy/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/cachepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/cacheprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-28 10:58:13.000000 wheezy.http-3.2.0/src/wheezy/http/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:22.202438 wheezy.http-3.2.0/src/wheezy.http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:22.000000 wheezy.http-3.2.0/src/wheezy.http.egg-info/top_level.txt
```

### Comparing `wheezy.http-3.0.1/LICENSE` & `wheezy.http-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/PKG-INFO` & `wheezy.http-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 Metadata-Version: 2.1
 Name: wheezy.http
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight http request-response library
 Home-page: https://github.com/akornatskyy/wheezy.http
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.http
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.http.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.http)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.http/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.http?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyhttp/badge/?version=latest)](https://wheezyhttp.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.http.svg)](https://badge.fury.io/py/wheezy.http)
-        
-        [wheezy.http](https://pypi.org/project/wheezy.http/) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight http library for things like request, response,
-        headers, cookies and many others. It a wrapper around the
-        [WSGI](http://www.python.org/dev/peps/pep-3333) request environment.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.http),
-          [examples](https://github.com/akornatskyy/wheezy.http/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.http/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.http)
-        - [documentation](https://wheezyhttp.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.http](https://pypi.org/project/wheezy.http/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.http/)
-        site:
-        
-        ```sh
-        pip install -U wheezy.http
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.http).
-        
 Keywords: wsgi http request response cache cachepolicy cookie functional middleware transforms
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
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.http
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.http.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.http)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.http/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.http?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyhttp/badge/?version=latest)](https://wheezyhttp.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.http.svg)](https://badge.fury.io/py/wheezy.http)
+
+[wheezy.http](https://pypi.org/project/wheezy.http/) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight http library for things like request, response,
+headers, cookies and many others. It a wrapper around the
+[WSGI](http://www.python.org/dev/peps/pep-3333) request environment.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.http),
+  [examples](https://github.com/akornatskyy/wheezy.http/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.http/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.http)
+- [documentation](https://wheezyhttp.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.http](https://pypi.org/project/wheezy.http/) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.http/)
+site:
+
+```sh
+pip install -U wheezy.http
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.http).
```

### Comparing `wheezy.http-3.0.1/README.md` & `wheezy.http-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.http)
 - [documentation](https://wheezyhttp.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.http](https://pypi.org/project/wheezy.http/) requires
-[python](https://www.python.org) version 3.6+. It is independent of operating
+[python](https://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from [pypi](https://pypi.org/project/wheezy.http/)
 site:
 
 ```sh
 pip install -U wheezy.http
 ```
```

### Comparing `wheezy.http-3.0.1/setup.py` & `wheezy.http-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,33 +31,33 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.http",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight http request-response library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.http",
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

### Comparing `wheezy.http-3.0.1/src/wheezy/http/__init__.py` & `wheezy.http-3.2.0/src/wheezy/http/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,8 +68,8 @@
     "not_found",
     "permanent_redirect",
     "redirect",
     "see_other",
     "temporary_redirect",
     "unauthorized",
 )
-__version__ = "3.0.1"
+__version__ = "3.2.0"
```

### Comparing `wheezy.http-3.0.1/src/wheezy/http/application.py` & `wheezy.http-3.2.0/src/wheezy/http/application.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/authorization.py` & `wheezy.http-3.2.0/src/wheezy/http/authorization.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/cache.py` & `wheezy.http-3.2.0/src/wheezy/http/cache.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/cachepolicy.py` & `wheezy.http-3.2.0/src/wheezy/http/cachepolicy.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/cacheprofile.py` & `wheezy.http-3.2.0/src/wheezy/http/cacheprofile.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/cookie.py` & `wheezy.http-3.2.0/src/wheezy/http/cookie.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/functional.py` & `wheezy.http-3.2.0/src/wheezy/http/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,17 +418,15 @@
 
         def close(self):
             pass
 
         def feed(self, content):
             fromstring(content, parser=self.parser)
 
-
 except ImportError:  # pragma: nocover
-
     from html.parser import HTMLParser
 
     class HTMLParserAdapter(HTMLParser):
         def __init__(self, target):
             self.strict = True
             self.reset()
             self.target = target
```

### Comparing `wheezy.http-3.0.1/src/wheezy/http/method.py` & `wheezy.http-3.2.0/src/wheezy/http/method.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/middleware.py` & `wheezy.http-3.2.0/src/wheezy/http/middleware.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/parse.py` & `wheezy.http-3.2.0/src/wheezy/http/parse.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/request.py` & `wheezy.http-3.2.0/src/wheezy/http/request.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/response.py` & `wheezy.http-3.2.0/src/wheezy/http/response.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy/http/transforms.py` & `wheezy.http-3.2.0/src/wheezy/http/transforms.py`

 * *Files identical despite different names*

### Comparing `wheezy.http-3.0.1/src/wheezy.http.egg-info/PKG-INFO` & `wheezy.http-3.2.0/src/wheezy.http.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 Metadata-Version: 2.1
 Name: wheezy.http
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight http request-response library
 Home-page: https://github.com/akornatskyy/wheezy.http
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.http
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.http.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.http)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.http/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.http?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyhttp/badge/?version=latest)](https://wheezyhttp.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.http.svg)](https://badge.fury.io/py/wheezy.http)
-        
-        [wheezy.http](https://pypi.org/project/wheezy.http/) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight http library for things like request, response,
-        headers, cookies and many others. It a wrapper around the
-        [WSGI](http://www.python.org/dev/peps/pep-3333) request environment.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.http),
-          [examples](https://github.com/akornatskyy/wheezy.http/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.http/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.http)
-        - [documentation](https://wheezyhttp.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.http](https://pypi.org/project/wheezy.http/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.http/)
-        site:
-        
-        ```sh
-        pip install -U wheezy.http
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.http).
-        
 Keywords: wsgi http request response cache cachepolicy cookie functional middleware transforms
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
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.http
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.http.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.http)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.http/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.http?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyhttp/badge/?version=latest)](https://wheezyhttp.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.http.svg)](https://badge.fury.io/py/wheezy.http)
+
+[wheezy.http](https://pypi.org/project/wheezy.http/) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight http library for things like request, response,
+headers, cookies and many others. It a wrapper around the
+[WSGI](http://www.python.org/dev/peps/pep-3333) request environment.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.http),
+  [examples](https://github.com/akornatskyy/wheezy.http/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.http/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.http)
+- [documentation](https://wheezyhttp.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.http](https://pypi.org/project/wheezy.http/) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.http/)
+site:
+
+```sh
+pip install -U wheezy.http
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.http).
```

### Comparing `wheezy.http-3.0.1/src/wheezy.http.egg-info/SOURCES.txt` & `wheezy.http-3.2.0/src/wheezy.http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

