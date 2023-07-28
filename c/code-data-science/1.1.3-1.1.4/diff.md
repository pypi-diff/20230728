# Comparing `tmp/code_data_science-1.1.3.tar.gz` & `tmp/code_data_science-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_science-1.1.3.tar", last modified: Fri Jul 28 19:55:48 2023, max compression
+gzip compressed data, was "code_data_science-1.1.4.tar", last modified: Fri Jul 28 19:57:01 2023, max compression
```

## Comparing `code_data_science-1.1.3.tar` & `code_data_science-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:55:48.678045 code_data_science-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:55:48.678045 code_data_science-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-28 19:55:23.000000 code_data_science-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:55:48.674045 code_data_science-1.1.3/code_data_science/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:55:48.678045 code_data_science-1.1.3/code_data_science/clustering_src/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/datasets_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/hf_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/clustering_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/moderne_data_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/moderne_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/scm_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-28 19:55:23.000000 code_data_science-1.1.3/code_data_science/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:55:48.674045 code_data_science-1.1.3/code_data_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:55:48.000000 code_data_science-1.1.3/code_data_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-28 19:55:48.000000 code_data_science-1.1.3/code_data_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:55:48.000000 code_data_science-1.1.3/code_data_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 19:55:48.000000 code_data_science-1.1.3/code_data_science.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:55:48.000000 code_data_science-1.1.3/code_data_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-28 19:55:23.000000 code_data_science-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:55:48.678045 code_data_science-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:57:01.888242 code_data_science-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:57:01.888242 code_data_science-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-28 19:56:39.000000 code_data_science-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:57:01.884242 code_data_science-1.1.4/code_data_science/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:57:01.888242 code_data_science-1.1.4/code_data_science/clustering_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/datasets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/hf_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/clustering_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/data_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/data_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/scm_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-28 19:56:39.000000 code_data_science-1.1.4/code_data_science/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:57:01.888242 code_data_science-1.1.4/code_data_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:57:01.000000 code_data_science-1.1.4/code_data_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-28 19:57:01.000000 code_data_science-1.1.4/code_data_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:57:01.000000 code_data_science-1.1.4/code_data_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 19:57:01.000000 code_data_science-1.1.4/code_data_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:57:01.000000 code_data_science-1.1.4/code_data_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-28 19:56:39.000000 code_data_science-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:57:01.888242 code_data_science-1.1.4/setup.cfg
```

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/datasets_loader.py` & `code_data_science-1.1.4/code_data_science/clustering_src/datasets_loader.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/distributed_utils.py` & `code_data_science-1.1.4/code_data_science/clustering_src/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/hf_trainer.py` & `code_data_science-1.1.4/code_data_science/clustering_src/hf_trainer.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/logging_callback.py` & `code_data_science-1.1.4/code_data_science/clustering_src/logging_callback.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/preprocessing_utils.py` & `code_data_science-1.1.4/code_data_science/clustering_src/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/training_args.py` & `code_data_science-1.1.4/code_data_science/clustering_src/training_args.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/clustering_src/utils.py` & `code_data_science-1.1.4/code_data_science/clustering_src/utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/moderne_data_grid.py` & `code_data_science-1.1.4/code_data_science/data_grid.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/moderne_palette.py` & `code_data_science-1.1.4/code_data_science/palette.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/scm_link.py` & `code_data_science-1.1.4/code_data_science/scm_link.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science/versions.py` & `code_data_science-1.1.4/code_data_science/versions.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.3/code_data_science.egg-info/SOURCES.txt` & `code_data_science-1.1.4/code_data_science.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 README.rst
 pyproject.toml
 code_data_science/__init__.py
+code_data_science/data_grid.py
 code_data_science/data_table.py
-code_data_science/moderne_data_grid.py
-code_data_science/moderne_palette.py
+code_data_science/palette.py
 code_data_science/scm_link.py
 code_data_science/versions.py
 code_data_science.egg-info/PKG-INFO
 code_data_science.egg-info/SOURCES.txt
 code_data_science.egg-info/dependency_links.txt
 code_data_science.egg-info/requires.txt
 code_data_science.egg-info/top_level.txt
```

### Comparing `code_data_science-1.1.3/pyproject.toml` & `code_data_science-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "code_data_science"
-version = "1.1.3"
+version = "1.1.4"
 description = "A python implementation of various tools used in code data science."
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io"},
     { name = "Kyle Scully", email = "kyle@moderne.io"}
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

