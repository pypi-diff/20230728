# Comparing `tmp/PyGameLab-1.0.2a1.tar.gz` & `tmp/PyGameLab-1.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGameLab-1.0.2a1.tar", last modified: Fri Jul 28 01:10:36 2023, max compression
+gzip compressed data, was "PyGameLab-1.0.3a1.tar", last modified: Fri Jul 28 16:02:12 2023, max compression
```

## Comparing `PyGameLab-1.0.2a1.tar` & `PyGameLab-1.0.3a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1072 2023-07-16 20:03:01.000000 PyGameLab-1.0.2a1/LICENCE
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/PKG-INFO
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1133 2023-07-25 19:47:09.000000 PyGameLab-1.0.2a1/README.md
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      642 2023-07-28 00:53:07.000000 PyGameLab-1.0.2a1/pyproject.toml
--rw-r--r--   0 leandrofeippe     (0) staff       (20)       38 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/setup.cfg
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/PyGameLab.egg-info/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/PyGameLab.egg-info/PKG-INFO
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      424 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/PyGameLab.egg-info/SOURCES.txt
--rw-r--r--   0 leandrofeippe     (0) staff       (20)        1 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/PyGameLab.egg-info/dependency_links.txt
--rw-r--r--   0 leandrofeippe     (0) staff       (20)       10 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/PyGameLab.egg-info/top_level.txt
-drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 01:10:36.000000 PyGameLab-1.0.2a1/src/pygamelab/
--rw-r--r--   0 leandrofeippe     (0) staff       (20)    10765 2023-07-28 00:52:56.000000 PyGameLab-1.0.2a1/src/pygamelab/__init__.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1712 2023-07-25 21:20:34.000000 PyGameLab-1.0.2a1/src/pygamelab/canvas.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      403 2023-07-25 20:38:18.000000 PyGameLab-1.0.2a1/src/pygamelab/colors.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      297 2023-07-24 23:25:39.000000 PyGameLab-1.0.2a1/src/pygamelab/console.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      344 2023-07-25 19:45:05.000000 PyGameLab-1.0.2a1/src/pygamelab/constants.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      375 2023-07-28 00:17:19.000000 PyGameLab-1.0.2a1/src/pygamelab/data.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      367 2023-07-25 20:56:51.000000 PyGameLab-1.0.2a1/src/pygamelab/date.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)     1478 2023-07-25 21:08:01.000000 PyGameLab-1.0.2a1/src/pygamelab/random.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      929 2023-07-25 21:15:34.000000 PyGameLab-1.0.2a1/src/pygamelab/storage.py
--rw-r--r--   0 leandrofeippe     (0) staff       (20)      515 2023-07-25 21:00:14.000000 PyGameLab-1.0.2a1/src/pygamelab/unicode.py
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1072 2023-07-16 20:03:01.000000 PyGameLab-1.0.3a1/LICENCE
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/PKG-INFO
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1133 2023-07-25 19:47:09.000000 PyGameLab-1.0.3a1/README.md
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      642 2023-07-28 16:01:58.000000 PyGameLab-1.0.3a1/pyproject.toml
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)       38 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/setup.cfg
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/PyGameLab.egg-info/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1689 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/PyGameLab.egg-info/PKG-INFO
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      424 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/PyGameLab.egg-info/SOURCES.txt
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)        1 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/PyGameLab.egg-info/dependency_links.txt
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)       10 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/PyGameLab.egg-info/top_level.txt
+drwxr-xr-x   0 leandrofeippe     (0) staff       (20)        0 2023-07-28 16:02:12.000000 PyGameLab-1.0.3a1/src/pygamelab/
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)    10767 2023-07-28 15:42:48.000000 PyGameLab-1.0.3a1/src/pygamelab/__init__.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1712 2023-07-25 21:20:34.000000 PyGameLab-1.0.3a1/src/pygamelab/canvas.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      403 2023-07-25 20:38:18.000000 PyGameLab-1.0.3a1/src/pygamelab/colors.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      297 2023-07-24 23:25:39.000000 PyGameLab-1.0.3a1/src/pygamelab/console.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      344 2023-07-25 19:45:05.000000 PyGameLab-1.0.3a1/src/pygamelab/constants.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      378 2023-07-28 16:01:53.000000 PyGameLab-1.0.3a1/src/pygamelab/data.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      367 2023-07-25 20:56:51.000000 PyGameLab-1.0.3a1/src/pygamelab/date.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)     1478 2023-07-25 21:08:01.000000 PyGameLab-1.0.3a1/src/pygamelab/random.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      929 2023-07-25 21:15:34.000000 PyGameLab-1.0.3a1/src/pygamelab/storage.py
+-rw-r--r--   0 leandrofeippe     (0) staff       (20)      515 2023-07-25 21:00:14.000000 PyGameLab-1.0.3a1/src/pygamelab/unicode.py
```

### Comparing `PyGameLab-1.0.2a1/LICENCE` & `PyGameLab-1.0.3a1/LICENCE`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.2a1/PKG-INFO` & `PyGameLab-1.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGameLab
-Version: 1.0.2a1
+Version: 1.0.3a1
 Summary: PyGameLab: A versatile Python library for game development using Pygame.
 Author-email: Leandro Feippe <feippe5454@gmail.com>
 Project-URL: Homepage, https://github.com/PyGameLab/pygamelab/
 Project-URL: Bug Tracker, https://github.com/PyGameLab/pygamelab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyGameLab-1.0.2a1/README.md` & `PyGameLab-1.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.2a1/pyproject.toml` & `PyGameLab-1.0.3a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "pygame"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "PyGameLab"
-version = "1.0.2-a1"
+version = "1.0.3-a1"
 authors = [
   { name="Leandro Feippe", email="feippe5454@gmail.com" },
 ]
 description = "PyGameLab: A versatile Python library for game development using Pygame."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `PyGameLab-1.0.2a1/src/PyGameLab.egg-info/PKG-INFO` & `PyGameLab-1.0.3a1/src/PyGameLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGameLab
