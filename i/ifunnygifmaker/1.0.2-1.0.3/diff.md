# Comparing `tmp/ifunnygifmaker-1.0.2.tar.gz` & `tmp/ifunnygifmaker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-1.0.2.tar", last modified: Fri Jul 28 04:49:50 2023, max compression
+gzip compressed data, was "ifunnygifmaker-1.0.3.tar", last modified: Fri Jul 28 04:52:10 2023, max compression
```

## Comparing `ifunnygifmaker-1.0.2.tar` & `ifunnygifmaker-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      274 2023-07-11 21:32:07.857910 ifunnygifmaker-1.0.2/README.md
--rw-r--r--   0        0        0       39 2023-07-11 21:32:07.857910 ifunnygifmaker-1.0.2/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0    25492 2023-07-11 21:32:07.857910 ifunnygifmaker-1.0.2/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
--rw-r--r--   0        0        0     5209 2023-07-28 04:48:05.341567 ifunnygifmaker-1.0.2/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      578 2023-07-28 03:31:44.122022 ifunnygifmaker-1.0.2/ifunnygifmaker/utils/image_utils.py
--rw-r--r--   0        0        0      447 2023-07-28 04:49:46.461556 ifunnygifmaker-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 ifunnygifmaker-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-07-11 21:32:07.857910 ifunnygifmaker-1.0.3/README.md
+-rw-r--r--   0        0        0       39 2023-07-11 21:32:07.857910 ifunnygifmaker-1.0.3/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0    25492 2023-07-11 21:32:07.857910 ifunnygifmaker-1.0.3/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
+-rw-r--r--   0        0        0     5209 2023-07-28 04:51:56.901543 ifunnygifmaker-1.0.3/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      578 2023-07-28 03:31:44.122022 ifunnygifmaker-1.0.3/ifunnygifmaker/utils/image_utils.py
+-rw-r--r--   0        0        0      447 2023-07-28 04:52:07.791541 ifunnygifmaker-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 ifunnygifmaker-1.0.3/PKG-INFO
```

### Comparing `ifunnygifmaker-1.0.2/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf` & `ifunnygifmaker-1.0.3/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf`

 * *Files identical despite different names*

### Comparing `ifunnygifmaker-1.0.2/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-1.0.3/ifunnygifmaker/mememaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from PIL import Image, ImageDraw, ImageFont, ImageSequence
 
 from ifunnygifmaker.utils.image_utils import get_wrapped_text
 
 FONT_PATH = os.path.join(
     os.path.dirname(__file__), "fonts", "Futura Condensed Extra Bold.otf"
 )
-FONT_SIZE = 45
+FONT_SIZE = 38
 PADDING = 0.1
 
 
 class MemeMaker:
     def __init__(self, token):
         """
         An engine for making memes
```

### Comparing `ifunnygifmaker-1.0.2/ifunnygifmaker/utils/image_utils.py` & `ifunnygifmaker-1.0.3/ifunnygifmaker/utils/image_utils.py`

 * *Files identical despite different names*

