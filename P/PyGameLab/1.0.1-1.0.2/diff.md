# Comparing `tmp/PyGameLab-1.0.1.tar.gz` & `tmp/PyGameLab-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGameLab-1.0.1.tar", last modified: Tue Jul 25 20:04:19 2023, max compression
+gzip compressed data, was "PyGameLab-1.0.2.tar", last modified: Fri Jul 28 00:18:25 2023, max compression
```

## Comparing `PyGameLab-1.0.1.tar` & `PyGameLab-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1072 2023-07-16 20:03:01.000000 PyGameLab-1.0.1/LICENCE
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1687 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/PKG-INFO
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1133 2023-07-25 19:47:09.000000 PyGameLab-1.0.1/README.md
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      639 2023-07-25 20:04:02.000000 PyGameLab-1.0.1/pyproject.toml
--rw-r--r--   0 leandrofeippe     (0) staff       (20)       38 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/setup.cfg
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/PyGameLab.egg-info/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1687 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/PyGameLab.egg-info/PKG-INFO
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      421 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/PyGameLab.egg-info/SOURCES.txt
--rw-r--r--   0 leandrofeippe     (0) staff       (20)        1 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/PyGameLab.egg-info/dependency_links.txt
--rw-r--r--   0 leandrofeippe     (0) staff       (20)       10 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/PyGameLab.egg-info/top_level.txt
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-25 20:04:19.000000 PyGameLab-1.0.1/src/pygamelab/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)    10800 2023-07-25 19:44:50.000000 PyGameLab-1.0.1/src/pygamelab/__init__.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)        0 2023-07-25 18:03:01.000000 PyGameLab-1.0.1/src/pygamelab/canvas.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      402 2023-07-24 23:20:36.000000 PyGameLab-1.0.1/src/pygamelab/colors.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      297 2023-07-24 23:25:39.000000 PyGameLab-1.0.1/src/pygamelab/console.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      375 2023-07-24 23:17:56.000000 PyGameLab-1.0.1/src/pygamelab/data.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      368 2023-07-24 23:17:41.000000 PyGameLab-1.0.1/src/pygamelab/date.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      344 2023-07-25 19:45:05.000000 PyGameLab-1.0.1/src/pygamelab/locals.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1505 2023-07-23 19:50:56.000000 PyGameLab-1.0.1/src/pygamelab/random.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      929 2023-07-23 18:40:13.000000 PyGameLab-1.0.1/src/pygamelab/storage.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      604 2023-07-24 23:19:53.000000 PyGameLab-1.0.1/src/pygamelab/unicode.py
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1072 2023-07-16 20:03:01.000000 PyGameLab-1.0.2/LICENCE
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1687 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/PKG-INFO
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1133 2023-07-25 19:47:09.000000 PyGameLab-1.0.2/README.md
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      639 2023-07-28 00:17:04.000000 PyGameLab-1.0.2/pyproject.toml
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)       38 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/setup.cfg
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/PyGameLab.egg-info/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1687 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/PyGameLab.egg-info/PKG-INFO
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      424 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/PyGameLab.egg-info/SOURCES.txt
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)        1 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/PyGameLab.egg-info/dependency_links.txt
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)       10 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/PyGameLab.egg-info/top_level.txt
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 00:18:25.000000 PyGameLab-1.0.2/src/pygamelab/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)    10792 2023-07-27 23:06:04.000000 PyGameLab-1.0.2/src/pygamelab/__init__.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1712 2023-07-25 21:20:34.000000 PyGameLab-1.0.2/src/pygamelab/canvas.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      403 2023-07-25 20:38:18.000000 PyGameLab-1.0.2/src/pygamelab/colors.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      297 2023-07-24 23:25:39.000000 PyGameLab-1.0.2/src/pygamelab/console.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      344 2023-07-25 19:45:05.000000 PyGameLab-1.0.2/src/pygamelab/constants.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      375 2023-07-28 00:17:19.000000 PyGameLab-1.0.2/src/pygamelab/data.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      367 2023-07-25 20:56:51.000000 PyGameLab-1.0.2/src/pygamelab/date.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1478 2023-07-25 21:08:01.000000 PyGameLab-1.0.2/src/pygamelab/random.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      929 2023-07-25 21:15:34.000000 PyGameLab-1.0.2/src/pygamelab/storage.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      515 2023-07-25 21:00:14.000000 PyGameLab-1.0.2/src/pygamelab/unicode.py
```

### Comparing `PyGameLab-1.0.1/LICENCE` & `PyGameLab-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.1/PKG-INFO` & `PyGameLab-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGameLab
-Version: 1.0.1
+Version: 1.0.2
 Summary: PyGameLab: A versatile Python library for game development using Pygame.
 Author-email: Leandro Feippe <feippe5454@gmail.com>
 Project-URL: Homepage, https://github.com/PyGameLab/pygamelab/
 Project-URL: Bug Tracker, https://github.com/PyGameLab/pygamelab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyGameLab-1.0.1/README.md` & `PyGameLab-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.1/pyproject.toml` & `PyGameLab-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "pygame"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "PyGameLab"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Leandro Feippe", email="feippe5454@gmail.com" },
 ]
 description = "PyGameLab: A versatile Python library for game development using Pygame."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `PyGameLab-1.0.1/src/PyGameLab.egg-info/PKG-INFO` & `PyGameLab-1.0.2/src/PyGameLab.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGameLab
-Version: 1.0.1
+Version: 1.0.2
 Summary: PyGameLab: A versatile Python library for game development using Pygame.
 Author-email: Leandro Feippe <feippe5454@gmail.com>
 Project-URL: Homepage, https://github.com/PyGameLab/pygamelab/
 Project-URL: Bug Tracker, https://github.com/PyGameLab/pygamelab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyGameLab-1.0.1/src/pygamelab/__init__.py` & `PyGameLab-1.0.2/src/pygamelab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyGameLab import data, document
+from PyGameLab import data, document, locals
 import pygame
 import unicodedata
 import sys
 import pygame
 import pygame.locals
 
 
@@ -325,13 +325,14 @@
                 image_surface.set_at((x, y), pixel_color)
 
         return image_surface
 
     @staticmethod
     def createBitMap(color, size):
         bitmap = []
-        count = 0
         w, h = size
         for i in range(w):
             for j in range(h):
                 bitmap.append(color)
         return bitmap
+
+
```

### Comparing `PyGameLab-1.0.1/src/pygamelab/random.py` & `PyGameLab-1.0.2/src/pygamelab/random.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     return ''.join(random.choice(characters) for _ in range(length))
 
 
 def boolean():
     return random.choice([True, False])
 
 
-def element_from_string(text):
+def element(text):
     return random.choice(text)
 
 
-def sample_from_list(lst, k):
+def sample(lst, k):
     return random.sample(lst, k)
 
 
-def shuffle_list(lst):
+def shuffle(lst):
     random.shuffle(lst)
     return lst
 
 
 def color():
     r = random.randint(0, 255)
     g = random.randint(0, 255)
```

### Comparing `PyGameLab-1.0.1/src/pygamelab/storage.py` & `PyGameLab-1.0.2/src/pygamelab/storage.py`

 * *Files identical despite different names*

