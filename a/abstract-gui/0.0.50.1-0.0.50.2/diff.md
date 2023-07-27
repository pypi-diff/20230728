# Comparing `tmp/abstract_gui-0.0.50.1.tar.gz` & `tmp/abstract_gui-0.0.50.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.1.tar", last modified: Thu Jul 27 23:31:21 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.2.tar", last modified: Thu Jul 27 23:53:33 2023, max compression
```

## Comparing `abstract_gui-0.0.50.1.tar` & `abstract_gui-0.0.50.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/
--rw-r--r--   0 root         (0) root         (0)     3802 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.50.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.50.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-27 23:31:18.000000 abstract_gui-0.0.50.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:31:21.538281 abstract_gui-0.0.50.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.50.1/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.50.1/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.50.1/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.50.1/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.50.1/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.50.1/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-27 23:31:12.000000 abstract_gui-0.0.50.1/src/abstract_gui/simple_gui/gui_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:31:21.542281 abstract_gui-0.0.50.1/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3802 2023-07-27 23:31:21.000000 abstract_gui-0.0.50.1/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 23:31:21.000000 abstract_gui-0.0.50.1/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 23:31:21.000000 abstract_gui-0.0.50.1/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 23:31:21.000000 abstract_gui-0.0.50.1/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 23:31:21.000000 abstract_gui-0.0.50.1/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.50.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.50.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1134 2023-07-27 23:53:16.000000 abstract_gui-0.0.50.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.283817 abstract_gui-0.0.50.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.283817 abstract_gui-0.0.50.2/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.50.2/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.50.2/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-05-31 14:39:25.000000 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-27 23:31:12.000000 abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:53:33.287817 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3812 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-27 23:53:33.000000 abstract_gui-0.0.50.2/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.1/PKG-INFO` & `abstract_gui-0.0.50.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.50.1
+Version: 0.0.50.2
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_gui-0.0.50.1/README.md` & `abstract_gui-0.0.50.2/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.1/setup.py` & `abstract_gui-0.0.50.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.1',
+    version='0.0.50.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
+    url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
     ],
```

### Comparing `abstract_gui-0.0.50.1/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.1/src/abstract_gui/main.py` & `abstract_gui-0.0.50.2/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.1/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.1/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.2/src/abstract_gui/simple_gui/gui_template.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.1/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.2/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.50.1
+Version: 0.0.50.2
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

