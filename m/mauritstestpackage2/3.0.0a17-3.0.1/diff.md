# Comparing `tmp/mauritstestpackage2-3.0.0a17.tar.gz` & `tmp/mauritstestpackage2-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauritstestpackage2-3.0.0a17.tar", last modified: Thu Jul 13 12:46:30 2023, max compression
+gzip compressed data, was "mauritstestpackage2-3.0.1.tar", last modified: Fri Jul 28 18:51:12 2023, max compression
```

## Comparing `mauritstestpackage2-3.0.0a17.tar` & `mauritstestpackage2-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.320341 mauritstestpackage2-3.0.0a17/
--rw-r--r--   0 maurits    (501) staff       (20)     4597 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5317 2023-07-13 12:46:30.320476 mauritstestpackage2-3.0.0a17/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.318371 mauritstestpackage2-3.0.0a17/mauritstestpackage/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.316653 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.316727 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.318592 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.320005 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     5317 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       24 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-13 12:46:30.320827 mauritstestpackage2-3.0.0a17/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 18:51:12.388973 mauritstestpackage2-3.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     4725 2023-07-28 18:51:11.000000 mauritstestpackage2-3.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-28 18:51:11.000000 mauritstestpackage2-3.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5442 2023-07-28 18:51:12.389121 mauritstestpackage2-3.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-28 18:51:11.000000 mauritstestpackage2-3.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 18:51:12.386670 mauritstestpackage2-3.0.1/mauritstestpackage/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-28 18:51:11.000000 mauritstestpackage2-3.0.1/mauritstestpackage/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 18:51:12.384692 mauritstestpackage2-3.0.1/mauritstestpackage/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 18:51:12.384792 mauritstestpackage2-3.0.1/mauritstestpackage/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 18:51:12.387266 mauritstestpackage2-3.0.1/mauritstestpackage/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      554 2023-07-28 18:51:12.000000 mauritstestpackage2-3.0.1/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-28 18:51:11.000000 mauritstestpackage2-3.0.1/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 18:51:12.388713 mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     5442 2023-07-28 18:51:12.000000 mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      426 2023-07-28 18:51:12.000000 mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 18:51:12.000000 mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 18:51:12.000000 mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-07-28 18:51:12.000000 mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-28 18:51:12.389621 mauritstestpackage2-3.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1089 2023-07-28 18:51:11.000000 mauritstestpackage2-3.0.1/setup.py
```

### Comparing `mauritstestpackage2-3.0.0a17/CHANGES.rst` & `mauritstestpackage2-3.0.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+3.0.1 (2023-07-28)
+------------------
+
+- Nothing changed yet.
+
+
+3.0.0 (2023-07-28)
+------------------
+
+- Nothing changed yet.
+
+
 3.0.0a17 (2023-07-13)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a16 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a17/PKG-INFO` & `mauritstestpackage2-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mauritstestpackage2
-Version: 3.0.0a17
+Version: 3.0.1
 Summary: Test package from Maurits for uploading to PyPI.
 Home-page: https://github.com/mauritsvanrees/mauritstestpackage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: test release pypi
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,26 @@
 
 Maurits van Rees
 
 
 Changelog
 =========
 
+3.0.1 (2023-07-28)
+------------------
+
+- Nothing changed yet.
+
+
+3.0.0 (2023-07-28)
+------------------
+
+- Nothing changed yet.
+
+
 3.0.0a17 (2023-07-13)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a16 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po` & `mauritstestpackage2-3.0.1/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po`

 * *Files identical despite different names*

### Comparing `mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/PKG-INFO` & `mauritstestpackage2-3.0.1/mauritstestpackage2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mauritstestpackage2
-Version: 3.0.0a17
+Version: 3.0.1
 Summary: Test package from Maurits for uploading to PyPI.
 Home-page: https://github.com/mauritsvanrees/mauritstestpackage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: test release pypi
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,26 @@
 
 Maurits van Rees
 
 
 Changelog
 =========
 
+3.0.1 (2023-07-28)
+------------------
+
+- Nothing changed yet.
+
+
+3.0.0 (2023-07-28)
+------------------
+
+- Nothing changed yet.
+
+
 3.0.0a17 (2023-07-13)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a16 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a17/setup.py` & `mauritstestpackage2-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 
-version = "3.0.0a17"
+version = "3.0.1"
 
 setup(
     name="mauritstestpackage2",
     version=version,
     description="Test package from Maurits for uploading to PyPI.",
     long_description=(open("README.rst").read() + "\n\n" + open("CHANGES.rst").read()),
     # Get strings from https://pypi.org/classifiers/
```

