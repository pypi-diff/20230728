# Comparing `tmp/setuptools-github-0.3.0b64.tar.gz` & `tmp/setuptools-github-0.3.0b65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.0b64.tar", last modified: Fri Jul 28 19:05:01 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.0b65.tar", last modified: Fri Jul 28 19:42:31 2023, max compression
```

## Comparing `setuptools-github-0.3.0b64.tar` & `setuptools-github-0.3.0b65.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.689865 setuptools-github-0.3.0b64/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 19:42:31.000000 setuptools-github-0.3.0b65/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:42:31.090448 setuptools-github-0.3.0b65/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-28 19:42:00.000000 setuptools-github-0.3.0b65/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b64/LICENSE` & `setuptools-github-0.3.0b65/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/PKG-INFO` & `setuptools-github-0.3.0b65/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b64
+Version: 0.3.0b65
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -146,17 +146,17 @@
 On completion static and dynamic tests are supported.
 
 ### Setup the beta/N.M.O branch
 
 In order to prepare for a release a new **beta/N.M.O** branch should be created:
 ```python
 
-python -m setuptools_github.script make-beta 
+python -m setuptools_github.script make-beta src/project_name/__init__.py 
 or
-setuptools-github make-beta
+setuptools-github make-beta src/project_name/__init__.py
 ```
 
 Every commit on **beta/N.M.O** branch ASSUMING [Secrets](#add-secrets) have been set
 properly:
 - Runs mypy on src/
 - Runs ruff on src/
 - Run all tests under tests/
@@ -171,17 +171,17 @@
 > the correct package ordering.
 
 ### Release the project N.M.O
 To release an official package for **project-N.M.O** from
 the **beta/N.M.O** branch:
 ```python
 
-python -m setuptools_github.script micro 
+python -m setuptools_github.script micro src/project_name/__init__.py
 or
-setuptools-github make-beta micro
+setuptools-github make-beta micro src/project_name/__init__.py
 ```
 This will tag the HEAD on **beta/N.M.O** branch 
 with the **release/N.M.O** tag and increment the **initfile** with the
 next version N.M.O+1 (using micro).
 
 Once done, you'll need to push it the tag.
 ```bash
```

### Comparing `setuptools-github-0.3.0b64/README.md` & `setuptools-github-0.3.0b65/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -127,17 +127,17 @@
 On completion static and dynamic tests are supported.
 
 ### Setup the beta/N.M.O branch
 
 In order to prepare for a release a new **beta/N.M.O** branch should be created:
 ```python
 
-python -m setuptools_github.script make-beta 
+python -m setuptools_github.script make-beta src/project_name/__init__.py 
 or
-setuptools-github make-beta
+setuptools-github make-beta src/project_name/__init__.py
 ```
 
 Every commit on **beta/N.M.O** branch ASSUMING [Secrets](#add-secrets) have been set
 properly:
 - Runs mypy on src/
 - Runs ruff on src/
 - Run all tests under tests/
@@ -152,23 +152,23 @@
 > the correct package ordering.
 
 ### Release the project N.M.O
 To release an official package for **project-N.M.O** from
 the **beta/N.M.O** branch:
 ```python
 
-python -m setuptools_github.script micro 
+python -m setuptools_github.script micro src/project_name/__init__.py
 or
-setuptools-github make-beta micro
+setuptools-github make-beta micro src/project_name/__init__.py
 ```
 This will tag the HEAD on **beta/N.M.O** branch 
 with the **release/N.M.O** tag and increment the **initfile** with the
 next version N.M.O+1 (using micro).
 
 Once done, you'll need to push it the tag.
 ```bash
 git push release/N.M.O
 ```
 This will:
 - trigger a CI build that will create the project-name-N.M.O
 - Create a new wheel package under dist/
-- (on success) Send the new wheels **project-N.M.O** to [PyPI](https://pypi.org)
+- (on success) Send the new wheels **project-N.M.O** to [PyPI](https://pypi.org)
```

### Comparing `setuptools-github-0.3.0b64/pyproject.toml` & `setuptools-github-0.3.0b65/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/setup.py` & `setuptools-github-0.3.0b65/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.0b65/setuptools_github.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b64
+Version: 0.3.0b65
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -146,17 +146,17 @@
 On completion static and dynamic tests are supported.
 
 ### Setup the beta/N.M.O branch
 
 In order to prepare for a release a new **beta/N.M.O** branch should be created:
 ```python
 
-python -m setuptools_github.script make-beta 
+python -m setuptools_github.script make-beta src/project_name/__init__.py 
 or
-setuptools-github make-beta
+setuptools-github make-beta src/project_name/__init__.py
 ```
 
 Every commit on **beta/N.M.O** branch ASSUMING [Secrets](#add-secrets) have been set
 properly:
 - Runs mypy on src/
 - Runs ruff on src/
 - Run all tests under tests/
@@ -171,17 +171,17 @@
 > the correct package ordering.
 
 ### Release the project N.M.O
 To release an official package for **project-N.M.O** from
 the **beta/N.M.O** branch:
 ```python
 
-python -m setuptools_github.script micro 
+python -m setuptools_github.script micro src/project_name/__init__.py
 or
-setuptools-github make-beta micro
+setuptools-github make-beta micro src/project_name/__init__.py
 ```
 This will tag the HEAD on **beta/N.M.O** branch 
 with the **release/N.M.O** tag and increment the **initfile** with the
 next version N.M.O+1 (using micro).
 
 Once done, you'll need to push it the tag.
 ```bash
```

### Comparing `setuptools-github-0.3.0b64/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.0b65/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/src/setuptools_github/checks.py` & `setuptools-github-0.3.0b65/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/src/setuptools_github/cli.py` & `setuptools-github-0.3.0b65/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/src/setuptools_github/scm.py` & `setuptools-github-0.3.0b65/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/src/setuptools_github/script.py` & `setuptools-github-0.3.0b65/src/setuptools_github/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This script will either create a new beta branch:
 
      setuptools-github beta ./src/setuptools_github/__init__.py
 
 Or will release the beta branch and will move inot the next minor
 
-    setuptools-github {major|minor|micro} ./src/setuptools_github/__init__.py
+    setuptools-github {major|minor|micro|make-beta} ./src/setuptools_github/__init__.py
 
 """
 from __future__ import annotations
 
 import argparse
 import logging
 import re
@@ -27,16 +27,16 @@
     parser.add_argument(
         "-w",
         "--workdir",
         help="git working dir",
         default=Path("."),
         type=Path,
     )
-    parser.add_argument("initfile", metavar="__init__.py", type=Path)
     parser.add_argument("mode", choices=["micro", "minor", "major", "make-beta"])
+    parser.add_argument("initfile", metavar="__init__.py", type=Path)
 
 
 def process_options(
     options: argparse.Namespace, error: cli.ErrorFn
 ) -> argparse.Namespace:
     try:
         options.repo = repo = scm.GitRepo(options.workdir)
```

### Comparing `setuptools-github-0.3.0b64/src/setuptools_github/tools.py` & `setuptools-github-0.3.0b65/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/conftest.py` & `setuptools-github-0.3.0b65/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/test_checks.py` & `setuptools-github-0.3.0b65/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/test_cli.py` & `setuptools-github-0.3.0b65/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/test_conftest.py` & `setuptools-github-0.3.0b65/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/test_scm.py` & `setuptools-github-0.3.0b65/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/test_script.py` & `setuptools-github-0.3.0b65/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b64/tests/test_tools.py` & `setuptools-github-0.3.0b65/tests/test_tools.py`

 * *Files identical despite different names*