-Version: 1.0.2a1
+Version: 1.0.3a1
 Summary: PyGameLab: A versatile Python library for game development using Pygame.
 Author-email: Leandro Feippe <feippe5454@gmail.com>
 Project-URL: Homepage, https://github.com/PyGameLab/pygamelab/
 Project-URL: Bug Tracker, https://github.com/PyGameLab/pygamelab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyGameLab-1.0.2a1/src/pygamelab/__init__.py` & `PyGameLab-1.0.3a1/src/pygamelab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from PyGameLab import data, unicode
+from PyGameLab import data, unicode, constants
 import pygame
 import unicodedata
 import sys
 import pygame
 import pygame.locals
 
 
+
 def init():
     if not data.initialized:
         pygame.init()
         unicode.key = {}
         for codepoint in range(0x10000):
             char = chr(codepoint)
             name = unicodedata.name(char, "")
@@ -289,15 +290,15 @@
         if text_rect is not None:
             pygame.draw.rect(screen.screen, (0, 0, 0), text_rect)
             pygame.display.update(text_rect)
 
 
 class Image:
     @staticmethod
-    def displayImage(screen, image, position, size, opacity=255, brightness=255):
+    def display(screen, image, position, size, opacity=255, brightness=255):
         if isinstance(image, str):
             image_surface = pygame.image.load(image).convert_alpha()
         elif isinstance(image, pygame.Surface):
             image_surface = image
         else:
             raise ValueError(
                 "El argumento 'image' debe ser una cadena de ruta de archivo o un objeto pygame.Surface.")
@@ -312,15 +313,15 @@
             image_surface = pygame.Surface.convert(image_surface)
             image_surface.fill(
                 (brightness, brightness, brightness), None, pygame.BLEND_RGB_MULT)
 
         screen.screen.blit(image_surface, position)
 
     @staticmethod
-    def newImage(bitMap, size=(16, 16)):
+    def new(bitMap, size=(16, 16)):
         image_surface = pygame.Surface(size, pygame.SRCALPHA)
 
         for y in range(size[1]):
             for x in range(size[0]):
                 pixel_color = bitMap[y * size[0] + x]
                 image_surface.set_at((x, y), pixel_color)
```

### Comparing `PyGameLab-1.0.2a1/src/pygamelab/canvas.py` & `PyGameLab-1.0.3a1/src/pygamelab/canvas.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.2a1/src/pygamelab/random.py` & `PyGameLab-1.0.3a1/src/pygamelab/random.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.2a1/src/pygamelab/storage.py` & `PyGameLab-1.0.3a1/src/pygamelab/storage.py`

 * *Files identical despite different names*

### Comparing `PyGameLab-1.0.2a1/src/pygamelab/unicode.py` & `PyGameLab-1.0.3a1/src/pygamelab/unicode.py`

 * *Files identical despite different names*

