# Comparing `tmp/wheezy.caching-3.0.1.tar.gz` & `tmp/wheezy.caching-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.caching-3.0.1.tar", last modified: Tue Dec 29 14:39:05 2020, max compression
+gzip compressed data, was "wheezy.caching-3.2.0.tar", last modified: Fri Jul 28 10:58:32 2023, max compression
```

## Comparing `wheezy.caching-3.0.1.tar` & `wheezy.caching-3.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 14:39:05.924600 wheezy.caching-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3472 2020-12-29 14:39:05.924600 wheezy.caching-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2031 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-29 14:39:05.924600 wheezy.caching-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 14:39:05.920600 wheezy.caching-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 14:39:05.920600 wheezy.caching-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 14:39:05.924600 wheezy.caching-3.0.1/src/wheezy/caching/
--rw-r--r--   0 runner    (1001) docker     (116)      293 2020-12-29 14:39:04.000000 wheezy.caching-3.0.1/src/wheezy/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4825 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     3157 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/dependency.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     5884 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/lockout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/logging.py
--rw-r--r--   0 runner    (1001) docker     (116)     5042 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/memcache.py
--rw-r--r--   0 runner    (1001) docker     (116)    13835 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/memory.py
--rw-r--r--   0 runner    (1001) docker     (116)     3702 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/null.py
--rw-r--r--   0 runner    (1001) docker     (116)    16706 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/patterns.py
--rw-r--r--   0 runner    (1001) docker     (116)     6989 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/pylibmc.py
--rw-r--r--   0 runner    (1001) docker     (116)      716 2020-12-29 14:38:52.000000 wheezy.caching-3.0.1/src/wheezy/caching/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 14:39:05.920600 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3472 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      722 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-29 14:39:05.000000 wheezy.caching-3.0.1/src/wheezy.caching.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:32.092097 wheezy.caching-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-28 10:58:32.092097 wheezy.caching-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:32.092097 wheezy.caching-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:32.088097 wheezy.caching-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:32.088097 wheezy.caching-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:32.092097 wheezy.caching-3.2.0/src/wheezy/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-28 10:58:29.000000 wheezy.caching-3.2.0/src/wheezy/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/lockout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/pylibmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-28 10:58:18.000000 wheezy.caching-3.2.0/src/wheezy/caching/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:32.088097 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:32.000000 wheezy.caching-3.2.0/src/wheezy.caching.egg-info/top_level.txt
```

### Comparing `wheezy.caching-3.0.1/LICENSE` & `wheezy.caching-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/PKG-INFO` & `wheezy.caching-3.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 Metadata-Version: 2.1
 Name: wheezy.caching
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight caching library
 Home-page: https://github.com/akornatskyy/wheezy.caching
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.caching
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.caching.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.caching)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.caching/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.caching?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezycaching/badge/?version=latest)](https://wheezycaching.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.caching.svg)](https://badge.fury.io/py/wheezy.caching)
-        
-        [wheezy.caching](https://pypi.org/project/wheezy.caching/) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight caching library that provides integration with:
-        
-        - [python-memcached](https://pypi.org/project/python-memcached/) -
-          Pure Python [memcached](http://memcached.org) client.
-        - [pylibmc](https://pypi.org/project/pylibmc/) - Quick and small
-          [memcached](http://memcached.org) client for Python written in C.
-        
-        It introduces idea of *cache dependency* (effectively invalidate
-        dependent cache items) and other cache related algorithms.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.caching)
-          and [issues](https://github.com/akornatskyy/wheezy.caching/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.caching)
-        - [documentation](https://wheezycaching.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.caching](https://pypi.org/project/wheezy.caching/) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.caching/) site:
-        
-        ```sh
-        pip install -U wheezy.caching
-        pip install -U wheezy.caching[pylibmc]
-        pip install -U wheezy.caching[python-memcached]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.caching).
-        
 Keywords: caching dependency memory null memcache memcached pylibmc
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
 Provides-Extra: pylibmc
 Provides-Extra: python-memcached
+License-File: LICENSE
+
+# wheezy.caching
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.caching.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.caching)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.caching/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.caching?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezycaching/badge/?version=latest)](https://wheezycaching.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.caching.svg)](https://badge.fury.io/py/wheezy.caching)
+
+[wheezy.caching](https://pypi.org/project/wheezy.caching/) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight caching library that provides integration with:
+
+- [python-memcached](https://pypi.org/project/python-memcached/) -
+  Pure Python [memcached](http://memcached.org) client.
+- [pylibmc](https://pypi.org/project/pylibmc/) - Quick and small
+  [memcached](http://memcached.org) client for Python written in C.
+
+It introduces idea of *cache dependency* (effectively invalidate
+dependent cache items) and other cache related algorithms.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.caching)
+  and [issues](https://github.com/akornatskyy/wheezy.caching/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.caching)
+- [documentation](https://wheezycaching.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.caching](https://pypi.org/project/wheezy.caching/) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.caching/) site:
+
+```sh
+pip install -U wheezy.caching
+pip install -U wheezy.caching[pylibmc]
+pip install -U wheezy.caching[python-memcached]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.caching).
```

### Comparing `wheezy.caching-3.0.1/README.md` & `wheezy.caching-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.caching)
 - [documentation](https://wheezycaching.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.caching](https://pypi.org/project/wheezy.caching/) requires
-[python](http://www.python.org) version 3.6+. It is independent of operating
+[python](http://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from
 [pypi](https://pypi.org/project/wheezy.caching/) site:
 
 ```sh
 pip install -U wheezy.caching
 pip install -U wheezy.caching[pylibmc]
 pip install -U wheezy.caching[python-memcached]
```

### Comparing `wheezy.caching-3.0.1/setup.py` & `wheezy.caching-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,32 +31,32 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.caching",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight caching library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.caching",
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
     keywords="caching dependency memory null memcache memcached pylibmc",
     packages=["wheezy", "wheezy.caching"],
     package_dir={"": "src"},
```

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/client.py` & `wheezy.caching-3.2.0/src/wheezy/caching/client.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/dependency.py` & `wheezy.caching-3.2.0/src/wheezy/caching/dependency.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/encoding.py` & `wheezy.caching-3.2.0/src/wheezy/caching/encoding.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/lockout.py` & `wheezy.caching-3.2.0/src/wheezy/caching/lockout.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/logging.py` & `wheezy.caching-3.2.0/src/wheezy/caching/logging.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/memcache.py` & `wheezy.caching-3.2.0/src/wheezy/caching/memcache.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/memory.py` & `wheezy.caching-3.2.0/src/wheezy/caching/memory.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/null.py` & `wheezy.caching-3.2.0/src/wheezy/caching/null.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/patterns.py` & `wheezy.caching-3.2.0/src/wheezy/caching/patterns.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/pylibmc.py` & `wheezy.caching-3.2.0/src/wheezy/caching/pylibmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         """Client factory for pylibmc."""
         kwargs.setdefault("binary", True)
         behaviors = kwargs.setdefault("behaviors", {})
         behaviors.setdefault("tcp_nodelay", True)
         behaviors.setdefault("ketama", True)
         return Client(*args, **kwargs)
 
-
 except ImportError:  # pragma: nocover
     import warnings
 
     warnings.warn("No module named 'pylibmc'", stacklevel=2)
 
 
 class MemcachedClient(object):
```

### Comparing `wheezy.caching-3.0.1/src/wheezy/caching/utils.py` & `wheezy.caching-3.2.0/src/wheezy/caching/utils.py`

 * *Files identical despite different names*

### Comparing `wheezy.caching-3.0.1/src/wheezy.caching.egg-info/PKG-INFO` & `wheezy.caching-3.2.0/src/wheezy.caching.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 Metadata-Version: 2.1
 Name: wheezy.caching
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight caching library
 Home-page: https://github.com/akornatskyy/wheezy.caching
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.caching
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.caching.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.caching)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.caching/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.caching?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezycaching/badge/?version=latest)](https://wheezycaching.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.caching.svg)](https://badge.fury.io/py/wheezy.caching)
-        
-        [wheezy.caching](https://pypi.org/project/wheezy.caching/) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        is a lightweight caching library that provides integration with:
-        
-        - [python-memcached](https://pypi.org/project/python-memcached/) -
-          Pure Python [memcached](http://memcached.org) client.
-        - [pylibmc](https://pypi.org/project/pylibmc/) - Quick and small
-          [memcached](http://memcached.org) client for Python written in C.
-        
-        It introduces idea of *cache dependency* (effectively invalidate
-        dependent cache items) and other cache related algorithms.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.caching)
-          and [issues](https://github.com/akornatskyy/wheezy.caching/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.caching)
-        - [documentation](https://wheezycaching.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.caching](https://pypi.org/project/wheezy.caching/) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.caching/) site:
-        
-        ```sh
-        pip install -U wheezy.caching
-        pip install -U wheezy.caching[pylibmc]
-        pip install -U wheezy.caching[python-memcached]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.caching).
-        
 Keywords: caching dependency memory null memcache memcached pylibmc
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
 Provides-Extra: pylibmc
 Provides-Extra: python-memcached
+License-File: LICENSE
+
+# wheezy.caching
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.caching.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.caching)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.caching/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.caching?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezycaching/badge/?version=latest)](https://wheezycaching.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.caching.svg)](https://badge.fury.io/py/wheezy.caching)
+
+[wheezy.caching](https://pypi.org/project/wheezy.caching/) is a
+[python](http://www.python.org) package written in pure Python code. It
+is a lightweight caching library that provides integration with:
+
+- [python-memcached](https://pypi.org/project/python-memcached/) -
+  Pure Python [memcached](http://memcached.org) client.
+- [pylibmc](https://pypi.org/project/pylibmc/) - Quick and small
+  [memcached](http://memcached.org) client for Python written in C.
+
+It introduces idea of *cache dependency* (effectively invalidate
+dependent cache items) and other cache related algorithms.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.caching)
+  and [issues](https://github.com/akornatskyy/wheezy.caching/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.caching)
+- [documentation](https://wheezycaching.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.caching](https://pypi.org/project/wheezy.caching/) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.caching/) site:
+
+```sh
+pip install -U wheezy.caching
+pip install -U wheezy.caching[pylibmc]
+pip install -U wheezy.caching[python-memcached]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.caching).
```

### Comparing `wheezy.caching-3.0.1/src/wheezy.caching.egg-info/SOURCES.txt` & `wheezy.caching-3.2.0/src/wheezy.caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

