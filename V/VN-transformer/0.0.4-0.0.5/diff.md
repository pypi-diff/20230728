# Comparing `tmp/VN-transformer-0.0.4.tar.gz` & `tmp/VN-transformer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.4.tar", last modified: Fri Jul 28 18:18:55 2023, max compression
+gzip compressed data, was "VN-transformer-0.0.5.tar", last modified: Fri Jul 28 18:19:29 2023, max compression
```

## Comparing `VN-transformer-0.0.4.tar` & `VN-transformer-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:18:55.979866 VN-transformer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 18:18:55.979866 VN-transformer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:18:55.979866 VN-transformer-0.0.4/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:18:55.979866 VN-transformer-0.0.4/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 18:18:55.000000 VN-transformer-0.0.4/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 18:18:55.000000 VN-transformer-0.0.4/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:18:55.000000 VN-transformer-0.0.4/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 18:18:55.000000 VN-transformer-0.0.4/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 18:18:55.000000 VN-transformer-0.0.4/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 18:18:55.979866 VN-transformer-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:18:55.979866 VN-transformer-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 18:18:42.000000 VN-transformer-0.0.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/tests/test.py
```

### Comparing `VN-transformer-0.0.4/LICENSE` & `VN-transformer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.4/PKG-INFO` & `VN-transformer-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.4/README.md` & `VN-transformer-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.4/VN_transformer/VN_transformer.py` & `VN-transformer-0.0.5/VN_transformer/VN_transformer.py`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.4/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.0.5/VN_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.4/setup.py` & `VN-transformer-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

### Comparing `VN-transformer-0.0.4/tests/test.py` & `VN-transformer-0.0.5/tests/test.py`

 * *Files identical despite different names*

