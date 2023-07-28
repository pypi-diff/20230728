# Comparing `tmp/cvat-cli-2.5.0.tar.gz` & `tmp/cvat-cli-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat-cli-2.5.0.tar", last modified: Thu Jul  6 08:18:03 2023, max compression
+gzip compressed data, was "cvat-cli-2.5.2.tar", last modified: Fri Jul 28 10:57:56 2023, max compression
```

## Comparing `cvat-cli-2.5.0.tar` & `cvat-cli-2.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/README.md
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-07-06 04:10:23.000000 cvat-cli-2.5.0/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/setup.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/src/
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/src/cvat_cli/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/src/cvat_cli/__init__.py
--rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2229 2023-06-17 07:46:59.000000 cvat-cli-2.5.0/src/cvat_cli/__main__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4879 2023-07-05 11:32:32.000000 cvat-cli-2.5.0/src/cvat_cli/cli.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13469 2023-06-17 07:46:59.000000 cvat-cli-2.5.0/src/cvat_cli/parser.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-07-06 04:10:23.000000 cvat-cli-2.5.0/src/cvat_cli/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/src/cvat_cli.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/entry_points.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.5.2/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.5.2/README.md
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.5.2/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-07-27 15:53:25.000000 cvat-cli-2.5.2/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.5.2/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/src/
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/src/cvat_cli/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.5.2/src/cvat_cli/__init__.py
+-rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2229 2023-06-17 07:46:59.000000 cvat-cli-2.5.2/src/cvat_cli/__main__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4879 2023-07-13 10:33:37.000000 cvat-cli-2.5.2/src/cvat_cli/cli.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13469 2023-06-17 07:46:59.000000 cvat-cli-2.5.2/src/cvat_cli/parser.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-07-28 10:52:29.000000 cvat-cli-2.5.2/src/cvat_cli/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:57:56.278087 cvat-cli-2.5.2/src/cvat_cli.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-07-28 10:57:56.000000 cvat-cli-2.5.2/src/cvat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-07-28 10:57:56.000000 cvat-cli-2.5.2/src/cvat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-07-28 10:57:56.000000 cvat-cli-2.5.2/src/cvat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-07-28 10:57:56.000000 cvat-cli-2.5.2/src/cvat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-07-28 10:57:56.000000 cvat-cli-2.5.2/src/cvat_cli.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-07-28 10:57:56.000000 cvat-cli-2.5.2/src/cvat_cli.egg-info/top_level.txt
```

### Comparing `cvat-cli-2.5.0/PKG-INFO` & `cvat-cli-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.5.0
+Version: 2.5.2
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cvat-cli-2.5.0/README.md` & `cvat-cli-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.5.0/setup.py` & `cvat-cli-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.5.0/src/cvat_cli/__main__.py` & `cvat-cli-2.5.2/src/cvat_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.5.0/src/cvat_cli/cli.py` & `cvat-cli-2.5.2/src/cvat_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.5.0/src/cvat_cli/parser.py` & `cvat-cli-2.5.2/src/cvat_cli/parser.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.5.0/src/cvat_cli.egg-info/PKG-INFO` & `cvat-cli-2.5.2/src/cvat_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.5.0
+Version: 2.5.2
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

