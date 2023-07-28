# Comparing `tmp/code_data_science-1.1.0.tar.gz` & `tmp/code_data_science-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_science-1.1.0.tar", last modified: Fri Jul 28 18:19:35 2023, max compression
+gzip compressed data, was "code_data_science-1.1.1.tar", last modified: Fri Jul 28 19:40:23 2023, max compression
```

## Comparing `code_data_science-1.1.0.tar` & `code_data_science-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.742563 code_data_science-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 18:19:35.742563 code_data_science-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-28 18:19:16.000000 code_data_science-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.734562 code_data_science-1.1.0/code_data_science/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.742563 code_data_science-1.1.0/code_data_science/clustering_src/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/datasets_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/hf_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/index_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/moderne_data_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/moderne_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/scm_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/sort_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.738563 code_data_science-1.1.0/code_data_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-28 18:19:16.000000 code_data_science-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:19:35.742563 code_data_science-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:40:23.630113 code_data_science-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:40:23.630113 code_data_science-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-28 19:40:06.000000 code_data_science-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:40:23.630113 code_data_science-1.1.1/code_data_science/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:40:23.630113 code_data_science-1.1.1/code_data_science/clustering_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/datasets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/hf_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/clustering_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/index_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/moderne_data_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/moderne_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/read_data_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/scm_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-28 19:40:06.000000 code_data_science-1.1.1/code_data_science/sort_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:40:23.630113 code_data_science-1.1.1/code_data_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:40:23.000000 code_data_science-1.1.1/code_data_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-28 19:40:23.000000 code_data_science-1.1.1/code_data_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:40:23.000000 code_data_science-1.1.1/code_data_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 19:40:23.000000 code_data_science-1.1.1/code_data_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:40:23.000000 code_data_science-1.1.1/code_data_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-28 19:40:06.000000 code_data_science-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:40:23.630113 code_data_science-1.1.1/setup.cfg
```

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/datasets_loader.py` & `code_data_science-1.1.1/code_data_science/clustering_src/datasets_loader.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/distributed_utils.py` & `code_data_science-1.1.1/code_data_science/clustering_src/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/hf_trainer.py` & `code_data_science-1.1.1/code_data_science/clustering_src/hf_trainer.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/logging_callback.py` & `code_data_science-1.1.1/code_data_science/clustering_src/logging_callback.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/preprocessing_utils.py` & `code_data_science-1.1.1/code_data_science/clustering_src/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/training_args.py` & `code_data_science-1.1.1/code_data_science/clustering_src/training_args.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/clustering_src/utils.py` & `code_data_science-1.1.1/code_data_science/clustering_src/utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/moderne_data_grid.py` & `code_data_science-1.1.1/code_data_science/moderne_data_grid.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/moderne_palette.py` & `code_data_science-1.1.1/code_data_science/moderne_palette.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/scm_link.py` & `code_data_science-1.1.1/code_data_science/scm_link.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science/sort_versions.py` & `code_data_science-1.1.1/code_data_science/sort_versions.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.1.0/code_data_science.egg-info/SOURCES.txt` & `code_data_science-1.1.1/code_data_science.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 README.rst
 pyproject.toml
 code_data_science/__init__.py
-code_data_science/data_table.py
 code_data_science/index_versions.py
 code_data_science/moderne_data_grid.py
 code_data_science/moderne_palette.py
+code_data_science/read_data_table.py
 code_data_science/scm_link.py
 code_data_science/sort_versions.py
 code_data_science.egg-info/PKG-INFO
 code_data_science.egg-info/SOURCES.txt
 code_data_science.egg-info/dependency_links.txt
 code_data_science.egg-info/requires.txt
 code_data_science.egg-info/top_level.txt
```

### Comparing `code_data_science-1.1.0/pyproject.toml` & `code_data_science-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "code_data_science"
-version = "1.1.0"
+version = "1.1.1"
 description = "A python implementation of various tools used in code data science."
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io"},
     { name = "Kyle Scully", email = "kyle@moderne.io"}
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

