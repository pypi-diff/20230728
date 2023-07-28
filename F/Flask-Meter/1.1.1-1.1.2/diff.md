# Comparing `tmp/Flask-Meter-1.1.1.tar.gz` & `tmp/Flask-Meter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Meter-1.1.1.tar", last modified: Thu Jul 27 16:19:38 2023, max compression
+gzip compressed data, was "Flask-Meter-1.1.2.tar", last modified: Fri Jul 28 15:17:22 2023, max compression
```

## Comparing `Flask-Meter-1.1.1.tar` & `Flask-Meter-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/
--rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/AUTHORS.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      688 2023-07-27 16:17:14.000000 Flask-Meter-1.1.1/HISTORY.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/LICENSE
--rw-rw-r--   0 herman    (1000) herman    (1000)      264 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/MANIFEST.in
--rw-rw-r--   0 herman    (1000) herman    (1000)     4520 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)     3091 2023-07-27 15:32:18.000000 Flask-Meter-1.1.1/README.rst
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/docs/
--rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/Makefile
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/docs/_build/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/docs/_build/html/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/docs/_build/html/_static/
--rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-02-19 21:41:17.000000 Flask-Meter-1.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-02-19 21:41:17.000000 Flask-Meter-1.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-02-19 21:41:17.000000 Flask-Meter-1.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/authors.rst
--rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/docs/conf.py
--rw-rw-r--   0 herman    (1000) herman    (1000)       33 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/contributing.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      627 2023-07-27 16:17:36.000000 Flask-Meter-1.1.1/docs/flask_meter.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/history.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/docs/index.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/installation.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/make.bat
--rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-07-27 16:17:36.000000 Flask-Meter-1.1.1/docs/modules.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       27 2018-04-17 03:06:44.000000 Flask-Meter-1.1.1/docs/readme.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/docs/usage.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/pyproject.toml
--rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/setup.cfg
--rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/setup.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/Flask_Meter.egg-info/
--rw-rw-r--   0 herman    (1000) herman    (1000)     4520 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/Flask_Meter.egg-info/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)      788 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/Flask_Meter.egg-info/SOURCES.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/Flask_Meter.egg-info/dependency_links.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/Flask_Meter.egg-info/requires.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/Flask_Meter.egg-info/top_level.txt
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/src/flask_meter/
--rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-07-27 16:17:14.000000 Flask-Meter-1.1.1/src/flask_meter/__init__.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     2504 2023-07-27 15:30:59.000000 Flask-Meter-1.1.1/src/flask_meter/flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     1179 2023-07-27 16:08:16.000000 Flask-Meter-1.1.1/src/flask_meter/git.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      207 2023-07-27 16:17:14.000000 Flask-Meter-1.1.1/src/flask_meter/version.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/tests/
--rw-rw-r--   0 herman    (1000) herman    (1000)     2608 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/tests/test_flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      449 2023-07-26 22:55:52.000000 Flask-Meter-1.1.1/tests/test_git.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 16:19:38.000000 Flask-Meter-1.1.1/tests/version/
--rw-rw-r--   0 herman    (1000) herman    (1000)      652 2023-07-27 16:17:14.000000 Flask-Meter-1.1.1/tests/version/test_version.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/AUTHORS.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/CONTRIBUTING.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      770 2023-07-28 02:04:41.000000 Flask-Meter-1.1.2/HISTORY.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/LICENSE
+-rw-rw-r--   0 herman    (1000) herman    (1000)      264 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/MANIFEST.in
+-rw-rw-r--   0 herman    (1000) herman    (1000)     4520 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3091 2023-07-27 15:32:18.000000 Flask-Meter-1.1.2/README.rst
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/docs/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/Makefile
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.035828 Flask-Meter-1.1.2/docs/_build/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.035828 Flask-Meter-1.1.2/docs/_build/html/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/docs/_build/html/_static/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-07-27 21:57:49.000000 Flask-Meter-1.1.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-07-27 21:57:49.000000 Flask-Meter-1.1.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-07-27 21:57:49.000000 Flask-Meter-1.1.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/authors.rst
+-rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/docs/conf.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)       33 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/contributing.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      627 2023-07-27 21:58:04.000000 Flask-Meter-1.1.2/docs/flask_meter.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/history.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/docs/index.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/installation.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/make.bat
+-rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-07-27 21:58:04.000000 Flask-Meter-1.1.2/docs/modules.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       27 2018-04-17 03:06:44.000000 Flask-Meter-1.1.2/docs/readme.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/docs/usage.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/pyproject.toml
+-rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/setup.cfg
+-rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/setup.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.035828 Flask-Meter-1.1.2/src/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/src/Flask_Meter.egg-info/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     4520 2023-07-28 15:17:22.000000 Flask-Meter-1.1.2/src/Flask_Meter.egg-info/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)      788 2023-07-28 15:17:22.000000 Flask-Meter-1.1.2/src/Flask_Meter.egg-info/SOURCES.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-07-28 15:17:22.000000 Flask-Meter-1.1.2/src/Flask_Meter.egg-info/dependency_links.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-07-28 15:17:22.000000 Flask-Meter-1.1.2/src/Flask_Meter.egg-info/requires.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-07-28 15:17:22.000000 Flask-Meter-1.1.2/src/Flask_Meter.egg-info/top_level.txt
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/src/flask_meter/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-07-28 02:04:00.000000 Flask-Meter-1.1.2/src/flask_meter/__init__.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2504 2023-07-27 15:30:59.000000 Flask-Meter-1.1.2/src/flask_meter/flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1179 2023-07-27 16:08:16.000000 Flask-Meter-1.1.2/src/flask_meter/git.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      207 2023-07-27 16:17:14.000000 Flask-Meter-1.1.2/src/flask_meter/version.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/tests/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2608 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/tests/test_flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      449 2023-07-26 22:55:52.000000 Flask-Meter-1.1.2/tests/test_git.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-28 15:17:22.039828 Flask-Meter-1.1.2/tests/version/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      652 2023-07-27 16:17:14.000000 Flask-Meter-1.1.2/tests/version/test_version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-Meter-1.1.1/CONTRIBUTING.rst` & `Flask-Meter-1.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/HISTORY.rst` & `Flask-Meter-1.1.2/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 History
 =======
 
