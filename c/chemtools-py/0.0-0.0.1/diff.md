# Comparing `tmp/chemtools-py-0.0.tar.gz` & `tmp/chemtools-py-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemtools-py-0.0.tar", last modified: Fri Jul 28 06:28:06 2023, max compression
+gzip compressed data, was "chemtools-py-0.0.1.tar", last modified: Fri Jul 28 06:39:59 2023, max compression
```

## Comparing `chemtools-py-0.0.tar` & `chemtools-py-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 06:28:06.875335 chemtools-py-0.0/
--rw-rw-rw-   0        0        0      315 2023-07-28 06:28:06.875335 chemtools-py-0.0/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-07-24 15:38:57.000000 chemtools-py-0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 06:28:06.859331 chemtools-py-0.0/chemtools-py/
--rw-rw-rw-   0        0        0      117 2023-07-28 05:34:11.000000 chemtools-py-0.0/chemtools-py/__init__.py
--rw-rw-rw-   0        0        0     3299 2023-07-24 12:01:49.000000 chemtools-py-0.0/chemtools-py/funclib.py
-drwxrwxrwx   0        0        0        0 2023-07-28 06:28:06.874335 chemtools-py-0.0/chemtools_py.egg-info/
--rw-rw-rw-   0        0        0      315 2023-07-28 06:28:06.000000 chemtools-py-0.0/chemtools_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-07-28 06:28:06.000000 chemtools-py-0.0/chemtools_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 06:28:06.000000 chemtools-py-0.0/chemtools_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-28 06:28:06.000000 chemtools-py-0.0/chemtools_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 06:28:06.000000 chemtools-py-0.0/chemtools_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 06:28:06.876336 chemtools-py-0.0/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-07-28 06:25:21.000000 chemtools-py-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:39:59.942756 chemtools-py-0.0.1/
+-rw-rw-rw-   0        0        0      317 2023-07-28 06:39:59.942756 chemtools-py-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-07-24 15:38:57.000000 chemtools-py-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 06:39:59.931752 chemtools-py-0.0.1/chemtools-py/
+-rw-rw-rw-   0        0        0      117 2023-07-28 05:34:11.000000 chemtools-py-0.0.1/chemtools-py/__init__.py
+-rw-rw-rw-   0        0        0     3299 2023-07-24 12:01:49.000000 chemtools-py-0.0.1/chemtools-py/funclib.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:39:59.940754 chemtools-py-0.0.1/chemtools_py.egg-info/
+-rw-rw-rw-   0        0        0      317 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 06:39:59.942756 chemtools-py-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-07-28 06:39:52.000000 chemtools-py-0.0.1/setup.py
```

### Comparing `chemtools-py-0.0/chemtools-py/funclib.py` & `chemtools-py-0.0.1/chemtools-py/funclib.py`

 * *Files identical despite different names*

