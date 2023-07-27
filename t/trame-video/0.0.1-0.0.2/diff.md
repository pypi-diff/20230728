# Comparing `tmp/trame-video-0.0.1.tar.gz` & `tmp/trame-video-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-video-0.0.1.tar", last modified: Thu Jul 27 22:36:42 2023, max compression
+gzip compressed data, was "trame-video-0.0.2.tar", last modified: Thu Jul 27 22:55:14 2023, max compression
```

## Comparing `trame-video-0.0.1.tar` & `trame-video-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.254881 trame-video-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-07-27 22:36:34.000000 trame-video-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-27 22:36:34.000000 trame-video-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 22:36:42.254881 trame-video-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2023-07-27 22:36:34.000000 trame-video-0.0.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      889 2023-07-27 22:36:42.254881 trame-video-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 22:36:34.000000 trame-video-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.250881 trame-video-0.0.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.250881 trame-video-0.0.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame/modules/video.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.250881 trame-video-0.0.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame/widgets/video.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.250881 trame-video-0.0.1/trame_video/
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame_video/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.254881 trame-video-0.0.1/trame_video/module/
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame_video/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.254881 trame-video-0.0.1/trame_video/module/serve/
--rw-r--r--   0 root         (0) root         (0)   299042 2023-07-27 22:36:35.000000 trame-video-0.0.1/trame_video/module/serve/trame-fabric.js
--rw-r--r--   0 root         (0) root         (0)    30008 2023-07-27 22:36:35.000000 trame-video-0.0.1/trame_video/module/serve/trame-panzoom.js
--rw-r--r--   0 root         (0) root         (0)     3001 2023-07-27 22:36:38.000000 trame-video-0.0.1/trame_video/module/serve/trame-videothing-comp.css
--rw-r--r--   0 root         (0) root         (0)   552875 2023-07-27 22:36:38.000000 trame-video-0.0.1/trame_video/module/serve/trame-videothing-comp.js
--rw-r--r--   0 root         (0) root         (0)    43092 2023-07-27 22:36:37.000000 trame-video-0.0.1/trame_video/module/serve/trame-videothing.js
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame_video/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.254881 trame-video-0.0.1/trame_video/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame_video/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-07-27 22:36:34.000000 trame-video-0.0.1/trame_video/widgets/video.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:36:42.250881 trame-video-0.0.1/trame_video.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 22:36:42.000000 trame-video-0.0.1/trame_video.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      711 2023-07-27 22:36:42.000000 trame-video-0.0.1/trame_video.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 22:36:42.000000 trame-video-0.0.1/trame_video.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 22:36:42.000000 trame-video-0.0.1/trame_video.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-27 22:36:42.000000 trame-video-0.0.1/trame_video.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.926652 trame-video-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-07-27 22:55:03.000000 trame-video-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-27 22:55:03.000000 trame-video-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 22:55:14.926652 trame-video-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2023-07-27 22:55:03.000000 trame-video-0.0.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      889 2023-07-27 22:55:14.926652 trame-video-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 22:55:03.000000 trame-video-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.922652 trame-video-0.0.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.922652 trame-video-0.0.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame/modules/video.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.922652 trame-video-0.0.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame/widgets/video.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.922652 trame-video-0.0.2/trame_video/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.926652 trame-video-0.0.2/trame_video/module/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.926652 trame-video-0.0.2/trame_video/module/serve/
+-rw-r--r--   0 root         (0) root         (0)   299042 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/module/serve/trame-fabric.js
+-rw-r--r--   0 root         (0) root         (0)    30008 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/module/serve/trame-panzoom.js
+-rw-r--r--   0 root         (0) root         (0)     3001 2023-07-27 22:55:12.000000 trame-video-0.0.2/trame_video/module/serve/trame-videothing-comp.css
+-rw-r--r--   0 root         (0) root         (0)   552875 2023-07-27 22:55:10.000000 trame-video-0.0.2/trame_video/module/serve/trame-videothing-comp.js
+-rw-r--r--   0 root         (0) root         (0)    43092 2023-07-27 22:55:06.000000 trame-video-0.0.2/trame_video/module/serve/trame-videothing.js
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.926652 trame-video-0.0.2/trame_video/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2023-07-27 22:55:03.000000 trame-video-0.0.2/trame_video/widgets/video.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:55:14.922652 trame-video-0.0.2/trame_video.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 22:55:14.000000 trame-video-0.0.2/trame_video.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      711 2023-07-27 22:55:14.000000 trame-video-0.0.2/trame_video.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 22:55:14.000000 trame-video-0.0.2/trame_video.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 22:55:14.000000 trame-video-0.0.2/trame_video.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-27 22:55:14.000000 trame-video-0.0.2/trame_video.egg-info/top_level.txt
```

### Comparing `trame-video-0.0.1/LICENSE` & `trame-video-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/PKG-INFO` & `trame-video-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-video
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trame wrapper to vue @videothing components
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-video-0.0.1/setup.cfg` & `trame-video-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-video
-version = 0.0.1
+version = 0.0.2
 description = Trame wrapper to vue @videothing components
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-video-0.0.1/trame_video/module/serve/trame-fabric.js` & `trame-video-0.0.2/trame_video/module/serve/trame-fabric.js`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/trame_video/module/serve/trame-panzoom.js` & `trame-video-0.0.2/trame_video/module/serve/trame-panzoom.js`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/trame_video/module/serve/trame-videothing-comp.css` & `trame-video-0.0.2/trame_video/module/serve/trame-videothing-comp.css`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/trame_video/module/serve/trame-videothing-comp.js` & `trame-video-0.0.2/trame_video/module/serve/trame-videothing-comp.js`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/trame_video/module/serve/trame-videothing.js` & `trame-video-0.0.2/trame_video/module/serve/trame-videothing.js`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/trame_video/module/vue2.py` & `trame-video-0.0.2/trame_video/module/vue2.py`

 * *Files identical despite different names*

### Comparing `trame-video-0.0.1/trame_video.egg-info/PKG-INFO` & `trame-video-0.0.2/trame_video.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-video
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trame wrapper to vue @videothing components
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-video-0.0.1/trame_video.egg-info/SOURCES.txt` & `trame-video-0.0.2/trame_video.egg-info/SOURCES.txt`

 * *Files identical despite different names*

