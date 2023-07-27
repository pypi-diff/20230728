# Comparing `tmp/ladybug-radiance-0.2.2.tar.gz` & `tmp/ladybug-radiance-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-radiance-0.2.2.tar", last modified: Sat Jul 22 02:57:45 2023, max compression
+gzip compressed data, was "dist/ladybug-radiance-0.2.3.tar", last modified: Thu Jul 27 23:57:56 2023, max compression
```

## Comparing `ladybug-radiance-0.2.2.tar` & `ladybug-radiance-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/display-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/skymatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance/study/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/study/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/study/directsun.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/study/radiation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/visualize/raddome.py
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/visualize/radrose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/ladybug_radiance/visualize/skydome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/ladybug_radiance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 02:57:45.000000 ladybug-radiance-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-22 02:56:38.000000 ladybug-radiance-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/display-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/skymatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance/study/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/study/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/study/directsun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/study/radiation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/visualize/raddome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/visualize/radrose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/ladybug_radiance/visualize/skydome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/ladybug_radiance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 23:57:56.000000 ladybug-radiance-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-27 23:56:57.000000 ladybug-radiance-0.2.3/setup.py
```

### Comparing `ladybug-radiance-0.2.2/LICENSE` & `ladybug-radiance-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/PKG-INFO` & `ladybug-radiance-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-radiance
-Version: 0.2.2
+Version: 0.2.3
 Summary: Radiance extension for Ladybug, used for all radiation studies and graphics.
 Home-page: https://github.com/ladybug-tools/ladybug-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ladybug-radiance-0.2.2/README.md` & `ladybug-radiance-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/dev-requirements.txt` & `ladybug-radiance-0.2.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/config.py` & `ladybug-radiance-0.2.3/ladybug_radiance/config.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/intersection.py` & `ladybug-radiance-0.2.3/ladybug_radiance/intersection.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/skymatrix.py` & `ladybug-radiance-0.2.3/ladybug_radiance/skymatrix.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/study/directsun.py` & `ladybug-radiance-0.2.3/ladybug_radiance/study/directsun.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/study/radiation.py` & `ladybug-radiance-0.2.3/ladybug_radiance/study/radiation.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/visualize/raddome.py` & `ladybug-radiance-0.2.3/ladybug_radiance/visualize/raddome.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/visualize/radrose.py` & `ladybug-radiance-0.2.3/ladybug_radiance/visualize/radrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance/visualize/skydome.py` & `ladybug-radiance-0.2.3/ladybug_radiance/visualize/skydome.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance.egg-info/PKG-INFO` & `ladybug-radiance-0.2.3/ladybug_radiance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-radiance
-Version: 0.2.2
+Version: 0.2.3
 Summary: Radiance extension for Ladybug, used for all radiation studies and graphics.
 Home-page: https://github.com/ladybug-tools/ladybug-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ladybug-radiance-0.2.2/ladybug_radiance.egg-info/SOURCES.txt` & `ladybug-radiance-0.2.3/ladybug_radiance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.2/setup.py` & `ladybug-radiance-0.2.3/setup.py`

 * *Files identical despite different names*

