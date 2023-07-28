# Comparing `tmp/wheezy.core-3.0.1.tar.gz` & `tmp/wheezy.core-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wheezy.core-3.0.1.tar", last modified: Sat Dec 12 13:20:57 2020, max compression
+gzip compressed data, was "wheezy.core-3.2.0.tar", last modified: Fri Jul 28 10:58:20 2023, max compression
```

## Comparing `wheezy.core-3.0.1.tar` & `wheezy.core-3.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-12 13:20:57.956440 wheezy.core-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3060 2020-12-12 13:20:57.956440 wheezy.core-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1534 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-12 13:20:57.956440 wheezy.core-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2343 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-12 13:20:57.952440 wheezy.core-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-12 13:20:57.952440 wheezy.core-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-12 13:20:57.956440 wheezy.core-3.0.1/src/wheezy/core/
--rw-r--r--   0 runner    (1001) docker     (116)       31 2020-12-12 13:20:56.000000 wheezy.core-3.0.1/src/wheezy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2849 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)     6409 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/collections.py
--rw-r--r--   0 runner    (1001) docker     (116)     1748 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     5633 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/datetime.py
--rw-r--r--   0 runner    (1001) docker     (116)     6913 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/db.py
--rw-r--r--   0 runner    (1001) docker     (116)      724 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/feistel.py
--rw-r--r--   0 runner    (1001) docker     (116)      420 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/gzip.py
--rw-r--r--   0 runner    (1001) docker     (116)     5696 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (116)     3529 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/i18n.py
--rw-r--r--   0 runner    (1001) docker     (116)     2507 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (116)     1418 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/json.py
--rw-r--r--   0 runner    (1001) docker     (116)     1431 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/luhn.py
--rw-r--r--   0 runner    (1001) docker     (116)     8034 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/mail.py
--rw-r--r--   0 runner    (1001) docker     (116)     2076 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/pooling.py
--rw-r--r--   0 runner    (1001) docker     (116)     2269 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/retry.py
--rw-r--r--   0 runner    (1001) docker     (116)     2416 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/url.py
--rw-r--r--   0 runner    (1001) docker     (116)     1833 2020-12-12 13:20:47.000000 wheezy.core-3.0.1/src/wheezy/core/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-12 13:20:57.952440 wheezy.core-3.0.1/src/wheezy.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3060 2020-12-12 13:20:57.000000 wheezy.core-3.0.1/src/wheezy.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      807 2020-12-12 13:20:57.000000 wheezy.core-3.0.1/src/wheezy.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-12 13:20:57.000000 wheezy.core-3.0.1/src/wheezy.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-12 13:20:57.000000 wheezy.core-3.0.1/src/wheezy.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-12 13:20:57.000000 wheezy.core-3.0.1/src/wheezy.core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-12 13:20:57.000000 wheezy.core-3.0.1/src/wheezy.core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:20.306557 wheezy.core-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-28 10:58:20.306557 wheezy.core-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:20.306557 wheezy.core-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:20.302557 wheezy.core-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:20.302557 wheezy.core-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:20.306557 wheezy.core-3.2.0/src/wheezy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 10:58:18.000000 wheezy.core-3.2.0/src/wheezy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/feistel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/luhn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-28 10:58:11.000000 wheezy.core-3.2.0/src/wheezy/core/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:20.306557 wheezy.core-3.2.0/src/wheezy.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-28 10:58:20.000000 wheezy.core-3.2.0/src/wheezy.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-28 10:58:20.000000 wheezy.core-3.2.0/src/wheezy.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:20.000000 wheezy.core-3.2.0/src/wheezy.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:20.000000 wheezy.core-3.2.0/src/wheezy.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:20.000000 wheezy.core-3.2.0/src/wheezy.core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:20.000000 wheezy.core-3.2.0/src/wheezy.core.egg-info/top_level.txt
```

### Comparing `wheezy.core-3.0.1/LICENSE` & `wheezy.core-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/PKG-INFO` & `wheezy.core-3.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 Metadata-Version: 2.1
 Name: wheezy.core
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight core library
 Home-page: https://github.com/akornatskyy/wheezy.core
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.core
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.core.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.core)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.core/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.core?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezycore/badge/?version=latest)](https://wheezycore.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.core.svg)](https://badge.fury.io/py/wheezy.core)
-        
-        [wheezy.core](https://pypi.org/project/wheezy.core) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        provides core features.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.core),
-          [examples](https://github.com/akornatskyy/wheezy.core/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.core/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.core)
-        - [documentation](https://wheezycore.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.core](https://pypi.org/project/wheezy.core) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.core)
-        site:
-        
-        ```sh
-        pip install -U wheezy.core
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.core).
-        
 Keywords: core benchmark collections config datetime db descriptor feistel i18n introspection json luhn mail pooling url uuid
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
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: System :: Benchmark
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.core
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.core.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.core)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.core/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.core?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezycore/badge/?version=latest)](https://wheezycore.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.core.svg)](https://badge.fury.io/py/wheezy.core)
+
+[wheezy.core](https://pypi.org/project/wheezy.core) is a
+[python](http://www.python.org) package written in pure Python code. It
+provides core features.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.core),
+  [examples](https://github.com/akornatskyy/wheezy.core/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.core/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.core)
+- [documentation](https://wheezycore.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.core](https://pypi.org/project/wheezy.core) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.core)
+site:
+
+```sh
+pip install -U wheezy.core
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.core).
```

### Comparing `wheezy.core-3.0.1/README.md` & `wheezy.core-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.core)
 - [documentation](https://wheezycore.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.core](https://pypi.org/project/wheezy.core) requires
-[python](http://www.python.org) version 3.6+. It is independent of operating
+[python](http://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from [pypi](https://pypi.org/project/wheezy.core)
 site:
 
 ```sh
 pip install -U wheezy.core
 ```
```

### Comparing `wheezy.core-3.0.1/setup.py` & `wheezy.core-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.core",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight core library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.core",
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
         "Topic :: Software Development :: Internationalization",
         "Topic :: Software Development :: Localization",
         "Topic :: System :: Benchmark",
     ],
```

### Comparing `wheezy.core-3.0.1/src/wheezy/core/benchmark.py` & `wheezy.core-3.2.0/src/wheezy/core/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def report(self, name=None, baselines=None):
         baselines = baselines or {}
         print(
             "%s: %s x %s" % (name or "noname", len(self.targets), self.number)
         )
         print("%s %s %s %s" % ("baseline", "throughput", "change", "target"))
         base = None
-        for (name, result) in self.run():
+        for name, result in self.run():
             if not result:
                 print("     - %      - rps    - % " + name)
                 continue
             if base is None:
                 base = result
             base_relative = round(base / result, 3)
             rps = round(self.number / result, 1)
```

### Comparing `wheezy.core-3.0.1/src/wheezy/core/collections.py` & `wheezy.core-3.2.0/src/wheezy/core/collections.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/config.py` & `wheezy.core-3.2.0/src/wheezy/core/config.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/datetime.py` & `wheezy.core-3.2.0/src/wheezy/core/datetime.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/db.py` & `wheezy.core-3.2.0/src/wheezy/core/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,16 @@
         for s in sessions:
             if s.status == SESSION_STATUS_ACTIVE:
                 try:
                     s.connection.tpc_rollback()
                 except Exception:
                     warnings.warn(
                         "An error occured while rolling back "
-                        "two phase transaction."
+                        "two phase transaction.",
+                        stacklevel=2,
                     )
             s.__exit__(exc_type, exc_value, traceback)
 
 
 class NullSession(object):
     """Null session is supposed to be used in mock scenarios."""
```

### Comparing `wheezy.core-3.0.1/src/wheezy/core/descriptors.py` & `wheezy.core-3.2.0/src/wheezy/core/descriptors.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/feistel.py` & `wheezy.core-3.2.0/src/wheezy/core/feistel.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/httpclient.py` & `wheezy.core-3.2.0/src/wheezy/core/httpclient.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/i18n.py` & `wheezy.core-3.2.0/src/wheezy/core/i18n.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/introspection.py` & `wheezy.core-3.2.0/src/wheezy/core/introspection.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/json.py` & `wheezy.core-3.2.0/src/wheezy/core/json.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/luhn.py` & `wheezy.core-3.2.0/src/wheezy/core/luhn.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/mail.py` & `wheezy.core-3.2.0/src/wheezy/core/mail.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/pooling.py` & `wheezy.core-3.2.0/src/wheezy/core/pooling.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/retry.py` & `wheezy.core-3.2.0/src/wheezy/core/retry.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/url.py` & `wheezy.core-3.2.0/src/wheezy/core/url.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy/core/uuid.py` & `wheezy.core-3.2.0/src/wheezy/core/uuid.py`

 * *Files identical despite different names*

### Comparing `wheezy.core-3.0.1/src/wheezy.core.egg-info/PKG-INFO` & `wheezy.core-3.2.0/src/wheezy.core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 Metadata-Version: 2.1
 Name: wheezy.core
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight core library
 Home-page: https://github.com/akornatskyy/wheezy.core
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.core
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.core.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.core)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.core/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.core?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezycore/badge/?version=latest)](https://wheezycore.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.core.svg)](https://badge.fury.io/py/wheezy.core)
-        
-        [wheezy.core](https://pypi.org/project/wheezy.core) is a
-        [python](http://www.python.org) package written in pure Python code. It
-        provides core features.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.core),
-          [examples](https://github.com/akornatskyy/wheezy.core/tree/master/demos)
-          and [issues](https://github.com/akornatskyy/wheezy.core/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.core)
-        - [documentation](https://wheezycore.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.core](https://pypi.org/project/wheezy.core) requires
-        [python](http://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.core)
-        site:
-        
-        ```sh
-        pip install -U wheezy.core
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.core).
-        
 Keywords: core benchmark collections config datetime db descriptor feistel i18n introspection json luhn mail pooling url uuid
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
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: System :: Benchmark
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.core
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.core.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.core)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.core/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.core?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezycore/badge/?version=latest)](https://wheezycore.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.core.svg)](https://badge.fury.io/py/wheezy.core)
+
+[wheezy.core](https://pypi.org/project/wheezy.core) is a
+[python](http://www.python.org) package written in pure Python code. It
+provides core features.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.core),
+  [examples](https://github.com/akornatskyy/wheezy.core/tree/master/demos)
+  and [issues](https://github.com/akornatskyy/wheezy.core/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.core)
+- [documentation](https://wheezycore.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.core](https://pypi.org/project/wheezy.core) requires
+[python](http://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.core)
+site:
+
+```sh
+pip install -U wheezy.core
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.core).
```

### Comparing `wheezy.core-3.0.1/src/wheezy.core.egg-info/SOURCES.txt` & `wheezy.core-3.2.0/src/wheezy.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

