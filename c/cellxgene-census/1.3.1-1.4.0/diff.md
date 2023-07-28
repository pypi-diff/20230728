# Comparing `tmp/cellxgene_census-1.3.1.tar.gz` & `tmp/cellxgene_census-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.3.1.tar", last modified: Thu Jul 20 01:12:29 2023, max compression
+gzip compressed data, was "cellxgene_census-1.4.0.tar", last modified: Fri Jul 28 18:35:37 2023, max compression
```

## Comparing `cellxgene_census-1.3.1.tar` & `cellxgene_census-1.4.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.248885 cellxgene_census-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-20 01:12:29.248885 cellxgene_census-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.236885 cellxgene_census-1.3.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:12:29.248885 cellxgene_census-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.232885 cellxgene_census-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.236885 cellxgene_census-1.3.1/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.240885 cellxgene_census-1.3.1/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.240885 cellxgene_census-1.3.1/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.244886 cellxgene_census-1.3.1/src/cellxgene_census/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14770 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/pp/_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.244886 cellxgene_census-1.3.1/src/cellxgene_census/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/util/_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/src/cellxgene_census/experimental/util/_eager_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.240885 cellxgene_census-1.3.1/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-20 01:12:29.000000 cellxgene_census-1.3.1/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-20 01:12:29.000000 cellxgene_census-1.3.1/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:12:29.000000 cellxgene_census-1.3.1/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 01:12:29.000000 cellxgene_census-1.3.1/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 01:12:29.000000 cellxgene_census-1.3.1/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.244886 cellxgene_census-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    39660 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.244886 cellxgene_census-1.3.1/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.244886 cellxgene_census-1.3.1/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/experimental/ml/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.248885 cellxgene_census-1.3.1/tests/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/experimental/pp/test_hvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/experimental/pp/test_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:12:29.248885 cellxgene_census-1.3.1/tests/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/experimental/util/test_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-20 01:12:10.000000 cellxgene_census-1.3.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.654118 cellxgene_census-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_eager_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56048 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/pp/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/pp/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/tests/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/util/test_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_util.py
```

### Comparing `cellxgene_census-1.3.1/LICENSE` & `cellxgene_census-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/PKG-INFO` & `cellxgene_census-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.3.1
+Version: 1.4.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.3.1/README.md` & `cellxgene_census-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/pyproject.toml` & `cellxgene_census-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/release_process.md` & `cellxgene_census-1.4.0/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/__init__.py` & `cellxgene_census-1.4.0/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.4.0/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.4.0/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/_open.py` & `cellxgene_census-1.4.0/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.4.0/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.4.0/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py` & `cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         mvn = MeanVarianceAccumulator(n_batches, n_samples, query.n_vars)
         for arrow_tbl in _EagerIterator(query.X(layer).tables(), pool=pool):
             data = arrow_tbl["soma_data"].to_numpy()
             if batch_indexer:
                 _batch_take_at_future = pool.submit(batch_indexer, arrow_tbl["soma_dim_0"])
                 var_dim = var_indexer.by_var(arrow_tbl["soma_dim_1"])
                 _batch_vec = batch_codes[_batch_take_at_future.result()]
-                mvn.update_by_batch(_batch_vec, var_dim, data)
+                mvn.update(var_dim, data, _batch_vec)
             else:
                 var_dim = var_indexer.by_var(arrow_tbl["soma_dim_1"])
