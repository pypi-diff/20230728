# Comparing `tmp/circadian_desktops-0.0.5.tar.gz` & `tmp/circadian_desktops-0.1.0.tar.gz`

## Comparing `circadian_desktops-0.0.5.tar` & `circadian_desktops-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/requirements.txt
--rw-r--r--   0        0        0   297003 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/screenshot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/__init__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/__main__.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/app.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/custom_qt.py
--rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/desktopUi.ui
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/functions.py
--rw-r--r--   0        0        0    18146 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/ui_mainwindow.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/clock.png
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/clock_32.png
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/clock_50.png
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/dawn.png
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/dawn_64.png
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/dawn_80.png
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/day.png
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/day_64.png
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/day_80.png
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/dusk.png
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/dusk_64.png
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/dusk_80.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/logo.ico
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/logo.png
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/night.png
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/night_64.png
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/night_80.png
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/preferences.png
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/preferences_32.png
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/preferences_50.png
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/screen.png
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/screen_32.png
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/src/circadian_desktops/Icons/screen_50.png
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/LICENSE
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 circadian_desktops-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/logo.png
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/requirements.txt
+-rw-r--r--   0        0        0   297003 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/screenshot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/__init__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/__main__.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/app.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/clean.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/custom_qt.py
+-rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/desktopUi.ui
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/functions.py
+-rw-r--r--   0        0        0    18146 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/ui_mainwindow.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/clock.png
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/clock_32.png
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/clock_50.png
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/dawn.png
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/dawn_64.png
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/dawn_80.png
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/day.png
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/day_64.png
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/day_80.png
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/dusk.png
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/dusk_64.png
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/dusk_80.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/logo.ico
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/logo.png
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/night.png
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/night_64.png
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/night_80.png
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/preferences.png
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/preferences_32.png
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/preferences_50.png
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/screen.png
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/screen_32.png
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/src/circadian_desktops/Icons/screen_50.png
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 circadian_desktops-0.1.0/PKG-INFO
```

### Comparing `circadian_desktops-0.0.5/screenshot.png` & `circadian_desktops-0.1.0/screenshot.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/app.py` & `circadian_desktops-0.1.0/src/circadian_desktops/app.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/custom_qt.py` & `circadian_desktops-0.1.0/src/circadian_desktops/custom_qt.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/desktopUi.ui` & `circadian_desktops-0.1.0/src/circadian_desktops/desktopUi.ui`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/functions.py` & `circadian_desktops-0.1.0/src/circadian_desktops/functions.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/ui_mainwindow.py` & `circadian_desktops-0.1.0/src/circadian_desktops/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/clock.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/clock.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/clock_32.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/clock_32.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/clock_50.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/clock_50.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/dawn.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/dawn.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/dawn_64.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/dawn_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/dawn_80.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/dawn_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/day.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/day.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/day_64.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/day_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/day_80.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/day_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/dusk.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/dusk.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/dusk_64.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/dusk_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/dusk_80.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/dusk_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/logo.ico` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/logo.ico`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/logo.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/logo.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/night.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/night.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/night_64.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/night_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/night_80.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/night_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/preferences.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/preferences.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/preferences_32.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/preferences_32.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/preferences_50.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/preferences_50.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/src/circadian_desktops/Icons/screen.png` & `circadian_desktops-0.1.0/src/circadian_desktops/Icons/screen.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/LICENSE` & `circadian_desktops-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.5/README.md` & `circadian_desktops-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CIRCADIAN DESKTOPS
+# ![Logo](logo.png) CIRCADIAN DESKTOPS 
 
 ## Description
 
 Circadian Desktops is a Python app for Windows 10 that changes your desktop background based on time of day.
 
 ![Screenshot](screenshot.png)
 
@@ -10,15 +10,15 @@
 Allows users to select different image files to use as desktop background during dawn, day, dust and night.
 A single image can be selected for each period or the app can be set to shuffle images from the selected image's folder.
 
 ### Transition Times
 The app determines image transition times based on sunrise and sunset times at the users location.
 This is calculated using two non-standard library Python modules:
 - [Geocoder](https://github.com/DenisCarriere/geocoder) - Retrieves the users location and timezone using their IP address.
-- [Astral](https://sffjunkie.github.io/astral/) - calculates sunrise and sunset times based on user location and the current date.
+- [Astral](https://sffjunkie.github.io/astral/) - Calculates sunrise and sunset times based on user location and the current date.
 
 Alternatively, the user can select their own times for images to transition.
 
 ### Preferences
 The app offers three additional options:
 - Dark Theme - Toggles the GUI between light and dark theme.
 - Minimize to tray - When selected the app will minimize to the system tray and continue running, instead of shutting down when the window in closed.
@@ -51,7 +51,8 @@
 - `__main__.py` - Entry point to run module as a script.
 - `app.py` - Primary script to run the app. Contains the MainWindow class and script to start app.
 - `functions.py` - Helper functions called by app.py. Handles functionality outside the GUI.
 - `ui_mainwindow.py` - Python script generated from destopUi.ui by `pyuic5`. Used as GUI layout for MainWindow in app.py.
 - `desktopUi.ui` - Widget layout for GUI generated by [Qt Designer](https://doc.qt.io/qt-6/qtdesigner-manual.html). Not required for app to run.
 - `custom_qt.py` - Contains a custom QtPalette class used for 'dark theme'.
 - `Icons/` - Folder with image files used in GUI and for Windows system icons.
+- `clean.py` - Run to remove traces of Circadian Desktop from you PC not contained in `src`, i.e. settings file and registry entry.
```

