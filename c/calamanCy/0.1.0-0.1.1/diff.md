# Comparing `tmp/calamanCy-0.1.0.tar.gz` & `tmp/calamanCy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calamanCy-0.1.0.tar", last modified: Sun Jul  2 02:26:07 2023, max compression
+gzip compressed data, was "calamanCy-0.1.1.tar", last modified: Fri Jul 28 00:31:38 2023, max compression
```

## Comparing `calamanCy-0.1.0.tar` & `calamanCy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:07.359783 calamanCy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-02 02:25:57.000000 calamanCy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-02 02:26:07.359783 calamanCy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-02 02:25:57.000000 calamanCy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:07.359783 calamanCy-0.1.0/calamanCy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:07.359783 calamanCy-0.1.0/calamancy/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-02 02:25:57.000000 calamanCy-0.1.0/calamancy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-02 02:25:57.000000 calamanCy-0.1.0/calamancy/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-02 02:25:57.000000 calamanCy-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:26:07.359783 calamanCy-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:31:38.586874 calamanCy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-28 00:31:27.000000 calamanCy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-28 00:31:38.586874 calamanCy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-28 00:31:27.000000 calamanCy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:31:38.586874 calamanCy-0.1.1/calamanCy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-28 00:31:38.000000 calamanCy-0.1.1/calamanCy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 00:31:38.000000 calamanCy-0.1.1/calamanCy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:31:38.000000 calamanCy-0.1.1/calamanCy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 00:31:38.000000 calamanCy-0.1.1/calamanCy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 00:31:38.000000 calamanCy-0.1.1/calamanCy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:31:38.586874 calamanCy-0.1.1/calamancy/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 00:31:27.000000 calamanCy-0.1.1/calamancy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-28 00:31:27.000000 calamanCy-0.1.1/calamancy/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-28 00:31:27.000000 calamanCy-0.1.1/calamancy/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 00:31:27.000000 calamanCy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:31:38.586874 calamanCy-0.1.1/setup.cfg
```

### Comparing `calamanCy-0.1.0/LICENSE` & `calamanCy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calamanCy-0.1.0/calamancy/loaders.py` & `calamanCy-0.1.1/calamancy/loaders.py`

 * *Files identical despite different names*

### Comparing `calamanCy-0.1.0/pyproject.toml` & `calamanCy-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calamanCy"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Lj V. Miranda", email = "ljvmiranda@gmail.com"}
 ]
 description = "NLP Pipelines for Tagalog"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 keywords = ["nlp", "natural language processing", "language technology", "tagalog"]
```

