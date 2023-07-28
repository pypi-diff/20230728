# Comparing `tmp/kiri_walkgame-1.1.0.tar.gz` & `tmp/kiri_walkgame-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiri_walkgame-1.1.0.tar", max compression
+gzip compressed data, was "kiri_walkgame-1.2.0.tar", max compression
```

## Comparing `kiri_walkgame-1.1.0.tar` & `kiri_walkgame-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/LICENSE
--rw-r--r--   0        0        0      563 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/README.md
--rw-r--r--   0        0        0     8818 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/__init__.py
--rw-r--r--   0        0        0      177 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/__main__.py
--rw-r--r--   0        0        0     5533 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/characters.py
--rw-r--r--   0        0        0      838 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/output.py
--rw-r--r--   0        0        0     1788 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/shortcuts.py
--rw-r--r--   0        0        0  5256004 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/audios/Fantasy_by_Pufino_on_freetouse_com.mp3
--rw-r--r--   0        0        0      337 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/box.png
--rw-r--r--   0        0        0      898 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/refresh.png
--rw-r--r--   0        0        0     1016 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/voice_off.png
--rw-r--r--   0        0        0      899 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/voice_on.png
--rw-r--r--   0        0        0      703 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/run.png
--rw-r--r--   0        0        0      647 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/stand.png
--rw-r--r--   0        0        0    97861 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/logo.png
--rw-r--r--   0        0        0      532 2023-07-21 08:54:13.393527 kiri_walkgame-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 kiri_walkgame-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-28 03:13:53.172249 kiri_walkgame-1.2.0/LICENSE
+-rw-r--r--   0        0        0      562 2023-07-28 03:13:53.172249 kiri_walkgame-1.2.0/README.md
+-rw-r--r--   0        0        0    10344 2023-07-28 03:13:53.176249 kiri_walkgame-1.2.0/kiri_walkgame/__init__.py
+-rw-r--r--   0        0        0     5533 2023-07-28 03:13:53.176249 kiri_walkgame-1.2.0/kiri_walkgame/characters.py
+-rw-r--r--   0        0        0      838 2023-07-28 03:13:53.176249 kiri_walkgame-1.2.0/kiri_walkgame/output.py
+-rw-r--r--   0        0        0     1788 2023-07-28 03:13:53.176249 kiri_walkgame-1.2.0/kiri_walkgame/shortcuts.py
+-rw-r--r--   0        0        0  5256004 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/audios/Fantasy_by_Pufino_on_freetouse_com.mp3
+-rw-r--r--   0        0        0   125438 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/audios/meow.mp3
+-rw-r--r--   0        0        0      337 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/box.png
+-rw-r--r--   0        0        0      898 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/icons/refresh.png
+-rw-r--r--   0        0        0     1016 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/icons/voice_off.png
+-rw-r--r--   0        0        0      899 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/icons/voice_on.png
+-rw-r--r--   0        0        0      703 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/kiri/run.png
+-rw-r--r--   0        0        0      647 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/kiri/stand.png
+-rw-r--r--   0        0        0    97861 2023-07-28 03:13:53.208249 kiri_walkgame-1.2.0/kiri_walkgame/sources/logo.png
+-rw-r--r--   0        0        0      608 2023-07-28 03:13:53.672248 kiri_walkgame-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 kiri_walkgame-1.2.0/PKG-INFO
```

### Comparing `kiri_walkgame-1.1.0/LICENSE` & `kiri_walkgame-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/README.md` & `kiri_walkgame-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 This is a mini game to visualize the path-finding algorithm.
 
 To play this game, you just need to click the map twice. The first clicking will place a cat named **Kiri**, and the following one will place a box. Then Kiri will find his way to get inside the box immediately.
 
 ## Usage
 
 ```shell
-python kiri_walkgame
+kiri_walkgame -s 20
 ```
 
 ## Credits
 Music track: Fantasy by Pufino
 Source: https://freetouse.com/music
 Copyright Free Music for Video
```

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/characters.py` & `kiri_walkgame-1.2.0/kiri_walkgame/characters.py`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/output.py` & `kiri_walkgame-1.2.0/kiri_walkgame/output.py`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/shortcuts.py` & `kiri_walkgame-1.2.0/kiri_walkgame/shortcuts.py`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/audios/Fantasy_by_Pufino_on_freetouse_com.mp3` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/audios/Fantasy_by_Pufino_on_freetouse_com.mp3`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/refresh.png` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/voice_off.png` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/icons/voice_off.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/voice_on.png` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/icons/voice_on.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/run.png` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/kiri/run.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/stand.png` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/kiri/stand.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/kiri_walkgame/sources/logo.png` & `kiri_walkgame-1.2.0/kiri_walkgame/sources/logo.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.1.0/pyproject.toml` & `kiri_walkgame-1.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiri-walkgame"
-version = "1.1.0"
+version = "1.2.0"
 description = "a mini game to visualize the path-finding algorithm"
 authors = [ "anthony <mrchowpoor@gmail.com>" ]
 license = "MIT"
 repository = "https://github.com/kiri-chow/kiri-walkgame"
 readme = "README.md"
 
   [[tool.poetry.packages]]
@@ -12,10 +12,13 @@
 
   [tool.poetry.dependencies]
   python = "^3.9"
   kiri-pathfinding = "^1.2.0"
   pygame = "^2.5.0"
   pypng = "^0.20220715.0"
 
+[tool.poetry.plugins.console_scripts]
+kiri_walkgame = "kiri_walkgame:main"
+
 [build-system]
 requires = [ "poetry-core" ]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kiri_walkgame-1.1.0/PKG-INFO` & `kiri_walkgame-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiri-walkgame
-Version: 1.1.0
+Version: 1.2.0
 Summary: a mini game to visualize the path-finding algorithm
 Home-page: https://github.com/kiri-chow/kiri-walkgame
 License: MIT
 Author: anthony
 Author-email: mrchowpoor@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 This is a mini game to visualize the path-finding algorithm.
 
 To play this game, you just need to click the map twice. The first clicking will place a cat named **Kiri**, and the following one will place a box. Then Kiri will find his way to get inside the box immediately.
 
 ## Usage
 
 ```shell
-python kiri_walkgame
+kiri_walkgame -s 20
 ```
 
 ## Credits
 Music track: Fantasy by Pufino
 Source: https://freetouse.com/music
 Copyright Free Music for Video
```