### Comparing `circadian_desktops-0.0.5/pyproject.toml` & `circadian_desktops-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "circadian_desktops"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Luke Hartley", email="luke.hartley05@gmail.com" },
 ]
 description = "An app that changes your desktop background based on time of day."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `circadian_desktops-0.0.5/PKG-INFO` & `circadian_desktops-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: circadian_desktops
-Version: 0.0.5
+Version: 0.1.0
 Summary: An app that changes your desktop background based on time of day.
 Project-URL: Homepage, https://github.com/Luke943/CircadianDesktops
 Project-URL: Bug Tracker, https://github.com/Luke943/CircadianDesktops/issues
 Author-email: Luke Hartley <luke.hartley05@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: astral
 Requires-Dist: geocoder
 Requires-Dist: pyqt5
 Description-Content-Type: text/markdown
 
-# CIRCADIAN DESKTOPS
+# ![Logo](logo.png) CIRCADIAN DESKTOPS 
 
 ## Description
 
 Circadian Desktops is a Python app for Windows 10 that changes your desktop background based on time of day.
 
 ![Screenshot](screenshot.png)
 
@@ -27,15 +27,15 @@
 Allows users to select different image files to use as desktop background during dawn, day, dust and night.
 A single image can be selected for each period or the app can be set to shuffle images from the selected image's folder.
 
 ### Transition Times
 The app determines image transition times based on sunrise and sunset times at the users location.
 This is calculated using two non-standard library Python modules:
 - [Geocoder](https://github.com/DenisCarriere/geocoder) - Retrieves the users location and timezone using their IP address.
-- [Astral](https://sffjunkie.github.io/astral/) - calculates sunrise and sunset times based on user location and the current date.
+- [Astral](https://sffjunkie.github.io/astral/) - Calculates sunrise and sunset times based on user location and the current date.
 
 Alternatively, the user can select their own times for images to transition.
 
 ### Preferences
 The app offers three additional options:
 - Dark Theme - Toggles the GUI between light and dark theme.
 - Minimize to tray - When selected the app will minimize to the system tray and continue running, instead of shutting down when the window in closed.
@@ -68,7 +68,8 @@
 - `__main__.py` - Entry point to run module as a script.
 - `app.py` - Primary script to run the app. Contains the MainWindow class and script to start app.
 - `functions.py` - Helper functions called by app.py. Handles functionality outside the GUI.
 - `ui_mainwindow.py` - Python script generated from destopUi.ui by `pyuic5`. Used as GUI layout for MainWindow in app.py.
 - `desktopUi.ui` - Widget layout for GUI generated by [Qt Designer](https://doc.qt.io/qt-6/qtdesigner-manual.html). Not required for app to run.
 - `custom_qt.py` - Contains a custom QtPalette class used for 'dark theme'.
 - `Icons/` - Folder with image files used in GUI and for Windows system icons.
+- `clean.py` - Run to remove traces of Circadian Desktop from you PC not contained in `src`, i.e. settings file and registry entry.
```

