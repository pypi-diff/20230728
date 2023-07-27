# Comparing `tmp/abstract_gui-0.0.48.tar.gz` & `tmp/abstract_gui-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.48.tar", last modified: Thu Jul 27 22:30:55 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.49.tar", last modified: Thu Jul 27 23:27:21 2023, max compression
```

## Comparing `abstract_gui-0.0.48.tar` & `abstract_gui-0.0.49.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/
--rw-r--r--   0 root         (0) root         (0)     3800 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.48/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.48/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1122 2023-07-27 22:30:51.000000 abstract_gui-0.0.48/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.48/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.48/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.48/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.48/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.48/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    11222 2023-07-27 22:29:11.000000 abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:55.748497 abstract_gui-0.0.48/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3800 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 22:30:55.000000 abstract_gui-0.0.48/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.49/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.49/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1122 2023-07-27 23:27:18.000000 abstract_gui-0.0.49/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.49/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.49/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.49/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.49/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.49/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.49/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11722 2023-07-27 23:26:13.000000 abstract_gui-0.0.49/src/abstract_gui/simple_gui/gui_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:27:21.077935 abstract_gui-0.0.49/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3800 2023-07-27 23:27:21.000000 abstract_gui-0.0.49/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 23:27:21.000000 abstract_gui-0.0.49/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 23:27:21.000000 abstract_gui-0.0.49/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 23:27:21.000000 abstract_gui-0.0.49/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 23:27:21.000000 abstract_gui-0.0.49/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.48/PKG-INFO` & `abstract_gui-0.0.49/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract_gui
-Version: 0.0.48
+Name: abstract-gui
+Version: 0.0.49
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.48/README.md` & `abstract_gui-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.48/setup.py` & `abstract_gui-0.0.49/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.48',
+    version='0.0.49',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.48/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.49/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.48/src/abstract_gui/main.py` & `abstract_gui-0.0.49/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.49/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.48/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.49/src/abstract_gui/simple_gui/gui_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 def get_all_windows():
     glob = get_global_from_registry(registry_name)
     return glob['all_windows']
 def get_window_from_global(obj:str):
     glob = get_global_from_registry(registry_name)
     if obj in glob:
         return glob[obj]
+def update_window_to_registry(win,win_name:str ='default_window'):
+    windows =get_all_windows()
+    if win_name in windows:
+        win_name = create_win_name(win_name=win_name)
+    windows[win_name]={'name': win_name, 'values': {}, 'event': ''}
+    update_registry(var='all_windows',windows,name=registry_name)
 def get_window(title: str = 'basic window', layout: list = [[]]):
     """
     Returns a callable object for creating a PySimpleGUI window with the specified title and layout.
 
     Args:
         title (str): The title of the window.
         layout (list): The layout of the window.
@@ -125,31 +131,35 @@
     Checks if the given object is out of the specified upper and lower bounds.
 
     Args:
         upper (int or float): The upper bound.
         lower (int or float): The lower bound.
         obj (int or float): The object to check.
 
-    Returns:
         bool: True if the object is out of bounds, False otherwise.
     """
     return det_bool_T(obj > 100 or obj < 0)
 
-def create_win_name():
+def create_win_name(win_name:str='default_window'):
     """
     Generates a unique window name based on the existing window names.
 
     Returns:
         str: The generated unique window name.
     """
     all_windows = get_all_windows()
     keys = get_keys(all_windows)
-    i, curr_try = 'default_window', 0
+    curr_try,i = win_name, 0
+    if '_' in win_name:
+        num = win_name.split('_')[-1]
+        if is_number(num):
+          i=int(num)
+          win_name= win_name[:-len(in_name.split('_')[-1]+1)]
     while curr_try in keys:
-        curr_try = f'default_window_{i}'
+        curr_try = f'{win_name}_{i}'
         i += 1
     return curr_try
 
 def update_read(curr_win: type(get_window()), win_name: str = create_win_name()):
     """
     Updates the current window's event and values based on the latest user input.
 
@@ -244,15 +254,15 @@
 def get_last_window():
     """
     Returns the name of the last opened window.
 
     Returns:
         str: The name of the last opened window.
     """
-    return ret_globals('all_windows')['last_window']['name']
+    return get_window_from_global('all_windows')['last_window']['name']
 
 def while_progress(win=None, progress: int = 0, step: int = 5, thread=None):
     """
     Executes a while loop with a progress bar in a PySimpleGUI window.
 
     Args:
         win: The window to display the progress bar. If not provided, it uses the last opened window.
```

### Comparing `abstract_gui-0.0.48/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.49/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract-gui
-Version: 0.0.48
+Name: abstract_gui
+Version: 0.0.49
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

