# Comparing `tmp/idefix_cli-2.3.2.tar.gz` & `tmp/idefix_cli-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.3.2.tar", last modified: Wed Jul 26 17:12:39 2023, max compression
+gzip compressed data, was "idefix_cli-2.3.3.tar", last modified: Fri Jul 28 15:49:29 2023, max compression
```

## Comparing `idefix_cli-2.3.2.tar` & `idefix_cli-2.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.335352 idefix_cli-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.335352 idefix_cli-2.3.2/src/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/src/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.335352 idefix_cli-2.3.2/src/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.334329 idefix_cli-2.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.334329 idefix_cli-2.3.3/src/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.338329 idefix_cli-2.3.3/src/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.338329 idefix_cli-2.3.3/src/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_write.py
```

### Comparing `idefix_cli-2.3.2/LICENSE` & `idefix_cli-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/PKG-INFO` & `idefix_cli-2.3.3/src/idefix_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idefix_cli
-Version: 2.3.2
+Name: idefix-cli
+Version: 2.3.3
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-2.3.2/README.md` & `idefix_cli-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/pyproject.toml` & `idefix_cli-2.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/__main__.py` & `idefix_cli-2.3.3/src/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_backports.py` & `idefix_cli-2.3.3/src/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/clean.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/clone.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     make_file_tree,
     print_err,
     print_warning,
 )
 
 BASE_INCLUDE = frozenset(
     (
-        "idefix.ini",
+        "*.ini",
         "*.hpp",
         "*.cpp",
         "*.h",
         "*.c",
         "CMakeLists.txt",
     )
 )
```

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/conf.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/read.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/run.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/stamp.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/switch.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/_commands/write.py` & `idefix_cli-2.3.3/src/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli/lib.py` & `idefix_cli-2.3.3/src/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/src/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idefix-cli
-Version: 2.3.2
+Name: idefix_cli
+Version: 2.3.3
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-2.3.2/src/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.3.3/src/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_app_structure.py` & `idefix_cli-2.3.3/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_clean.py` & `idefix_cli-2.3.3/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_clone.py` & `idefix_cli-2.3.3/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_commons.py` & `idefix_cli-2.3.3/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_conf.py` & `idefix_cli-2.3.3/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_read.py` & `idefix_cli-2.3.3/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_run.py` & `idefix_cli-2.3.3/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_stamp.py` & `idefix_cli-2.3.3/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_ux.py` & `idefix_cli-2.3.3/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.2/tests/test_write.py` & `idefix_cli-2.3.3/tests/test_write.py`

 * *Files identical despite different names*

