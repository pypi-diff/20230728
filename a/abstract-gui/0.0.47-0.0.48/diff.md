# Comparing `tmp/abstract_gui-0.0.47.tar.gz` & `tmp/abstract_gui-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.47.tar", last modified: Thu Jul 27 22:26:01 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.48.tar", last modified: Thu Jul 27 22:30:55 2023, max compression
```

## Comparing `abstract_gui-0.0.47.tar` & `abstract_gui-0.0.48.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 john-putkey  (1000) john-putkey  (1000)        0 2023-07-27 22:25:55.872169 abstract_gui-0.0.47/
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)     3810 2023-07-27 22:26:01.080174 abstract_gui-0.0.47/PKG-INFO
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.47/README.md
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.47/pyproject.toml
--rw-r--r--   0 john-putkey  (1000) john-putkey  (1000)       38 2023-07-27 22:26:01.080174 abstract_gui-0.0.47/setup.cfg
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)     1132 2023-07-27 22:23:49.000000 abstract_gui-0.0.47/setup.py
-drwxrwxr-x   0 john-putkey  (1000) john-putkey  (1000)        0 2023-07-27 22:25:55.872169 abstract_gui-0.0.47/src/
-drwxrwxr-x   0 john-putkey  (1000) john-putkey  (1000)        0 2023-07-27 22:25:55.872169 abstract_gui-0.0.47/src/abstract_gui/
-drwxrwxr-x   0 john-putkey  (1000) john-putkey  (1000)        0 2023-07-27 22:25:55.872169 abstract_gui-0.0.47/src/abstract_gui/PyQt5/
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.47/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.47/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.47/src/abstract_gui/__init__.py
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.47/src/abstract_gui/main.py
-drwxrwxr-x   0 john-putkey  (1000) john-putkey  (1000)        0 2023-07-27 22:25:55.872169 abstract_gui-0.0.47/src/abstract_gui/simple_gui/
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.47/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.47/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 john-putkey  (1000) john-putkey  (1000)    11278 2023-07-27 22:11:43.000000 abstract_gui-0.0.47/src/abstract_gui/simple_gui/gui_template.py
-drwxrwxr-x   0 john-putkey  (1000) john-putkey  (1000)        0 2023-07-27 22:26:01.080174 abstract_gui-0.0.47/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3810 2023-07-27 22:26:01.000000 abstract_gui-0.0.47/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 22:26:01.000000 abstract_gui-0.0.47/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 22:26:01.000000 abstract_gui-0.0.47/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 22:26:01.000000 abstract_gui-0.0.47/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 22:26:01.000000 abstract_gui-0.0.47/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.48/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.48/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1122 2023-07-27 22:30:51.000000 abstract_gui-0.0.48/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.48/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.48/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.48/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.48/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.48/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11222 2023-07-27 22:29:11.000000 abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3800 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.47/PKG-INFO` & `abstract_gui-0.0.48/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.47
+Version: 0.0.48
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_gui-0.0.47/README.md` & `abstract_gui-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.47/setup.py` & `abstract_gui-0.0.48/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.47',
+    version='0.0.48',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui',
+    url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
     ],
```

### Comparing `abstract_gui-0.0.47/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.48/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.47/src/abstract_gui/main.py` & `abstract_gui-0.0.48/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.47/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.47/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,17 +217,15 @@
     values_all=[]
     if win is None:
         win = get_globes(string='window')
     while verify_window(win):
         event, values = win.read()
         if values != None:
             values_all = values
-        print(values_all)
         if win_closed(event):
-            print(values_all)
             return values_all
             break
     close_window(win)
     return values_all
 
 def single_call(win):
     """
```

### Comparing `abstract_gui-0.0.47/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.48/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.47
+Version: 0.0.48
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

