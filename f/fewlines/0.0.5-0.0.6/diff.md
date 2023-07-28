# Comparing `tmp/fewlines-0.0.5.tar.gz` & `tmp/fewlines-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fewlines-0.0.5.tar", last modified: Tue Jul 25 01:28:54 2023, max compression
+gzip compressed data, was "fewlines-0.0.6.tar", last modified: Fri Jul 28 15:34:59 2023, max compression
```

## Comparing `fewlines-0.0.5.tar` & `fewlines-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:54.048626 fewlines-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-25 01:28:42.000000 fewlines-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 01:28:54.048626 fewlines-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-25 01:28:42.000000 fewlines-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:54.044626 fewlines-0.0.5/fewlines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:42.000000 fewlines-0.0.5/fewlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-25 01:28:42.000000 fewlines-0.0.5/fewlines/horizon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:54.044626 fewlines-0.0.5/fewlines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:28:54.048626 fewlines-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-25 01:28:42.000000 fewlines-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:59.973583 fewlines-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-28 15:34:48.000000 fewlines-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 15:34:59.969583 fewlines-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-28 15:34:48.000000 fewlines-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:59.969583 fewlines-0.0.6/fewlines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:48.000000 fewlines-0.0.6/fewlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-28 15:34:48.000000 fewlines-0.0.6/fewlines/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-28 15:34:48.000000 fewlines-0.0.6/fewlines/horizon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:59.969583 fewlines-0.0.6/fewlines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 15:34:59.000000 fewlines-0.0.6/fewlines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 15:34:59.000000 fewlines-0.0.6/fewlines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:34:59.000000 fewlines-0.0.6/fewlines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 15:34:59.000000 fewlines-0.0.6/fewlines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:34:59.973583 fewlines-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-28 15:34:48.000000 fewlines-0.0.6/setup.py
```

### Comparing `fewlines-0.0.5/LICENSE` & `fewlines-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fewlines-0.0.5/README.md` & `fewlines-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fewlines-0.0.5/fewlines/horizon.py` & `fewlines-0.0.6/fewlines/horizon.py`

 * *Files identical despite different names*

