# Comparing `tmp/cat_data_tools-0.4.0.tar.gz` & `tmp/cat_data_tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cat_data_tools-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cat_data_tools-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cat_data_tools-0.4.0.tar` & `cat_data_tools-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      353 2023-07-28 17:34:25.893442 cat_data_tools-0.4.0/README.md
--rw-r--r--   0        0        0      102 2023-07-28 17:34:25.893442 cat_data_tools-0.4.0/cat_data_tools/__init__.py
--rw-r--r--   0        0        0       76 2023-07-28 17:34:25.893442 cat_data_tools-0.4.0/cat_data_tools/transformations.py
--rw-r--r--   0        0        0      436 2023-07-28 17:34:25.893442 cat_data_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 cat_data_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/README.md
+-rw-r--r--   0        0        0      125 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/cat_data_tools/__init__.py
+-rw-r--r--   0        0        0      670 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/cat_data_tools/cli.py
+-rw-r--r--   0        0        0      788 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/cat_data_tools/filter_data_by_month.py
+-rw-r--r--   0        0        0      475 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 cat_data_tools-0.4.1/PKG-INFO
```

### Comparing `cat_data_tools-0.4.0/PKG-INFO` & `cat_data_tools-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: cat_data_tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/cat_data_tools
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: typer
 
 # Cat data tools <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 
 [![codecov](https://codecov.io/gh/IslasGECI/cat_data_tools/branch/develop/graph/badge.svg?token=MvLBzyGSH3)](https://codecov.io/gh/IslasGECI/cat_data_tools)
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: cat_data_tools Version: 0.4.0 Summary: A template
+Metadata-Version: 2.1 Name: cat_data_tools Version: 0.4.1 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/cat_data_tools Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
-OSI Approved :: GNU General Public License v3 or later (GPLv3+) # Cat data
-tools [https://www.islas.org.mx/img/logo.svg] [![codecov](https://codecov.io/
-gh/IslasGECI/cat_data_tools/branch/develop/graph/badge.svg?token=MvLBzyGSH3)]
-(https://codecov.io/gh/IslasGECI/cat_data_tools) ## Overview Python module with
-tools to process cat data.
+OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
+numpy Requires-Dist: pandas Requires-Dist: typer # Cat data tools [https://
+www.islas.org.mx/img/logo.svg] [![codecov](https://codecov.io/gh/IslasGECI/
+cat_data_tools/branch/develop/graph/badge.svg?token=MvLBzyGSH3)](https://
+codecov.io/gh/IslasGECI/cat_data_tools) ## Overview Python module with tools to
+process cat data.
```

