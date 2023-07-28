# Comparing `tmp/wheezy.web-3.0.1.tar.gz` & `tmp/wheezy.web-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.web-3.0.1.tar", last modified: Wed Dec 30 09:01:25 2020, max compression
+gzip compressed data, was "wheezy.web-3.2.0.tar", last modified: Fri Jul 28 10:58:38 2023, max compression
```

## Comparing `wheezy.web-3.0.1.tar` & `wheezy.web-3.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       26 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4842 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3458 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.105588 wheezy.web-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.105588 wheezy.web-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/src/wheezy/web/
--rw-r--r--   0 runner    (1001) docker     (116)      199 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2942 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/authorization.py
--rw-r--r--   0 runner    (1001) docker     (116)      107 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/src/wheezy/web/handlers/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11075 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1540 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/handlers/file.py
--rw-r--r--   0 runner    (1001) docker     (116)     1434 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/handlers/method.py
--rw-r--r--   0 runner    (1001) docker     (116)     1001 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/handlers/template.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/src/wheezy/web/middleware/
--rw-r--r--   0 runner    (1001) docker     (116)      374 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/middleware/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (116)     2478 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/middleware/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)      794 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/middleware/routing.py
--rw-r--r--   0 runner    (1001) docker     (116)     3748 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/templates.py
--rw-r--r--   0 runner    (1001) docker     (116)      857 2020-12-30 09:01:14.000000 wheezy.web-3.0.1/src/wheezy/web/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 09:01:25.109588 wheezy.web-3.0.1/src/wheezy.web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4842 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      796 2020-12-30 09:01:25.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      271 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-30 09:01:24.000000 wheezy.web-3.0.1/src/wheezy.web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/src/wheezy/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-28 10:58:36.000000 wheezy.web-3.2.0/src/wheezy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/src/wheezy/web/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/handlers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/handlers/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/handlers/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/src/wheezy/web/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/middleware/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/middleware/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/middleware/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-28 10:58:23.000000 wheezy.web-3.2.0/src/wheezy/web/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:38.090995 wheezy.web-3.2.0/src/wheezy.web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:38.000000 wheezy.web-3.2.0/src/wheezy.web.egg-info/top_level.txt
```

### Comparing `wheezy.web-3.0.1/LICENSE` & `wheezy.web-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/PKG-INFO` & `wheezy.web-3.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,93 @@
 Metadata-Version: 2.1
 Name: wheezy.web
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight, high performance, high concurrency WSGI web framework with the key features to build modern, efficient web
 Home-page: https://github.com/akornatskyy/wheezy.web
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.web
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.web.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.web)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.web/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.web?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyweb/badge/?version=latest)](https://wheezyweb.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.web.svg)](https://badge.fury.io/py/wheezy.web)
-        
-        [wheezy.web](https://pypi.org/project/wheezy.web/) is a lightweight,
-        [high performance](https://mindref.blogspot.com/2012/09/python-fastest-web-framework.html),
-        high concurrency [WSGI](http://www.python.org/dev/peps/pep-3333) web
-        framework with the key features to *build modern, efficient web*:
-        
-        - Requires Python 3.6+.
-        - MVC architectural pattern
-          ([push](http://en.wikipedia.org/wiki/Web_application_framework#Push-based_vs._pull-based)-based).
-        - Functionality includes
-          [routing](https://github.com/akornatskyy/wheezy.routing),
-          [model update/validation](https://github.com/akornatskyy/wheezy.validation),
-          [authentication/authorization](https://github.com/akornatskyy/wheezy.security),
-          [content](https://wheezyhttp.readthedocs.io/en/latest/userguide.html#content-cache)
-          [caching](https://github.com/akornatskyy/wheezy.caching) with
-          [dependency](https://wheezycaching.readthedocs.io/en/latest/userguide.html#cachedependency),
-          xsrf/resubmission protection, AJAX+JSON, i18n (gettext),
-          middlewares, and more.
-        - Template engine agnostic (integration with
-          [jinja2](http://jinja.pocoo.org),
-          [mako](http://www.makotemplates.org),
-          [tenjin](http://www.kuwata-lab.com/tenjin/) and
-          [wheezy.template](https://github.com/akornatskyy/wheezy.template)) plus
-          [html widgets](https://github.com/akornatskyy/wheezy.html).
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.web),
-          [examples](https://github.com/akornatskyy/wheezy.web/tree/master/demos)
-          ([live](http://wheezy.pythonanywhere.com)) and
-          [issues](https://github.com/akornatskyy/wheezy.web/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.web)
-        - [documentation](https://wheezyweb.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.web](https://pypi.org/project/wheezy.web/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.web/)
-        site:
-        
-        ```sh
-        pip install -U wheezy.web
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.web).
-        
 Keywords: wsgi web handler static template mako tenjin jinja2 routing middleware caching transforms
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
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: mako
 Provides-Extra: tenjin
 Provides-Extra: jinja2
 Provides-Extra: wheezy.template
+License-File: LICENSE
+
+# wheezy.web
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.web.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.web)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.web/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.web?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyweb/badge/?version=latest)](https://wheezyweb.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.web.svg)](https://badge.fury.io/py/wheezy.web)
+
+[wheezy.web](https://pypi.org/project/wheezy.web/) is a lightweight,
+[high performance](https://mindref.blogspot.com/2012/09/python-fastest-web-framework.html),
+high concurrency [WSGI](http://www.python.org/dev/peps/pep-3333) web
+framework with the key features to *build modern, efficient web*:
+
+- Requires Python 3.6+.
+- MVC architectural pattern
+  ([push](http://en.wikipedia.org/wiki/Web_application_framework#Push-based_vs._pull-based)-based).
+- Functionality includes
+  [routing](https://github.com/akornatskyy/wheezy.routing),
+  [model update/validation](https://github.com/akornatskyy/wheezy.validation),
+  [authentication/authorization](https://github.com/akornatskyy/wheezy.security),
+  [content](https://wheezyhttp.readthedocs.io/en/latest/userguide.html#content-cache)
+  [caching](https://github.com/akornatskyy/wheezy.caching) with
+  [dependency](https://wheezycaching.readthedocs.io/en/latest/userguide.html#cachedependency),
+  xsrf/resubmission protection, AJAX+JSON, i18n (gettext),
+  middlewares, and more.
+- Template engine agnostic (integration with
+  [jinja2](http://jinja.pocoo.org),
+  [mako](http://www.makotemplates.org),
+  [tenjin](http://www.kuwata-lab.com/tenjin/) and
+  [wheezy.template](https://github.com/akornatskyy/wheezy.template)) plus
+  [html widgets](https://github.com/akornatskyy/wheezy.html).
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.web),
+  [examples](https://github.com/akornatskyy/wheezy.web/tree/master/demos)
+  ([live](http://wheezy.pythonanywhere.com)) and
+  [issues](https://github.com/akornatskyy/wheezy.web/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.web)
+- [documentation](https://wheezyweb.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.web](https://pypi.org/project/wheezy.web/) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.web/)
+site:
+
+```sh
+pip install -U wheezy.web
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.web).
```

### Comparing `wheezy.web-3.0.1/README.md` & `wheezy.web-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.web)
 - [documentation](https://wheezyweb.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.web](https://pypi.org/project/wheezy.web/) requires
-[python](https://www.python.org) version 3.6+. It is independent of operating
+[python](https://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from [pypi](https://pypi.org/project/wheezy.web/)
 site:
 
 ```sh
 pip install -U wheezy.web
 ```
```

### Comparing `wheezy.web-3.0.1/setup.py` & `wheezy.web-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     import uuid  # noqa
 except ImportError:
     install_requires.append("uuid")
 
 setup(
     name="wheezy.web",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight, high performance, high concurrency WSGI "
     "web framework with the key features to build modern, efficient web",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.web",
     author="Andriy Kornatskyy",
     author_email="andriy.kornatskyy@live.com",
@@ -70,18 +70,18 @@
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

### Comparing `wheezy.web-3.0.1/src/wheezy/web/authorization.py` & `wheezy.web-3.2.0/src/wheezy/web/authorization.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/handlers/__init__.py` & `wheezy.web-3.2.0/src/wheezy/web/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/handlers/base.py` & `wheezy.web-3.2.0/src/wheezy/web/handlers/base.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/handlers/file.py` & `wheezy.web-3.2.0/src/wheezy/web/handlers/file.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/handlers/method.py` & `wheezy.web-3.2.0/src/wheezy/web/handlers/method.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/handlers/template.py` & `wheezy.web-3.2.0/src/wheezy/web/handlers/template.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/middleware/bootstrap.py` & `wheezy.web-3.2.0/src/wheezy/web/middleware/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/middleware/errors.py` & `wheezy.web-3.2.0/src/wheezy/web/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/middleware/routing.py` & `wheezy.web-3.2.0/src/wheezy/web/middleware/routing.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/templates.py` & `wheezy.web-3.2.0/src/wheezy/web/templates.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy/web/transforms.py` & `wheezy.web-3.2.0/src/wheezy/web/transforms.py`

 * *Files identical despite different names*

### Comparing `wheezy.web-3.0.1/src/wheezy.web.egg-info/PKG-INFO` & `wheezy.web-3.2.0/src/wheezy.web.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,93 @@
 Metadata-Version: 2.1
 Name: wheezy.web
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight, high performance, high concurrency WSGI web framework with the key features to build modern, efficient web
 Home-page: https://github.com/akornatskyy/wheezy.web
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.web
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.web.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.web)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.web/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.web?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezyweb/badge/?version=latest)](https://wheezyweb.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.web.svg)](https://badge.fury.io/py/wheezy.web)
-        
-        [wheezy.web](https://pypi.org/project/wheezy.web/) is a lightweight,
-        [high performance](https://mindref.blogspot.com/2012/09/python-fastest-web-framework.html),
-        high concurrency [WSGI](http://www.python.org/dev/peps/pep-3333) web
-        framework with the key features to *build modern, efficient web*:
-        
-        - Requires Python 3.6+.
-        - MVC architectural pattern
-          ([push](http://en.wikipedia.org/wiki/Web_application_framework#Push-based_vs._pull-based)-based).
-        - Functionality includes
-          [routing](https://github.com/akornatskyy/wheezy.routing),
-          [model update/validation](https://github.com/akornatskyy/wheezy.validation),
-          [authentication/authorization](https://github.com/akornatskyy/wheezy.security),
-          [content](https://wheezyhttp.readthedocs.io/en/latest/userguide.html#content-cache)
-          [caching](https://github.com/akornatskyy/wheezy.caching) with
-          [dependency](https://wheezycaching.readthedocs.io/en/latest/userguide.html#cachedependency),
-          xsrf/resubmission protection, AJAX+JSON, i18n (gettext),
-          middlewares, and more.
-        - Template engine agnostic (integration with
-          [jinja2](http://jinja.pocoo.org),
-          [mako](http://www.makotemplates.org),
-          [tenjin](http://www.kuwata-lab.com/tenjin/) and
-          [wheezy.template](https://github.com/akornatskyy/wheezy.template)) plus
-          [html widgets](https://github.com/akornatskyy/wheezy.html).
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.web),
-          [examples](https://github.com/akornatskyy/wheezy.web/tree/master/demos)
-          ([live](http://wheezy.pythonanywhere.com)) and
-          [issues](https://github.com/akornatskyy/wheezy.web/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.web)
-        - [documentation](https://wheezyweb.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.web](https://pypi.org/project/wheezy.web/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from [pypi](https://pypi.org/project/wheezy.web/)
-        site:
-        
-        ```sh
-        pip install -U wheezy.web
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.web).
-        
 Keywords: wsgi web handler static template mako tenjin jinja2 routing middleware caching transforms
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
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: mako
 Provides-Extra: tenjin
 Provides-Extra: jinja2
 Provides-Extra: wheezy.template
+License-File: LICENSE
+
+# wheezy.web
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.web.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.web)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.web/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.web?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezyweb/badge/?version=latest)](https://wheezyweb.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.web.svg)](https://badge.fury.io/py/wheezy.web)
+
+[wheezy.web](https://pypi.org/project/wheezy.web/) is a lightweight,
+[high performance](https://mindref.blogspot.com/2012/09/python-fastest-web-framework.html),
+high concurrency [WSGI](http://www.python.org/dev/peps/pep-3333) web
+framework with the key features to *build modern, efficient web*:
+
+- Requires Python 3.6+.
+- MVC architectural pattern
+  ([push](http://en.wikipedia.org/wiki/Web_application_framework#Push-based_vs._pull-based)-based).
+- Functionality includes
+  [routing](https://github.com/akornatskyy/wheezy.routing),
+  [model update/validation](https://github.com/akornatskyy/wheezy.validation),
+  [authentication/authorization](https://github.com/akornatskyy/wheezy.security),
+  [content](https://wheezyhttp.readthedocs.io/en/latest/userguide.html#content-cache)
+  [caching](https://github.com/akornatskyy/wheezy.caching) with
+  [dependency](https://wheezycaching.readthedocs.io/en/latest/userguide.html#cachedependency),
+  xsrf/resubmission protection, AJAX+JSON, i18n (gettext),
+  middlewares, and more.
+- Template engine agnostic (integration with
+  [jinja2](http://jinja.pocoo.org),
+  [mako](http://www.makotemplates.org),
+  [tenjin](http://www.kuwata-lab.com/tenjin/) and
+  [wheezy.template](https://github.com/akornatskyy/wheezy.template)) plus
+  [html widgets](https://github.com/akornatskyy/wheezy.html).
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.web),
+  [examples](https://github.com/akornatskyy/wheezy.web/tree/master/demos)
+  ([live](http://wheezy.pythonanywhere.com)) and
+  [issues](https://github.com/akornatskyy/wheezy.web/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.web)
+- [documentation](https://wheezyweb.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.web](https://pypi.org/project/wheezy.web/) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from [pypi](https://pypi.org/project/wheezy.web/)
+site:
+
+```sh
+pip install -U wheezy.web
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.web).
```

### Comparing `wheezy.web-3.0.1/src/wheezy.web.egg-info/SOURCES.txt` & `wheezy.web-3.2.0/src/wheezy.web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