+1.1.2 (2023-07-28)
+------------------
+* Fixes an issue with documentation builds
+
 1.1.1 (2023-07-27)
 ------------------
 * Fixes a bug where whitespace is not stripped from version stats
 
 1.1.0 (2023-07-27)
 ------------------
 * Add version stats
```

### Comparing `Flask-Meter-1.1.1/LICENSE` & `Flask-Meter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/PKG-INFO` & `Flask-Meter-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Meter
-Version: 1.1.1
+Version: 1.1.2
 Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
 Author-email: Herman Singh <kartstig@gmail.com>
 Maintainer-email: Herman Singh <kartstig@gmail.com>
 License: MIT License
 Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Source Code, https://github.com/Kartstig/flask-meter
```

### Comparing `Flask-Meter-1.1.1/README.rst` & `Flask-Meter-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/docs/Makefile` & `Flask-Meter-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/docs/conf.py` & `Flask-Meter-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/docs/flask_meter.rst` & `Flask-Meter-1.1.2/docs/flask_meter.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/docs/installation.rst` & `Flask-Meter-1.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/docs/make.bat` & `Flask-Meter-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/pyproject.toml` & `Flask-Meter-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/src/Flask_Meter.egg-info/PKG-INFO` & `Flask-Meter-1.1.2/src/Flask_Meter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Meter
-Version: 1.1.1
+Version: 1.1.2
 Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
 Author-email: Herman Singh <kartstig@gmail.com>
 Maintainer-email: Herman Singh <kartstig@gmail.com>
 License: MIT License
 Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Source Code, https://github.com/Kartstig/flask-meter
```

### Comparing `Flask-Meter-1.1.1/src/Flask_Meter.egg-info/SOURCES.txt` & `Flask-Meter-1.1.2/src/Flask_Meter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/src/flask_meter/flask_meter.py` & `Flask-Meter-1.1.2/src/flask_meter/flask_meter.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/src/flask_meter/git.py` & `Flask-Meter-1.1.2/src/flask_meter/git.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/tests/test_flask_meter.py` & `Flask-Meter-1.1.2/tests/test_flask_meter.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.1.1/tests/version/test_version.py` & `Flask-Meter-1.1.2/tests/version/test_version.py`

 * *Files identical despite different names*