-                mvn.update_single_batch(var_dim, data)
+                mvn.update(var_dim, data)
 
         batches_u, batches_var, all_u, all_var = mvn.finalize()
         del mvn
 
     var_df = pd.DataFrame(
         index=pd.Index(data=query.var_joinids(), name="soma_joinid"),
         data={
@@ -154,18 +154,18 @@
         acc = CountsAccumulator(n_batches, query.n_vars, clip_val)
         for arrow_tbl in _EagerIterator(query.X(layer).tables(), pool=pool):
             data = arrow_tbl["soma_data"].to_numpy()
             if batch_indexer:
                 _batch_take_at_future = pool.submit(batch_indexer, arrow_tbl["soma_dim_0"])
                 var_dim = var_indexer.by_var(arrow_tbl["soma_dim_1"])
                 _batch_vec = batch_codes[_batch_take_at_future.result()]
-                acc.update_by_batch(_batch_vec, var_dim, data)
+                acc.update(var_dim, data, _batch_vec)
             else:
                 var_dim = var_indexer.by_var(arrow_tbl["soma_dim_1"])
-                acc.update_single_batch(var_dim, data)
+                acc.update(var_dim, data)
 
         counts_sum, squared_counts_sum = acc.finalize()
         norm_gene_vars = (1 / ((n_samples - 1) * np.square(reg_std.T))).T * (
             (n_samples * np.square(batches_u.T)).T + squared_counts_sum - 2 * counts_sum * batches_u
         )
         del acc, counts_sum, squared_counts_sum
```

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/experimental/pp/_online.py` & `cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_online.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Optional, Tuple
 
 import numba
 import numpy as np
 import numpy.typing as npt
 
 
 class MeanVarianceAccumulator:
@@ -14,70 +14,100 @@
 
     References:
         https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance
     and
         Knuth, Art of Computer Programming, volume II
     """
 
-    def __init__(self, n_batches: int, n_samples: npt.NDArray[np.int64], n_variables: int):
+    def __init__(self, n_batches: int, n_samples: npt.NDArray[np.int64], n_variables: int, ddof: int = 1):
         if n_samples.sum() <= 0:
             raise ValueError("No samples provided - can't calculate mean or variance.")
 
+        self.ddof = ddof
         self.n_batches = n_batches
         self.n_samples = n_samples
         self.n = np.zeros((n_batches, n_variables), dtype=np.int32)
         self.u = np.zeros((n_batches, n_variables), dtype=np.float64)
         self.M2 = np.zeros((n_batches, n_variables), dtype=np.float64)
 
-    def update_by_batch(
-        self, batch_vec: npt.NDArray[np.int64], var_vec: npt.NDArray[np.int64], val_vec: npt.NDArray[np.float32]
+    def update(
+        self,
+        var_vec: npt.NDArray[np.int64],
+        val_vec: npt.NDArray[np.float32],
+        batch_vec: Optional[npt.NDArray[np.int64]] = None,
     ) -> None:
-        _mbomv_update_by_batch(batch_vec, var_vec, val_vec, self.n, self.u, self.M2)
-
-    def update_single_batch(self, var_vec: npt.NDArray[np.int64], val_vec: npt.NDArray[np.float32]) -> None:
-        assert self.n_batches == 1
-        _mbomv_update_single_batch(var_vec, val_vec, self.n, self.u, self.M2)
+        if self.n_batches == 1:
+            assert batch_vec is None
+            _mbomv_update_single_batch(var_vec, val_vec, self.n, self.u, self.M2)
+        else:
+            assert batch_vec is not None
+            _mbomv_update_by_batch(batch_vec, var_vec, val_vec, self.n, self.u, self.M2)
 
     def finalize(
         self,
     ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64], npt.NDArray[np.float64], npt.NDArray[np.float64]]:
-        # TODO: do we want to add ddof param?  Currently hard-wired to 1 (see var calcs)
-
         # correct each batch to account for sparsity
         _mbomv_sparse_correct_batches(self.n_batches, self.n_samples, self.n, self.u, self.M2)
 
         # compute u, var for each batch
         batches_u = self.u
-        batches_var = (self.M2.T / (self.n_samples - 1)).T
+
+        # Note: if N-ddof is less than or equal to 0, we will return Inf - this is consistent
+        # with the numpy.var behavior.
+        with np.errstate(divide="ignore"):
+            batches_var = (self.M2.T / np.maximum(0, (self.n_samples - self.ddof))).T
 
         # accum all batches using Chan's
         all_u, all_M2 = _mbomv_combine_batches(self.n_batches, self.n_samples, self.u, self.M2)
-        all_var = all_M2 / max(1, (self.n_samples.sum() - 1))
+        with np.errstate(divide="ignore"):
+            all_var = all_M2 / max(0, (self.n_samples.sum() - self.ddof))
 
         return batches_u, batches_var, all_u, all_var
 
 
+class MeanAccumulator:
+    def __init__(self, n_samples: int, n_variables: int):
+        if n_samples <= 0:
+            raise ValueError("No samples provided - can't calculate mean.")
+
+        if n_variables <= 0:
+            raise ValueError("No variables provided - can't calculate mean.")
+
+        self.u = np.zeros(n_variables, dtype=np.float64)
+        self.n_samples = n_samples
+
+    def update(self, var_vec: npt.NDArray[np.int64], val_vec: npt.NDArray[np.float32]) -> None:
+        _update_mean_vector(self.u, var_vec, val_vec)
+
+    def finalize(self) -> npt.NDArray[np.float64]:
+        return self.u / self.n_samples
+
+
 class CountsAccumulator:
     def __init__(self, n_batches: int, n_variables: int, clip_val: npt.NDArray[np.float64]):
         self.n_batches = n_batches
         self.n_variables = n_variables
         self.clip_val = clip_val
         self.counts_sum = np.zeros((n_batches, n_variables), dtype=np.float64)  # clipped
         self.squared_counts_sum = np.zeros((n_batches, n_variables), dtype=np.float64)  # clipped
 
-    def update_by_batch(
-        self, batch_vec: npt.NDArray[np.int64], var_vec: npt.NDArray[np.int64], val_vec: npt.NDArray[np.float32]
+    def update(
+        self,
+        var_vec: npt.NDArray[np.int64],
+        val_vec: npt.NDArray[np.float32],
+        batch_vec: Optional[npt.NDArray[np.int64]] = None,
     ) -> None:
-        _accum_clipped_counts_by_batch(
-            self.counts_sum, self.squared_counts_sum, batch_vec, var_vec, val_vec, self.clip_val
-        )
-
-    def update_single_batch(self, var_vec: npt.NDArray[np.int64], val_vec: npt.NDArray[np.float32]) -> None:
-        assert self.n_batches == 1
-        _accum_clipped_counts(self.counts_sum[0], self.squared_counts_sum[0], var_vec, val_vec, self.clip_val[0])
+        if self.n_batches == 1:
+            assert batch_vec is None
+            _accum_clipped_counts(self.counts_sum[0], self.squared_counts_sum[0], var_vec, val_vec, self.clip_val[0])
+        else:
+            assert batch_vec is not None
+            _accum_clipped_counts_by_batch(
+                self.counts_sum, self.squared_counts_sum, batch_vec, var_vec, val_vec, self.clip_val
+            )
 
     def finalize(self) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
         return self.counts_sum, self.squared_counts_sum
 
 
 """
 Private performance related top-level functions.
@@ -126,21 +156,30 @@
         M2_prev = M2[batch, col]
         n[batch, col] += 1
         u[batch, col] = u_prev + (val - u_prev) / n[batch, col]
         M2[batch, col] = M2_prev + (val - u_prev) * (val - u[batch, col])
 
 
 @numba.jit(
-    numba.void(
-        numba.types.Array(numba.int64, 1, "C", readonly=True),
-        numba.types.Array(numba.float32, 1, "C", readonly=True),
-        numba.int32[:, :],
-        numba.float64[:, :],
-        numba.float64[:, :],
-    ),
+    [
+        numba.void(
+            numba.types.Array(numba.int32, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+            numba.int32[:, :],
+            numba.float64[:, :],
+            numba.float64[:, :],
+        ),
+        numba.void(
+            numba.types.Array(numba.int64, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+            numba.int32[:, :],
+            numba.float64[:, :],
+            numba.float64[:, :],
+        ),
+    ],
     nopython=True,
     nogil=True,
 )  # type: ignore[misc]  # See https://github.com/numba/numba/issues/7424
 def _mbomv_update_single_batch(
     var_vec: npt.NDArray[np.int64],
     val_vec: npt.NDArray[np.float32],
     n: npt.NDArray[np.int32],
@@ -228,21 +267,30 @@
         acc_u = _u
         acc_M2 = _M2
 
     return acc_u, acc_M2
 
 
 @numba.jit(
-    numba.void(
-        numba.float64[:],
-        numba.float64[:],
-        numba.types.Array(numba.int64, 1, "C", readonly=True),
-        numba.types.Array(numba.float32, 1, "C", readonly=True),
-        numba.float64[:],
-    ),
+    [
+        numba.void(
+            numba.float64[:],
+            numba.float64[:],
+            numba.types.Array(numba.int32, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+            numba.float64[:],
+        ),
+        numba.void(
+            numba.float64[:],
+            numba.float64[:],
+            numba.types.Array(numba.int64, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+            numba.float64[:],
+        ),
+    ],
     nopython=True,
     nogil=True,
 )  # type: ignore[misc]  # See https://github.com/numba/numba/issues/7424
 def _accum_clipped_counts(
     counts_sum: npt.NDArray[np.float64],
     squared_counts_sum: npt.NDArray[np.float64],
     var_dim: npt.NDArray[np.int64],
@@ -253,22 +301,32 @@
         if val > clip_val[col]:
             val = clip_val[col]
         counts_sum[col] += val
         squared_counts_sum[col] += val**2
 
 
 @numba.jit(
-    numba.void(
-        numba.float64[:, :],
-        numba.float64[:, :],
-        numba.int64[:],
-        numba.types.Array(numba.int64, 1, "C", readonly=True),
-        numba.types.Array(numba.float32, 1, "C", readonly=True),
-        numba.float64[:, :],
-    ),
+    [
+        numba.void(
+            numba.float64[:, :],
+            numba.float64[:, :],
+            numba.int64[:],
+            numba.types.Array(numba.int32, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+            numba.float64[:, :],
+        ),
+        numba.void(
+            numba.float64[:, :],
+            numba.float64[:, :],
+            numba.int64[:],
+            numba.types.Array(numba.int64, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+            numba.float64[:, :],
+        ),
+    ],
     nopython=True,
     nogil=True,
 )  # type: ignore[misc]  # See https://github.com/numba/numba/issues/7424
 def _accum_clipped_counts_by_batch(
     counts_sum: npt.NDArray[np.float64],
     squared_counts_sum: npt.NDArray[np.float64],
     batch: npt.NDArray[np.int64],
@@ -277,7 +335,32 @@
     clip_val: npt.NDArray[np.float64],
 ) -> None:
     for bid, col, val in zip(batch, var_dim, data):
         if val > clip_val[bid, col]:
             val = clip_val[bid, col]
         counts_sum[bid, col] += val
         squared_counts_sum[bid, col] += val**2
+
+
+@numba.jit(
+    [
+        numba.void(
+            numba.float64[:],
+            numba.types.Array(numba.int32, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+        ),
+        numba.void(
+            numba.float64[:],
+            numba.types.Array(numba.int64, 1, "C", readonly=True),
+            numba.types.Array(numba.float32, 1, "C", readonly=True),
+        ),
+    ],
+    nopython=True,
+    nogil=True,
+)  # type: ignore[misc]  # See https://github.com/numba/numba/issues/7424
+def _update_mean_vector(
+    u: npt.NDArray[np.float64],
+    var_vec: npt.NDArray[np.int64],
+    val_vec: npt.NDArray[np.float32],
+) -> None:
+    for col, val in zip(var_vec, val_vec):
+        u[col] = u[col] + val
```

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/experimental/util/_csr_iter.py` & `cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census/experimental/util/_eager_iter.py` & `cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.4.0/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.3.1
+Version: 1.4.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.3.1/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.4.0/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/cellxgene_census.egg-info/top_level.txt
 src/cellxgene_census/experimental/__init__.py
 src/cellxgene_census/experimental/ml/__init__.py
 src/cellxgene_census/experimental/ml/pytorch.py
 src/cellxgene_census/experimental/pp/__init__.py
 src/cellxgene_census/experimental/pp/_highly_variable_genes.py
 src/cellxgene_census/experimental/pp/_online.py
+src/cellxgene_census/experimental/pp/_stats.py
 src/cellxgene_census/experimental/util/__init__.py
 src/cellxgene_census/experimental/util/_csr_iter.py
 src/cellxgene_census/experimental/util/_eager_iter.py
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/test_acceptance.py
@@ -34,8 +35,9 @@
 tests/test_open.py
 tests/test_util.py
 tests/experimental/__init__.py
 tests/experimental/ml/__init__.py
 tests/experimental/ml/test_pytorch.py
 tests/experimental/pp/test_hvg.py
 tests/experimental/pp/test_online.py
+tests/experimental/pp/test_stats.py
 tests/experimental/util/test_csr_iter.py
```

### Comparing `cellxgene_census-1.3.1/tests/README.md` & `cellxgene_census-1.4.0/tests/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -41,25 +41,210 @@
 These tests are periodically run, and are not part of CI due to their overhead.
 
 When run, please record the results in this file (below) and commit the change to git. Please include the following information:
 
 - date
 - config:
   - EC2 instance type and any system config (i.e., swap)
-  - host and OS as reported by `uname -a`
+  - host and OS as reported by `uname -a`. **Please remove IP address**
   - Python & package versions and OS - suggest capturing the output of `tiledbsoma.show_package_versions()`
   - The Census version used for the test (i.e., the version aliased as `latest`). This can be easily captured using `cellxgene_census.get_census_version_description('latest')`
   - the cellxgene_census package version (ie., `cellxgene_census.__version__`)
 - any run notes
 - full output of: `pytest -v --durations=0 --expensive ./api/python/cellxgene_census/tests/`
 
+## 2023-07-26
+
+- Host: EC2 instance type: `r6id.32xlarge`, all nvme mounted as swap.
+- Uname: Linux 5.19.0-1028-aws #29~22.04.1-Ubuntu SMP Tue Jun 20 19:12:11 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
+- Python & census versions:
+
+```
+>>> import cellxgene_census, tiledbsoma
+>>> tiledbsoma.show_package_versions()
+tiledbsoma.__version__        1.2.7
+TileDB-Py tiledb.version()    (0, 21, 3)
+TileDB core version           2.15.2
+libtiledbsoma version()       libtiledb=2.15.2
+python version                3.10.6.final.0
+OS version                    Linux 5.19.0-1028-aws
+```
+
+**Pytest output:**
+
+```
+============================= test session starts ==============================
+platform linux -- Python 3.10.6, pytest-7.1.3, pluggy-1.0.0 -- /home/ubuntu/venv/bin/python
+cachedir: .pytest_cache
+rootdir: /home/ubuntu/repos/cellxgene-census/api/python/cellxgene_census, configfile: pyproject.toml
+plugins: anyio-3.6.2, requests-mock-1.11.0
+collecting ... collected 274 items / 202 deselected / 72 selected
+
+api/python/cellxgene_census/tests/test_acceptance.py::test_load_axes[homo_sapiens] PASSED [  1%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_load_axes[mus_musculus] PASSED [  2%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_obs[2-None-homo_sapiens] PASSED [  4%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_obs[2-None-mus_musculus] PASSED [  5%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_obs[None-ctx_config1-homo_sapiens] PASSED [  6%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_obs[None-ctx_config1-mus_musculus] PASSED [  8%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_var[2-None-homo_sapiens] PASSED [  9%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_var[2-None-mus_musculus] PASSED [ 11%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_var[None-ctx_config1-homo_sapiens] PASSED [ 12%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_var[None-ctx_config1-mus_musculus] PASSED [ 13%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_X[2-None-homo_sapiens] PASSED [ 15%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_X[2-None-mus_musculus] PASSED [ 16%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_X[None-ctx_config1-homo_sapiens] PASSED [ 18%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_X[None-ctx_config1-mus_musculus] PASSED [ 19%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_X[None-ctx_config2-homo_sapiens] PASSED [ 20%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_read_X[None-ctx_config2-mus_musculus] PASSED [ 22%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[2-tissue=='aorta'-homo_sapiens] PASSED [ 23%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[2-tissue=='aorta'-mus_musculus] PASSED [ 25%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[2-tissue=='brain'-homo_sapiens] PASSED [ 26%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[2-tissue=='brain'-mus_musculus] PASSED [ 27%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[None-tissue=='aorta'-homo_sapiens] PASSED [ 29%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[None-tissue=='aorta'-mus_musculus] PASSED [ 30%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[None-tissue=='brain'-homo_sapiens] PASSED [ 31%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_incremental_query[None-tissue=='brain'-mus_musculus] PASSED [ 33%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[tissue=='aorta'-None-ctx_config0-homo_sapiens] PASSED [ 34%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[tissue=='aorta'-None-ctx_config0-mus_musculus] PASSED [ 36%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 10K cells-homo_sapiens] PASSED [ 37%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 10K cells-mus_musculus] PASSED [ 38%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 100K cells-homo_sapiens] PASSED [ 40%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 100K cells-mus_musculus] PASSED [ 41%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 250K cells-homo_sapiens] PASSED [ 43%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 250K cells-mus_musculus] PASSED [ 44%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 500K cells-homo_sapiens] PASSED [ 45%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 500K cells-mus_musculus] PASSED [ 47%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 750K cells-homo_sapiens] PASSED [ 48%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 750K cells-mus_musculus] PASSED [ 50%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 1M cells-homo_sapiens] PASSED [ 51%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[First 1M cells-mus_musculus] PASSED [ 52%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[tissue=='brain'-None-ctx_config7-homo_sapiens] PASSED [ 54%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[tissue=='brain'-None-ctx_config7-mus_musculus] PASSED [ 55%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[cell_type=='neuron'-None-ctx_config8-homo_sapiens] PASSED [ 56%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[cell_type=='neuron'-None-ctx_config8-mus_musculus] PASSED [ 58%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[is_primary_data==True-None-ctx_config9-homo_sapiens] PASSED [ 59%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[is_primary_data==True-None-ctx_config9-mus_musculus] PASSED [ 61%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[None-None-ctx_config10-homo_sapiens] PASSED [ 62%]
+api/python/cellxgene_census/tests/test_acceptance.py::test_get_anndata[None-None-ctx_config10-mus_musculus] PASSED [ 63%]
+api/python/cellxgene_census/tests/test_directory.py::test_get_census_version_directory PASSED [ 65%]
+api/python/cellxgene_census/tests/test_directory.py::test_get_census_version_description_errors PASSED [ 66%]
+api/python/cellxgene_census/tests/test_directory.py::test_live_directory_contents PASSED [ 68%]
+api/python/cellxgene_census/tests/test_get_anndata.py::test_get_anndata_value_filter PASSED [ 69%]
+api/python/cellxgene_census/tests/test_get_anndata.py::test_get_anndata_coords PASSED [ 70%]
+api/python/cellxgene_census/tests/test_get_anndata.py::test_get_anndata_allows_missing_obs_or_var_filter PASSED [ 72%]
+api/python/cellxgene_census/tests/test_get_helpers.py::test_get_experiment PASSED [ 73%]
+api/python/cellxgene_census/tests/test_get_helpers.py::test_get_presence_matrix[homo_sapiens] PASSED [ 75%]
+api/python/cellxgene_census/tests/test_get_helpers.py::test_get_presence_matrix[mus_musculus] PASSED [ 76%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_stable PASSED [ 77%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_latest PASSED [ 79%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_with_context PASSED [ 80%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_invalid_args PASSED [ 81%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_errors PASSED [ 83%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_defaults_to_latest_if_missing_stable PASSED [ 84%]
+api/python/cellxgene_census/tests/test_open.py::test_open_soma_defaults_to_stable PASSED [ 86%]
+api/python/cellxgene_census/tests/test_open.py::test_get_source_h5ad_uri PASSED [ 87%]
+api/python/cellxgene_census/tests/test_open.py::test_get_source_h5ad_uri_errors PASSED [ 88%]
+api/python/cellxgene_census/tests/test_open.py::test_download_source_h5ad PASSED [ 90%]
+api/python/cellxgene_census/tests/test_open.py::test_download_source_h5ad_errors PASSED [ 91%]
+api/python/cellxgene_census/tests/test_open.py::test_opening_census_without_anon_access_fails_with_bogus_creds PASSED [ 93%]
+api/python/cellxgene_census/tests/test_open.py::test_can_open_with_anonymous_access PASSED [ 94%]
+api/python/cellxgene_census/tests/test_util.py::test_uri_join PASSED     [ 95%]
+api/python/cellxgene_census/tests/experimental/pp/test_stats.py::test_mean_variance_no_flags PASSED [ 97%]
+api/python/cellxgene_census/tests/experimental/pp/test_stats.py::test_mean_variance_empty_query[mus_musculus] PASSED [ 98%]
+api/python/cellxgene_census/tests/experimental/pp/test_stats.py::test_mean_variance_wrong_axis PASSED [100%]
+
+============================== slowest durations ===============================
+8283.70s call     tests/test_acceptance.py::test_get_anndata[None-None-ctx_config10-homo_sapiens]
+1767.98s call     tests/test_acceptance.py::test_get_anndata[is_primary_data==True-None-ctx_config9-homo_sapiens]
+1304.89s call     tests/test_acceptance.py::test_incremental_read_X[None-ctx_config1-homo_sapiens]
+953.35s call     tests/test_acceptance.py::test_incremental_read_X[None-ctx_config2-homo_sapiens]
+903.42s call     tests/test_acceptance.py::test_get_anndata[cell_type=='neuron'-None-ctx_config8-homo_sapiens]
+309.04s call     tests/test_acceptance.py::test_get_anndata[None-None-ctx_config10-mus_musculus]
+195.72s call     tests/test_acceptance.py::test_get_anndata[is_primary_data==True-None-ctx_config9-mus_musculus]
+135.65s call     tests/test_acceptance.py::test_incremental_read_X[None-ctx_config1-mus_musculus]
+115.40s call     tests/test_acceptance.py::test_incremental_read_X[None-ctx_config2-mus_musculus]
+65.46s call     tests/test_acceptance.py::test_get_anndata[First 1M cells-mus_musculus]
+53.50s call     tests/test_acceptance.py::test_get_anndata[First 750K cells-mus_musculus]
+44.52s call     tests/test_acceptance.py::test_get_anndata[cell_type=='neuron'-None-ctx_config8-mus_musculus]
+38.62s call     tests/test_acceptance.py::test_get_anndata[tissue=='brain'-None-ctx_config7-homo_sapiens]
+38.56s call     tests/test_acceptance.py::test_get_anndata[First 500K cells-mus_musculus]
+34.90s call     tests/test_acceptance.py::test_get_anndata[First 1M cells-homo_sapiens]
+31.58s call     tests/test_acceptance.py::test_incremental_query[None-tissue=='brain'-homo_sapiens]
+26.10s call     tests/test_acceptance.py::test_get_anndata[First 750K cells-homo_sapiens]
+23.89s call     tests/test_acceptance.py::test_get_anndata[First 500K cells-homo_sapiens]
+23.75s call     tests/test_acceptance.py::test_get_anndata[First 250K cells-mus_musculus]
+19.00s call     tests/test_acceptance.py::test_incremental_query[2-tissue=='brain'-homo_sapiens]
+16.80s call     tests/test_acceptance.py::test_get_anndata[First 250K cells-homo_sapiens]
+12.47s call     tests/test_acceptance.py::test_get_anndata[tissue=='brain'-None-ctx_config7-mus_musculus]
+12.25s call     tests/test_acceptance.py::test_get_anndata[First 100K cells-mus_musculus]
+10.88s call     tests/test_acceptance.py::test_get_anndata[First 100K cells-homo_sapiens]
+10.52s call     tests/test_get_anndata.py::test_get_anndata_allows_missing_obs_or_var_filter
+9.96s call     tests/test_acceptance.py::test_incremental_query[2-tissue=='aorta'-homo_sapiens]
+9.67s call     tests/test_acceptance.py::test_incremental_read_X[2-None-homo_sapiens]
+9.45s call     tests/test_acceptance.py::test_incremental_query[2-tissue=='brain'-mus_musculus]
+9.11s call     tests/test_acceptance.py::test_load_axes[homo_sapiens]
+8.81s call     tests/test_acceptance.py::test_incremental_query[None-tissue=='aorta'-homo_sapiens]
+7.96s call     tests/test_acceptance.py::test_incremental_query[None-tissue=='brain'-mus_musculus]
+7.77s call     tests/test_acceptance.py::test_get_anndata[tissue=='aorta'-None-ctx_config0-homo_sapiens]
+7.14s call     tests/test_directory.py::test_live_directory_contents
+5.47s call     tests/test_get_anndata.py::test_get_anndata_value_filter
+5.30s call     tests/test_acceptance.py::test_get_anndata[First 10K cells-homo_sapiens]
+4.82s call     tests/test_acceptance.py::test_get_anndata[First 10K cells-mus_musculus]
+4.69s call     tests/test_open.py::test_get_source_h5ad_uri
+4.47s call     tests/test_get_helpers.py::test_get_presence_matrix[homo_sapiens]
+4.46s call     tests/test_acceptance.py::test_incremental_query[2-tissue=='aorta'-mus_musculus]
+4.26s call     tests/test_acceptance.py::test_incremental_query[None-tissue=='aorta'-mus_musculus]
+3.89s call     tests/test_acceptance.py::test_incremental_read_X[2-None-mus_musculus]
+3.80s call     tests/test_acceptance.py::test_get_anndata[tissue=='aorta'-None-ctx_config0-mus_musculus]
+3.39s call     tests/test_acceptance.py::test_incremental_read_obs[None-ctx_config1-homo_sapiens]
+3.24s call     tests/test_get_helpers.py::test_get_presence_matrix[mus_musculus]
+3.02s call     tests/test_get_anndata.py::test_get_anndata_coords
+2.94s call     tests/test_open.py::test_download_source_h5ad
+2.54s call     tests/test_acceptance.py::test_load_axes[mus_musculus]
+1.80s call     tests/test_acceptance.py::test_incremental_read_obs[2-None-homo_sapiens]
+1.62s call     tests/test_acceptance.py::test_incremental_read_obs[2-None-mus_musculus]
+1.54s call     tests/test_acceptance.py::test_incremental_read_obs[None-ctx_config1-mus_musculus]
+1.40s call     tests/experimental/pp/test_stats.py::test_mean_variance_empty_query[mus_musculus]
+1.37s call     tests/test_acceptance.py::test_incremental_read_var[2-None-mus_musculus]
+1.34s call     tests/test_acceptance.py::test_incremental_read_var[None-ctx_config1-homo_sapiens]
+1.34s call     tests/test_acceptance.py::test_incremental_read_var[2-None-homo_sapiens]
+1.33s setup    tests/test_open.py::test_download_source_h5ad_errors
+1.28s call     tests/test_acceptance.py::test_incremental_read_var[None-ctx_config1-mus_musculus]
+1.20s setup    tests/test_open.py::test_download_source_h5ad
+1.13s call     tests/test_open.py::test_get_source_h5ad_uri_errors
+0.76s call     tests/test_open.py::test_open_soma_with_context
+0.71s call     tests/test_open.py::test_open_soma_stable
+0.56s call     tests/test_directory.py::test_get_census_version_description_errors
+0.48s call     tests/test_get_helpers.py::test_get_experiment
+0.47s setup    tests/test_get_anndata.py::test_get_anndata_allows_missing_obs_or_var_filter
+0.43s setup    tests/test_get_anndata.py::test_get_anndata_coords
+0.39s call     tests/test_open.py::test_open_soma_defaults_to_latest_if_missing_stable
+0.34s setup    tests/test_get_anndata.py::test_get_anndata_value_filter
+0.34s call     tests/test_open.py::test_open_soma_latest
+0.33s call     tests/test_open.py::test_can_open_with_anonymous_access
+0.26s call     tests/test_open.py::test_opening_census_without_anon_access_fails_with_bogus_creds
+0.04s setup    tests/test_directory.py::test_get_census_version_directory
+0.03s teardown tests/test_acceptance.py::test_get_anndata[None-None-ctx_config10-homo_sapiens]
+0.03s setup    tests/test_acceptance.py::test_get_anndata[None-None-ctx_config10-mus_musculus]
+0.02s teardown tests/test_acceptance.py::test_get_anndata[is_primary_data==True-None-ctx_config9-homo_sapiens]
+0.02s call     tests/test_directory.py::test_get_census_version_directory
+0.02s setup    tests/test_acceptance.py::test_get_anndata[is_primary_data==True-None-ctx_config9-mus_musculus]
+0.01s setup    tests/experimental/pp/test_stats.py::test_mean_variance_empty_query[mus_musculus]
+0.01s teardown tests/test_acceptance.py::test_get_anndata[cell_type=='neuron'-None-ctx_config8-homo_sapiens]
+0.01s setup    tests/test_acceptance.py::test_get_anndata[cell_type=='neuron'-None-ctx_config8-mus_musculus]
+0.01s call     tests/experimental/pp/test_stats.py::test_mean_variance_no_flags
+
+(137 durations < 0.005s hidden.  Use -vv to show these durations.)
+=============== 72 passed, 202 deselected in 14584.03s (4:03:04) ===============
+```
+
 ## 2023-06-23
 
-- Host: EC2 instance type: `r6id.x32xlarge`, all nvme mounted as swap.
-- Uname: Linux ip-172-31-52-152 5.19.0-1025-aws #26~22.04.1-Ubuntu SMP Mon Apr 24 01:58:15 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
+- Host: EC2 instance type: `r6id.32xlarge`, all nvme mounted as swap.
+- Uname: Linux 5.19.0-1025-aws #26~22.04.1-Ubuntu SMP Mon Apr 24 01:58:15 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
 - Python & census versions:
 ```
 >>> import cellxgene_census, tiledbsoma
 >>> tiledbsoma.show_package_versions()
 tiledbsoma.__version__        1.2.5
 TileDB-Py tiledb.version()    (0, 21, 5)
 TileDB core version           2.15.4
@@ -233,16 +418,16 @@
 
 (131 durations < 0.005s hidden.  Use -vv to show these durations.)
 =============== 69 passed, 111 deselected in 15040.59s (4:10:40) ===============
 ```
 
 ## 2023-05-16
 
-- Host: EC2 instance type: `r6id.x32xlarge`, all nvme mounted as swap.
-- Uname: Linux ip-172-31-59-194 5.19.0-1022-aws #23~22.04.1-Ubuntu SMP Fri Mar 17 15:38:24 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
+- Host: EC2 instance type: `r6id.32xlarge`, all nvme mounted as swap.
+- Uname: Linux 5.19.0-1022-aws #23~22.04.1-Ubuntu SMP Fri Mar 17 15:38:24 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
 - Python & census versions:
 ```
 >>> import cellxgene_census, tiledbsoma
 >>> tiledbsoma.show_package_versions()
 tiledbsoma.__version__        1.2.3
 TileDB-Py tiledb.version()    (0, 21, 3)
 TileDB core version           2.15.2
@@ -380,15 +565,15 @@
 ======================= 51 passed in 10696.20s (2:58:16) =======================
 ```
 
 ## 2023-03-29
 
 **Config**
 
-- Host: EC2 instance type: `r6id.x32xlarge`, all nvme mounted as swap.
+- Host: EC2 instance type: `r6id.32xlarge`, all nvme mounted as swap.
 - Uname: Linux bruce.aegea 5.15.0-1033-aws #37~20.04.1-Ubuntu SMP Fri Mar 17 11:39:30 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
 - Python & census versions:
 
 ```
 In [1]: import cell_census, tiledbsoma
 
 In [2]: tiledbsoma.show_package_versions()
```

### Comparing `cellxgene_census-1.3.1/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.4.0/tests/experimental/ml/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/experimental/pp/test_hvg.py` & `cellxgene_census-1.4.0/tests/experimental/pp/test_hvg.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,14 @@
 import scanpy as sc
 import tiledbsoma as soma
 
 import cellxgene_census
 from cellxgene_census.experimental.pp import get_highly_variable_genes, highly_variable_genes
 
 
-@pytest.fixture
-def small_mem_context() -> soma.SOMATileDBContext:
-    """used to keep memory usage smaller for GHA runners."""
-    cfg = {
-        "tiledb_config": {
-            "soma.init_buffer_bytes": 32 * 1024**2,
-            "vfs.s3.no_sign_request": True,
-        },
-    }
-    return soma.SOMATileDBContext().replace(**cfg)
-
-
 @pytest.mark.experimental
 @pytest.mark.live_corpus
 @pytest.mark.parametrize(
     "experiment_name,obs_value_filter",
     [
         ("mus_musculus", 'is_primary_data == True and tissue_general == "skin of body"'),
         pytest.param(
```

### Comparing `cellxgene_census-1.3.1/tests/experimental/pp/test_online.py` & `cellxgene_census-1.4.0/tests/experimental/pp/test_online.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import numpy.typing as npt
 import pytest
 from scipy import sparse
 
-from cellxgene_census.experimental.pp._online import MeanVarianceAccumulator
+from cellxgene_census.experimental.pp._online import CountsAccumulator, MeanAccumulator, MeanVarianceAccumulator
 
 
 def allclose(a: npt.NDArray[np.float64], b: npt.NDArray[np.float64]) -> bool:
     return np.allclose(a, b, atol=1e-5, rtol=1e-3, equal_nan=True)
 
 
 @pytest.fixture
@@ -19,46 +19,108 @@
     return m
 
 
 @pytest.mark.experimental
 @pytest.mark.parametrize("stride", [101, 53])
 @pytest.mark.parametrize("n_batches", [1, 3, 11, 101])
 @pytest.mark.parametrize("m,n", [(1200, 511), (100001, 57)])
-def test_meanvar(matrix: sparse.coo_matrix, n_batches: int, stride: int) -> None:
+@pytest.mark.parametrize("ddof", [0, 1, 100])
+def test_meanvar(matrix: sparse.coo_matrix, n_batches: int, stride: int, ddof: int) -> None:
     rng = np.random.default_rng()
     batches_prob = rng.random(n_batches)
     batches_prob /= batches_prob.sum()
     batches = rng.choice(n_batches, matrix.shape[0], p=batches_prob)
     batches.flags.writeable = False
 
     batch_id, batch_count = np.unique(batches, return_counts=True)
     n_samples = np.zeros((n_batches,), dtype=np.int64)
     n_samples[batch_id] = batch_count
     assert n_samples.sum() == matrix.shape[0]
     assert len(n_samples) == n_batches
 
-    olmv = MeanVarianceAccumulator(n_batches, n_samples, matrix.shape[1])
+    olmv = MeanVarianceAccumulator(n_batches, n_samples, matrix.shape[1], ddof)
     for i in range(0, matrix.nnz, stride):
-        olmv.update_by_batch(
-            batches[matrix.row[i : i + stride]], matrix.col[i : i + stride], matrix.data[i : i + stride]
-        )
+        batch_vec = batches[matrix.row[i : i + stride]] if n_batches > 1 else None
+        olmv.update(matrix.col[i : i + stride], matrix.data[i : i + stride], batch_vec)
     batches_u, batches_var, all_u, all_var = olmv.finalize()
 
     assert isinstance(all_u, np.ndarray)
     assert isinstance(all_var, np.ndarray)
     assert isinstance(batches_u, np.ndarray)
     assert isinstance(batches_var, np.ndarray)
 
     assert all_u.shape == (matrix.shape[1],)
     assert all_var.shape == (matrix.shape[1],)
     assert batches_u.shape == (n_batches, matrix.shape[1])
     assert batches_var.shape == (n_batches, matrix.shape[1])
 
     dense = matrix.toarray()
     assert allclose(all_u, dense.mean(axis=0))
-    assert allclose(all_var, dense.var(axis=0, ddof=1, dtype=np.float64))
+    assert allclose(all_var, dense.var(axis=0, ddof=ddof, dtype=np.float64))
 
     matrix = matrix.tocsr()  # COO not conveniently indexable
     for batch in range(n_batches):
         dense = matrix[batches == batch, :].toarray()
         assert allclose(batches_u[batch], dense.mean(axis=0))
-        assert allclose(batches_var[batch], dense.var(axis=0, ddof=1, dtype=np.float64))
+        assert allclose(batches_var[batch], dense.var(axis=0, ddof=ddof, dtype=np.float64))
+
+
+@pytest.mark.experimental
+@pytest.mark.parametrize("stride", [101, 53])
+@pytest.mark.parametrize("m,n", [(1200, 511), (100001, 57)])
+def test_mean(matrix: sparse.coo_matrix, stride: int) -> None:
+    m_acc = MeanAccumulator(matrix.shape[0], matrix.shape[1])
+    for i in range(0, matrix.nnz, stride):
+        m_acc.update(matrix.col[i : i + stride], matrix.data[i : i + stride])
+    u = m_acc.finalize()
+
+    assert isinstance(u, np.ndarray)
+    assert u.shape == (matrix.shape[1],)
+
+    dense = matrix.toarray()
+    assert allclose(u, dense.mean(axis=0))
+
+
+@pytest.mark.experimental
+@pytest.mark.parametrize("stride", [101, 53])
+@pytest.mark.parametrize("n_batches", [1, 3, 11, 101])
+@pytest.mark.parametrize("m,n", [(1200, 511), (100001, 57)])
+def test_counts(matrix: sparse.coo_matrix, n_batches: int, stride: int) -> None:
+    rng = np.random.default_rng()
+    batches_prob = rng.random(n_batches)
+    batches_prob /= batches_prob.sum()
+    batches = rng.choice(n_batches, matrix.shape[0], p=batches_prob)
+    batches.flags.writeable = False
+
+    batch_id, batch_count = np.unique(batches, return_counts=True)
+    n_samples = np.zeros((n_batches,), dtype=np.int64)
+    n_samples[batch_id] = batch_count
+    assert n_samples.sum() == matrix.shape[0]
+    assert len(n_samples) == n_batches
+
+    clip_val = 50 * np.random.rand(n_batches, matrix.shape[1])
+
+    ca = CountsAccumulator(n_batches, matrix.shape[1], clip_val)
+    for i in range(0, matrix.nnz, stride):
+        batch_vec = batches[matrix.row[i : i + stride]] if n_batches > 1 else None
+        ca.update(matrix.col[i : i + stride], matrix.data[i : i + stride], batch_vec)
+    counts_sum, counts_squared_sum = ca.finalize()
+
+    assert isinstance(counts_sum, np.ndarray)
+    assert isinstance(counts_squared_sum, np.ndarray)
+
+    assert counts_sum.shape == (n_batches, matrix.shape[1])
+    assert counts_squared_sum.shape == (n_batches, matrix.shape[1])
+
+    matrix = matrix.tocsr()  # COO not conveniently indexable
+    for batch in range(n_batches):
+        dense = matrix[batches == batch, :].toarray()
+        assert allclose(counts_sum[batch], np.minimum(dense, clip_val[batch]).sum(axis=0))
+        assert allclose(counts_squared_sum[batch], (np.minimum(dense, clip_val[batch]) ** 2).sum(axis=0))
+
+
+@pytest.mark.experimental
+def test_mean_fails_no_variables_or_samples() -> None:
+    with pytest.raises(ValueError, match=r"No samples provided - can't calculate mean."):
+        MeanAccumulator(n_samples=0, n_variables=100)
+    with pytest.raises(ValueError, match=r"No variables provided - can't calculate mean."):
+        MeanAccumulator(n_samples=1000, n_variables=0)
```

### Comparing `cellxgene_census-1.3.1/tests/experimental/util/test_csr_iter.py` & `cellxgene_census-1.4.0/tests/experimental/util/test_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/test_acceptance.py` & `cellxgene_census-1.4.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/test_directory.py` & `cellxgene_census-1.4.0/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/test_get_anndata.py` & `cellxgene_census-1.4.0/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/test_get_helpers.py` & `cellxgene_census-1.4.0/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/test_open.py` & `cellxgene_census-1.4.0/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.3.1/tests/test_util.py` & `cellxgene_census-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

