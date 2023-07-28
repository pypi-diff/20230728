# Comparing `tmp/abstract_gui-0.0.50.2.tar.gz` & `tmp/abstract_gui-0.0.50.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.2.tar", last modified: Thu Jul 27 23:53:33 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.3.tar", last modified: Fri Jul 28 01:18:17 2023, max compression
```

## Comparing `abstract_gui-0.0.50.2.tar` & `abstract_gui-0.0.50.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/
--rw-r--r--   0 root         (0) root         (0)     3812 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.50.2/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.50.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1134 2023-07-27 23:53:16.000000 abstract_gui-0.0.50.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.283817 abstract_gui-0.0.50.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.283817 abstract_gui-0.0.50.2/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.50.2/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.50.2/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-27 23:31:12.000000 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3812 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 01:18:17.145642 abstract_gui-0.0.50.3/
+-rw-r--r--   0 root         (0) root         (0)     3833 2023-07-28 01:18:17.145642 abstract_gui-0.0.50.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3086 2023-07-28 00:06:19.000000 abstract_gui-0.0.50.3/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-28 01:18:17.145642 abstract_gui-0.0.50.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1134 2023-07-28 01:17:54.000000 abstract_gui-0.0.50.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 01:18:17.141642 abstract_gui-0.0.50.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 01:18:17.141642 abstract_gui-0.0.50.3/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 01:18:17.141642 abstract_gui-0.0.50.3/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 01:18:17.145642 abstract_gui-0.0.50.3/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.3/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11971 2023-07-28 01:17:30.000000 abstract_gui-0.0.50.3/src/abstract_gui/simple_gui/gui_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 01:18:17.141642 abstract_gui-0.0.50.3/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3833 2023-07-28 01:18:17.000000 abstract_gui-0.0.50.3/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-07-28 01:18:17.000000 abstract_gui-0.0.50.3/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-28 01:18:17.000000 abstract_gui-0.0.50.3/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-28 01:18:17.000000 abstract_gui-0.0.50.3/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-28 01:18:17.000000 abstract_gui-0.0.50.3/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.2/PKG-INFO` & `abstract_gui-0.0.50.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.50.2
+Version: 0.0.50.3
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,29 +13,29 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # abstract_gui
 
 This is a Python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 
-This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/abstract_gui/`.
+This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/tree/main/abstract_gui/`.
 
 ## Installation
 
 You can install the `abstract_gui` module via pip:
 
 ```sh
 pip install abstract_gui
 ```
 
 You can also install it directly from the source:
 
 ```sh
-git clone https://github.io/abstract_endeavors/abstract_essentials/abstract_gui/
-cd abstract_gui
+git clone https://github.com/AbstractEndeavors/abstract_essentials.git
+cd abstract_essentials/abstract_gui
 python setup.py install
 ```
 
 ## Usage
 
 Here's an example of how to use the `abstract_gui` module:
 
@@ -112,8 +112,8 @@
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 * putkoff - main developer
 
-This README file was last updated on May 29, 2023.
+This README file was last updated on july 29, 2023.
```

### Comparing `abstract_gui-0.0.50.2/README.md` & `abstract_gui-0.0.50.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # abstract_gui
 
 This is a Python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 
-This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/abstract_gui/`.
+This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/tree/main/abstract_gui/`.
 
 ## Installation
 
 You can install the `abstract_gui` module via pip:
 
 ```sh
 pip install abstract_gui
 ```
 
 You can also install it directly from the source:
 
 ```sh
-git clone https://github.io/abstract_endeavors/abstract_essentials/abstract_gui/
-cd abstract_gui
+git clone https://github.com/AbstractEndeavors/abstract_essentials.git
+cd abstract_essentials/abstract_gui
 python setup.py install
 ```
 
 ## Usage
 
 Here's an example of how to use the `abstract_gui` module:
 
@@ -97,8 +97,8 @@
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 * putkoff - main developer
 
-This README file was last updated on May 29, 2023.
+This README file was last updated on july 29, 2023.
```

### Comparing `abstract_gui-0.0.50.2/setup.py` & `abstract_gui-0.0.50.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.2',
+    version='0.0.50.3',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.3/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.2/src/abstract_gui/main.py` & `abstract_gui-0.0.50.3/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.3/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.3/src/abstract_gui/simple_gui/gui_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,29 @@
         return glob[obj]
 def update_window_to_registry(win,win_name:str ='default_window'):
     windows =get_all_windows()
     if win_name in windows:
         win_name = create_win_name(win_name=win_name)
     windows[win_name]={'name': win_name, 'values': {}, 'event': ''}
     update_registry(var='all_windows',val=windows,name=registry_name)
+    update_registry(var=win_name, val=win,name=registry_name)
 def get_window(title: str = 'basic window', layout: list = [[]]):
     """
     Returns a callable object for creating a PySimpleGUI window with the specified title and layout.
 
     Args:
         title (str): The title of the window.
         layout (list): The layout of the window.
 
     Returns:
         callable: A callable object that creates the PySimpleGUI window when called.
     """
-    return get_gui_fun(name='Window', args={"title": title, "layout": layout})
+    win = get_gui_fun(name='Window', args={"title": title, "layout": layout})
+    update_window_to_registry(win,win_name=title)
+    return win
 
 def verify_window(win: any = None) -> bool:
     """
     Verifies if the given object is a valid PySimpleGUI window.
 
     Args:
         win (any): The object to verify.
@@ -224,14 +227,16 @@
 
     Args:
         win: The window to handle events for. If not provided, it uses the 'window' global object.
     """
     values_all=[]
     if win is None:
         win = get_globes(string='window')
+    if type(win) is str:
+        win = get_window_from_global(win)
     while verify_window(win):
         event, values = win.read()
         if values != None:
             values_all = values
         if win_closed(event):
             return values_all
             break
```

### Comparing `abstract_gui-0.0.50.2/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.3/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.50.2
+Version: 0.0.50.3
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,29 +13,29 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # abstract_gui
 
 This is a Python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 
-This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/abstract_gui/`.
+This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/tree/main/abstract_gui/`.
 
 ## Installation
 
 You can install the `abstract_gui` module via pip:
 
 ```sh
 pip install abstract_gui
 ```
 
 You can also install it directly from the source:
 
 ```sh
-git clone https://github.io/abstract_endeavors/abstract_essentials/abstract_gui/
-cd abstract_gui
+git clone https://github.com/AbstractEndeavors/abstract_essentials.git
+cd abstract_essentials/abstract_gui
 python setup.py install
 ```
 
 ## Usage
 
 Here's an example of how to use the `abstract_gui` module:
 
@@ -112,8 +112,8 @@
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 * putkoff - main developer
 
-This README file was last updated on May 29, 2023.
+This README file was last updated on july 29, 2023.
```

