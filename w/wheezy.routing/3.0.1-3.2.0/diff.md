# Comparing `tmp/wheezy.routing-3.0.1.tar.gz` & `tmp/wheezy.routing-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.routing-3.0.1.tar", last modified: Sat Dec 19 14:59:03 2020, max compression
+gzip compressed data, was "wheezy.routing-3.2.0.tar", last modified: Fri Jul 28 10:58:27 2023, max compression
```

## Comparing `wheezy.routing-3.0.1.tar` & `wheezy.routing-3.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 14:59:03.660545 wheezy.routing-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3467 2020-12-19 14:59:03.660545 wheezy.routing-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1863 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-19 14:59:03.660545 wheezy.routing-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2290 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 14:59:03.656545 wheezy.routing-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 14:59:03.660545 wheezy.routing-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 14:59:03.660545 wheezy.routing-3.0.1/src/wheezy/routing/
--rw-r--r--   0 runner    (1001) docker     (116)      130 2020-12-19 14:59:02.000000 wheezy.routing-3.0.1/src/wheezy/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      478 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/builders.py
--rw-r--r--   0 runner    (1001) docker     (116)     1834 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/choice.py
--rw-r--r--   0 runner    (1001) docker     (116)      520 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     1936 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/curly.py
--rw-r--r--   0 runner    (1001) docker     (116)     2040 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/plain.py
--rw-r--r--   0 runner    (1001) docker     (116)     4845 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/regex.py
--rw-r--r--   0 runner    (1001) docker     (116)      435 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/route.py
--rw-r--r--   0 runner    (1001) docker     (116)     5461 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/router.py
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2020-12-19 14:58:52.000000 wheezy.routing-3.0.1/src/wheezy/routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 14:59:03.660545 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3467 2020-12-19 14:59:03.000000 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      610 2020-12-19 14:59:03.000000 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-19 14:59:03.000000 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-19 14:59:03.000000 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-19 14:59:03.000000 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-19 14:59:03.000000 wheezy.routing-3.0.1/src/wheezy.routing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.039023 wheezy.routing-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-28 10:58:27.039023 wheezy.routing-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:27.039023 wheezy.routing-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.035023 wheezy.routing-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.039023 wheezy.routing-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.039023 wheezy.routing-3.2.0/src/wheezy/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 10:58:25.000000 wheezy.routing-3.2.0/src/wheezy/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/curly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-28 10:58:17.000000 wheezy.routing-3.2.0/src/wheezy/routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:27.039023 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-28 10:58:26.000000 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 10:58:27.000000 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:26.000000 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:26.000000 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:26.000000 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:26.000000 wheezy.routing-3.2.0/src/wheezy.routing.egg-info/top_level.txt
```

### Comparing `wheezy.routing-3.0.1/LICENSE` & `wheezy.routing-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/PKG-INFO` & `wheezy.routing-3.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 Metadata-Version: 2.1
 Name: wheezy.routing
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight path routing library
 Home-page: https://github.com/akornatskyy/wheezy.routing
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.routing
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.routing.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.routing)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.routing/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.routing?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyrouting/badge/?version=latest)](https://wheezyrouting.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.routing.svg)](https://badge.fury.io/py/wheezy.routing)
-        
-        [wheezy.routing](https://pypi.org/project/wheezy.routing/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        is a simple mapping between URL patterns (as plain simple strings, curly
-        expressions or regular expressions) to a handler that can be anything
-        you like (there is no limitation or prescription what handler is or
-        could be).
-        
-        The mapping can include other mappings and constructed dynamically.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.routing),
-          [examples](https://github.com/akornatskyy/wheezy.routing/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.routing/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.routing)
-        - [documentation](https://wheezyrouting.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.routing](https://pypi.org/project/wheezy.routing) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.routing/):
-        
-        ```sh
-        pip install -U wheezy.routing
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.routing).
-        
 Keywords: routing path url patterns match web mapping
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.routing
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.routing.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.routing)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.routing/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.routing?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyrouting/badge/?version=latest)](https://wheezyrouting.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.routing.svg)](https://badge.fury.io/py/wheezy.routing)
+
+[wheezy.routing](https://pypi.org/project/wheezy.routing/) is a
+[python](https://www.python.org) package written in pure Python code. It
+is a simple mapping between URL patterns (as plain simple strings, curly
+expressions or regular expressions) to a handler that can be anything
+you like (there is no limitation or prescription what handler is or
+could be).
+
+The mapping can include other mappings and constructed dynamically.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.routing),
+  [examples](https://github.com/akornatskyy/wheezy.routing/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.routing/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.routing)
+- [documentation](https://wheezyrouting.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.routing](https://pypi.org/project/wheezy.routing) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.routing/):
+
+```sh
+pip install -U wheezy.routing
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.routing).
```

### Comparing `wheezy.routing-3.0.1/README.md` & `wheezy.routing-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.routing)
 - [documentation](https://wheezyrouting.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.routing](https://pypi.org/project/wheezy.routing) requires
-[python](https://www.python.org) version 3.6+. It is independent of operating
+[python](https://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from
 [pypi](https://pypi.org/project/wheezy.routing/):
 
 ```sh
 pip install -U wheezy.routing
 ```
```

### Comparing `wheezy.routing-3.0.1/setup.py` & `wheezy.routing-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,33 +31,33 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.routing",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight path routing library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.routing",
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
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/choice.py` & `wheezy.routing-3.2.0/src/wheezy/routing/choice.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/config.py` & `wheezy.routing-3.2.0/src/wheezy/routing/config.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/curly.py` & `wheezy.routing-3.2.0/src/wheezy/routing/curly.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/plain.py` & `wheezy.routing-3.2.0/src/wheezy/routing/plain.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/regex.py` & `wheezy.routing-3.2.0/src/wheezy/routing/regex.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/router.py` & `wheezy.routing-3.2.0/src/wheezy/routing/router.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy/routing/utils.py` & `wheezy.routing-3.2.0/src/wheezy/routing/utils.py`

 * *Files identical despite different names*

### Comparing `wheezy.routing-3.0.1/src/wheezy.routing.egg-info/PKG-INFO` & `wheezy.routing-3.2.0/src/wheezy.routing.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 Metadata-Version: 2.1
 Name: wheezy.routing
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight path routing library
 Home-page: https://github.com/akornatskyy/wheezy.routing
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.routing
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.routing.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.routing)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.routing/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.routing?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyrouting/badge/?version=latest)](https://wheezyrouting.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.routing.svg)](https://badge.fury.io/py/wheezy.routing)
-        
-        [wheezy.routing](https://pypi.org/project/wheezy.routing/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        is a simple mapping between URL patterns (as plain simple strings, curly
-        expressions or regular expressions) to a handler that can be anything
-        you like (there is no limitation or prescription what handler is or
-        could be).
-        
-        The mapping can include other mappings and constructed dynamically.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.routing),
-          [examples](https://github.com/akornatskyy/wheezy.routing/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.routing/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.routing)
-        - [documentation](https://wheezyrouting.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.routing](https://pypi.org/project/wheezy.routing) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.routing/):
-        
-        ```sh
-        pip install -U wheezy.routing
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.routing).
-        
 Keywords: routing path url patterns match web mapping
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.routing
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.routing.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.routing)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.routing/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.routing?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyrouting/badge/?version=latest)](https://wheezyrouting.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.routing.svg)](https://badge.fury.io/py/wheezy.routing)
+
+[wheezy.routing](https://pypi.org/project/wheezy.routing/) is a
+[python](https://www.python.org) package written in pure Python code. It
+is a simple mapping between URL patterns (as plain simple strings, curly
+expressions or regular expressions) to a handler that can be anything
+you like (there is no limitation or prescription what handler is or
+could be).
+
+The mapping can include other mappings and constructed dynamically.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.routing),
+  [examples](https://github.com/akornatskyy/wheezy.routing/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.routing/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.routing)
+- [documentation](https://wheezyrouting.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.routing](https://pypi.org/project/wheezy.routing) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.routing/):
+
+```sh
+pip install -U wheezy.routing
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.routing).
```

### Comparing `wheezy.routing-3.0.1/src/wheezy.routing.egg-info/SOURCES.txt` & `wheezy.routing-3.2.0/src/wheezy.routing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

