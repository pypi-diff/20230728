# Comparing `tmp/jamofetch-3.5.0.tar.gz` & `tmp/jamofetch-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamofetch-3.5.0.tar", max compression
+gzip compressed data, was "jamofetch-3.5.1.tar", max compression
```

## Comparing `jamofetch-3.5.0.tar` & `jamofetch-3.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4675 2023-07-22 04:56:00.098688 jamofetch-3.5.0/README.md
--rw-r--r--   0        0        0      522 2023-07-27 23:07:05.500848 jamofetch-3.5.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-07 23:08:25.647260 jamofetch-3.5.0/src/jamofetch/__init__.py
--rwxr-xr-x   0        0        0    10932 2023-07-27 23:05:24.072873 jamofetch-3.5.0/src/jamofetch/jamofetch.py
--rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4675 2023-07-27 23:09:54.226061 jamofetch-3.5.1/README.md
+-rw-r--r--   0        0        0      522 2023-07-27 23:43:14.073452 jamofetch-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.5.1/src/jamofetch/__init__.py
+-rwxr-xr-x   0        0        0    10932 2023-07-27 23:09:54.227061 jamofetch-3.5.1/src/jamofetch/jamofetch.py
+-rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.5.1/PKG-INFO
```

### Comparing `jamofetch-3.5.0/README.md` & `jamofetch-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `jamofetch-3.5.0/pyproject.toml` & `jamofetch-3.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamofetch"
-version = "3.5.0"
+version = "3.5.1"
 description = "A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori."
 authors = ["Duncan Scott"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `jamofetch-3.5.0/src/jamofetch/jamofetch.py` & `jamofetch-3.5.1/src/jamofetch/jamofetch.py`

 * *Files identical despite different names*

### Comparing `jamofetch-3.5.0/PKG-INFO` & `jamofetch-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamofetch
-Version: 3.5.0
+Version: 3.5.1
 Summary: A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori.
 License: None
 Author: Duncan Scott
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

