# Comparing `tmp/codingtoolkit-0.0.2.tar.gz` & `tmp/codingtoolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codingtoolkit-0.0.2.tar", last modified: Fri Jul 28 06:58:07 2023, max compression
+gzip compressed data, was "codingtoolkit-0.0.3.tar", last modified: Fri Jul 28 07:07:49 2023, max compression
```

## Comparing `codingtoolkit-0.0.2.tar` & `codingtoolkit-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kellen     (504) staff       (20)        0 2023-07-28 06:58:07.062339 codingtoolkit-0.0.2/
-drwxr-xr-x   0 kellen     (504) staff       (20)        0 2023-07-28 06:58:07.059621 codingtoolkit-0.0.2/CodingToolKit.egg-info/
--rw-r--r--   0 kellen     (504) staff       (20)      613 2023-07-28 06:58:06.000000 codingtoolkit-0.0.2/CodingToolKit.egg-info/PKG-INFO
--rw-r--r--   0 kellen     (504) staff       (20)      363 2023-07-28 06:58:06.000000 codingtoolkit-0.0.2/CodingToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 kellen     (504) staff       (20)        1 2023-07-28 06:58:06.000000 codingtoolkit-0.0.2/CodingToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 kellen     (504) staff       (20)       14 2023-07-28 06:58:06.000000 codingtoolkit-0.0.2/CodingToolKit.egg-info/top_level.txt
--rw-r--r--   0 kellen     (504) staff       (20)      613 2023-07-28 06:58:07.061999 codingtoolkit-0.0.2/PKG-INFO
--rw-r--r--   0 kellen     (504) staff       (20)       15 2023-07-28 06:43:59.000000 codingtoolkit-0.0.2/README.md
-drwxr-xr-x   0 kellen     (504) staff       (20)        0 2023-07-28 06:58:07.060976 codingtoolkit-0.0.2/codingtoolkit/
--rw-r--r--   0 kellen     (504) staff       (20)       50 2023-07-28 06:55:16.000000 codingtoolkit-0.0.2/codingtoolkit/__init__.py
--rw-r--r--   0 kellen     (504) staff       (20)     1498 2023-07-28 06:55:18.000000 codingtoolkit-0.0.2/codingtoolkit/flags.py
--rw-r--r--   0 kellen     (504) staff       (20)       38 2023-07-28 06:58:07.062484 codingtoolkit-0.0.2/setup.cfg
--rw-r--r--   0 kellen     (504) staff       (20)     1063 2023-07-28 06:55:15.000000 codingtoolkit-0.0.2/setup.py
+drwxr-xr-x   0 kellen     (504) staff       (20)        0 2023-07-28 07:07:49.492037 codingtoolkit-0.0.3/
+drwxr-xr-x   0 kellen     (504) staff       (20)        0 2023-07-28 07:07:49.489212 codingtoolkit-0.0.3/CodingToolKit.egg-info/
+-rw-r--r--   0 kellen     (504) staff       (20)      613 2023-07-28 07:07:49.000000 codingtoolkit-0.0.3/CodingToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 kellen     (504) staff       (20)      363 2023-07-28 07:07:49.000000 codingtoolkit-0.0.3/CodingToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 kellen     (504) staff       (20)        1 2023-07-28 07:07:49.000000 codingtoolkit-0.0.3/CodingToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 kellen     (504) staff       (20)       14 2023-07-28 07:07:49.000000 codingtoolkit-0.0.3/CodingToolKit.egg-info/top_level.txt
+-rw-r--r--   0 kellen     (504) staff       (20)      613 2023-07-28 07:07:49.491681 codingtoolkit-0.0.3/PKG-INFO
+-rw-r--r--   0 kellen     (504) staff       (20)       15 2023-07-28 06:43:59.000000 codingtoolkit-0.0.3/README.md
+drwxr-xr-x   0 kellen     (504) staff       (20)        0 2023-07-28 07:07:49.490638 codingtoolkit-0.0.3/codingtoolkit/
+-rw-r--r--   0 kellen     (504) staff       (20)       52 2023-07-28 07:06:50.000000 codingtoolkit-0.0.3/codingtoolkit/__init__.py
+-rw-r--r--   0 kellen     (504) staff       (20)     1498 2023-07-28 07:01:42.000000 codingtoolkit-0.0.3/codingtoolkit/flags.py
+-rw-r--r--   0 kellen     (504) staff       (20)       38 2023-07-28 07:07:49.492158 codingtoolkit-0.0.3/setup.cfg
+-rw-r--r--   0 kellen     (504) staff       (20)     1063 2023-07-28 07:07:42.000000 codingtoolkit-0.0.3/setup.py
```

### Comparing `codingtoolkit-0.0.2/CodingToolKit.egg-info/PKG-INFO` & `codingtoolkit-0.0.3/CodingToolKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: codingtoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A coding toolkit for python
 Home-page: UNKNOWN
 Author: flyingreshin
 Author-email: flyingreshin@gmail.com
 License: UNKNOWN
 Description: This toolkit contains useful packages to make writing pyhton prograsms easier
 Keywords: python,first package
```

### Comparing `codingtoolkit-0.0.2/PKG-INFO` & `codingtoolkit-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: codingtoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A coding toolkit for python
 Home-page: UNKNOWN
 Author: flyingreshin
 Author-email: flyingreshin@gmail.com
 License: UNKNOWN
 Description: This toolkit contains useful packages to make writing pyhton prograsms easier
 Keywords: python,first package
```

### Comparing `codingtoolkit-0.0.2/codingtoolkit/flags.py` & `codingtoolkit-0.0.3/codingtoolkit/flags.py`

 * *Files identical despite different names*

### Comparing `codingtoolkit-0.0.2/setup.py` & `codingtoolkit-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'A coding toolkit for python'
 LONG_DESCRIPTION = 'This toolkit contains useful packages to make writing pyhton prograsms easier'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="codingtoolkit",
```

