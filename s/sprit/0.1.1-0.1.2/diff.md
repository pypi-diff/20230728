# Comparing `tmp/sprit-0.1.1.tar.gz` & `tmp/sprit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprit-0.1.1.tar", last modified: Thu Jul 27 20:01:25 2023, max compression
+gzip compressed data, was "sprit-0.1.2.tar", last modified: Fri Jul 28 21:52:36 2023, max compression
```

## Comparing `sprit-0.1.1.tar` & `sprit-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:25.308226 sprit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 20:01:14.000000 sprit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-27 20:01:25.308226 sprit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-27 20:01:14.000000 sprit-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 20:01:14.000000 sprit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:01:25.308226 sprit-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-27 20:01:14.000000 sprit-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:25.304226 sprit-0.1.1/sprit/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:25.308226 sprit-0.1.1/sprit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/rs3dv7_metadata.inv
--rw-r--r--   0 runner    (1001) docker     (123)   536638 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/sprit_icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/sprit_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/sprit_icon.xcf
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/sprit_icon_alpha.ico
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/sprit_icon_thickly.xcf
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/resources/todo.md
--rw-r--r--   0 runner    (1001) docker     (123)   195150 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/sprit.py
--rw-r--r--   0 runner    (1001) docker     (123)   139040 2023-07-27 20:01:14.000000 sprit-0.1.1/sprit/sprit_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:25.304226 sprit-0.1.1/sprit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-27 20:01:25.000000 sprit-0.1.1/sprit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 20:01:25.000000 sprit-0.1.1/sprit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:01:25.000000 sprit-0.1.1/sprit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 20:01:25.000000 sprit-0.1.1/sprit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 20:01:25.000000 sprit-0.1.1/sprit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.681313 sprit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 21:52:24.000000 sprit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-28 21:52:36.681313 sprit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-28 21:52:24.000000 sprit-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-28 21:52:24.000000 sprit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:52:36.681313 sprit-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 21:52:24.000000 sprit-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.677313 sprit-0.1.2/sprit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.681313 sprit-0.1.2/sprit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/rs3dv7_metadata.inv
+-rw-r--r--   0 runner    (1001) docker     (123)   536638 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon_alpha.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon_thickly.xcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.681313 sprit-0.1.2/sprit/resources/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/themes/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/todo.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195150 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/sprit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139236 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/sprit_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.677313 sprit-0.1.2/sprit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/top_level.txt
```

### Comparing `sprit-0.1.1/LICENSE` & `sprit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/PKG-INFO` & `sprit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

### Comparing `sprit-0.1.1/README.md` & `sprit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/pyproject.toml` & `sprit-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprit"
 dynamic = ["readme"]
 license = {file = "LICENSE"}
-version="0.1.1"
+version="0.1.2"
 description = "A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data"
 keywords = ["HVSR", "seismic", "horizontal to vertical spectral ratio", "obspy", 'geology', 'geophysics', 'geotechnical']
 requires-python = ">=3.9"
 dependencies =  ["obspy", "scipy", "matplotlib", "pandas", "numpy", "pyqt5", "tkcalendar"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Science/Research",
```

### Comparing `sprit-0.1.1/sprit/__init__.py` & `sprit-0.1.2/sprit/__init__.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/resources/rs3dv7_metadata.inv` & `sprit-0.1.2/sprit/resources/rs3dv7_metadata.inv`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/resources/sprit_icon.ico` & `sprit-0.1.2/sprit/resources/sprit_icon.ico`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/resources/sprit_icon.png` & `sprit-0.1.2/sprit/resources/sprit_icon.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/resources/sprit_icon.xcf` & `sprit-0.1.2/sprit/resources/sprit_icon.xcf`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/resources/sprit_icon_alpha.ico` & `sprit-0.1.2/sprit/resources/sprit_icon_alpha.ico`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/resources/sprit_icon_thickly.xcf` & `sprit-0.1.2/sprit/resources/sprit_icon_thickly.xcf`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/sprit.py` & `sprit-0.1.2/sprit/sprit.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.1/sprit/sprit_gui.py` & `sprit-0.1.2/sprit/sprit_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 
 class App:
     def __init__(self, master):
         self.master = master
         self.master.title("SPRIT")
 
         # Set the theme
-        self.darkthemepath = os.path.abspath("./themes/forest-dark.tcl")
-        self.lightthemepath = os.path.abspath("./themes/forest-light.tcl")
+        self.darkthemepath = pathlib.Path(pkg_resources.resource_filename(__name__, "/resources/themes/forest-dark.tcl"))
+        self.lightthemepath = pathlib.Path(pkg_resources.resource_filename(__name__, "/resources/themes/forest-light.tcl"))
         
         # Create the style object
         self.style = ttk.Style(master)
-        self.style.theme_use('default')
+        root.tk.call('source', self.lightthemepath)
+        #self.style.theme_use('default')
+        self.style.theme_use('forest-light')
 
         self.create_menubar()
         self.create_tabs()
 
         self.master.rowconfigure(0, weight=1)
         self.master.columnconfigure(0, weight=1)
```

### Comparing `sprit-0.1.1/sprit.egg-info/PKG-INFO` & `sprit-0.1.2/sprit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

