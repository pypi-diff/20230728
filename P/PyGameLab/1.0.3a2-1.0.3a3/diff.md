# Comparing `tmp/PyGameLab-1.0.3a2.tar.gz` & `tmp/PyGameLab-1.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGameLab-1.0.3a2.tar", last modified: Fri Jul 28 16:15:16 2023, max compression
+gzip compressed data, was "PyGameLab-1.0.3a3.tar", last modified: Fri Jul 28 16:28:39 2023, max compression
```

## Comparing `PyGameLab-1.0.3a2.tar` & `PyGameLab-1.0.3a3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1072 2023-07-16 20:03:01.000000 PyGameLab-1.0.3a2/LICENCE
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/PKG-INFO
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1133 2023-07-25 19:47:09.000000 PyGameLab-1.0.3a2/README.md
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      642 2023-07-28 16:14:51.000000 PyGameLab-1.0.3a2/pyproject.toml
--rw-r--r--   0 leandrofeippe     (0) staff       (20)       38 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/setup.cfg
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/PyGameLab.egg-info/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/PyGameLab.egg-info/PKG-INFO
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      424 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/PyGameLab.egg-info/SOURCES.txt
--rw-r--r--   0 leandrofeippe     (0) staff       (20)        1 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/PyGameLab.egg-info/dependency_links.txt
--rw-r--r--   0 leandrofeippe     (0) staff       (20)       10 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/PyGameLab.egg-info/top_level.txt
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:15:16.000000 PyGameLab-1.0.3a2/src/pygamelab/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)    10743 2023-07-28 16:14:32.000000 PyGameLab-1.0.3a2/src/pygamelab/__init__.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1712 2023-07-25 21:20:34.000000 PyGameLab-1.0.3a2/src/pygamelab/canvas.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      403 2023-07-25 20:38:18.000000 PyGameLab-1.0.3a2/src/pygamelab/colors.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      297 2023-07-24 23:25:39.000000 PyGameLab-1.0.3a2/src/pygamelab/console.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      344 2023-07-25 19:45:05.000000 PyGameLab-1.0.3a2/src/pygamelab/constants.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      378 2023-07-28 16:15:02.000000 PyGameLab-1.0.3a2/src/pygamelab/data.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      367 2023-07-25 20:56:51.000000 PyGameLab-1.0.3a2/src/pygamelab/date.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1478 2023-07-25 21:08:01.000000 PyGameLab-1.0.3a2/src/pygamelab/random.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      929 2023-07-25 21:15:34.000000 PyGameLab-1.0.3a2/src/pygamelab/storage.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      515 2023-07-25 21:00:14.000000 PyGameLab-1.0.3a2/src/pygamelab/unicode.py
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1072 2023-07-16 20:03:01.000000 PyGameLab-1.0.3a3/LICENCE
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/PKG-INFO
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1133 2023-07-25 19:47:09.000000 PyGameLab-1.0.3a3/README.md
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      642 2023-07-28 16:28:13.000000 PyGameLab-1.0.3a3/pyproject.toml
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)       38 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/setup.cfg
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/PyGameLab.egg-info/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/PyGameLab.egg-info/PKG-INFO
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      424 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/PyGameLab.egg-info/SOURCES.txt
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)        1 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/PyGameLab.egg-info/dependency_links.txt
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)       10 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/PyGameLab.egg-info/top_level.txt
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:28:39.000000 PyGameLab-1.0.3a3/src/pygamelab/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)    10743 2023-07-28 16:14:32.000000 PyGameLab-1.0.3a3/src/pygamelab/__init__.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1712 2023-07-25 21:20:34.000000 PyGameLab-1.0.3a3/src/pygamelab/canvas.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      403 2023-07-25 20:38:18.000000 PyGameLab-1.0.3a3/src/pygamelab/colors.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      297 2023-07-24 23:25:39.000000 PyGameLab-1.0.3a3/src/pygamelab/console.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      757 2023-07-28 16:28:05.000000 PyGameLab-1.0.3a3/src/pygamelab/constants.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      378 2023-07-28 16:28:19.000000 PyGameLab-1.0.3a3/src/pygamelab/data.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      367 2023-07-25 20:56:51.000000 PyGameLab-1.0.3a3/src/pygamelab/date.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1478 2023-07-25 21:08:01.000000 PyGameLab-1.0.3a3/src/pygamelab/random.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      929 2023-07-25 21:15:34.000000 PyGameLab-1.0.3a3/src/pygamelab/storage.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      515 2023-07-25 21:00:14.000000 PyGameLab-1.0.3a3/src/pygamelab/unicode.py
```

### Comparing `PyGameLab-1.0.3a2/LICENCE` & `PyGameLab-1.0.3a3/LICENCE`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.3a2/PKG-INFO` & `PyGameLab-1.0.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGameLab
-Version: 1.0.3a2
+Version: 1.0.3a3
 Summary: PyGameLab: A versatile Python library for game development using Pygame.
 Author-email: Leandro Feippe <feippe5454@gmail.com>
 Project-URL: Homepage, https://github.com/PyGameLab/pygamelab/
 Project-URL: Bug Tracker, https://github.com/PyGameLab/pygamelab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyGameLab-1.0.3a2/README.md` & `PyGameLab-1.0.3a3/README.md`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.3a2/pyproject.toml` & `PyGameLab-1.0.3a3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "pygame"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "PyGameLab"
-version = "1.0.3-a2"
+version = "1.0.3-a3"
 authors = [
   { name="Leandro Feippe", email="feippe5454@gmail.com" },
 ]
 description = "PyGameLab: A versatile Python library for game development using Pygame."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `PyGameLab-1.0.3a2/src/PyGameLab.egg-info/PKG-INFO` & `PyGameLab-1.0.3a3/src/PyGameLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGameLab
-Version: 1.0.3a2
+Version: 1.0.3a3
 Summary: PyGameLab: A versatile Python library for game development using Pygame.
 Author-email: Leandro Feippe <feippe5454@gmail.com>
 Project-URL: Homepage, https://github.com/PyGameLab/pygamelab/
 Project-URL: Bug Tracker, https://github.com/PyGameLab/pygamelab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyGameLab-1.0.3a2/src/pygamelab/__init__.py` & `PyGameLab-1.0.3a3/src/pygamelab/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.3a2/src/pygamelab/canvas.py` & `PyGameLab-1.0.3a3/src/pygamelab/canvas.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.3a2/src/pygamelab/random.py` & `PyGameLab-1.0.3a3/src/pygamelab/random.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.3a2/src/pygamelab/storage.py` & `PyGameLab-1.0.3a3/src/pygamelab/storage.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.3a2/src/pygamelab/unicode.py` & `PyGameLab-1.0.3a3/src/pygamelab/unicode.py`

 * *Files identical despite different names*

