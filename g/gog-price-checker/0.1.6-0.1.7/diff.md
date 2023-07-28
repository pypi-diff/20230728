# Comparing `tmp/gog_price_checker-0.1.6.tar.gz` & `tmp/gog_price_checker-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.6.tar", last modified: Fri Jul 28 15:32:58 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.7.tar", last modified: Fri Jul 28 15:40:19 2023, max compression
```

## Comparing `gog_price_checker-0.1.6.tar` & `gog_price_checker-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:32:58.740218 gog_price_checker-0.1.6/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:32:58.740061 gog_price_checker-0.1.6/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)     3286 2023-07-28 15:15:44.000000 gog_price_checker-0.1.6/README.md
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:32:58.738902 gog_price_checker-0.1.6/gog_price_checker/
--rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 15:15:44.000000 gog_price_checker-0.1.6/gog_price_checker/__init__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     3227 2023-07-28 15:30:50.000000 gog_price_checker-0.1.6/gog_price_checker/__main__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 15:15:44.000000 gog_price_checker-0.1.6/gog_price_checker/countries.py
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:32:58.739813 gog_price_checker-0.1.6/gog_price_checker.egg-info/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 15:32:58.740279 gog_price_checker-0.1.6/setup.cfg
--rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 15:32:25.000000 gog_price_checker-0.1.6/setup.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:40:19.335054 gog_price_checker-0.1.7/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:40:19.334859 gog_price_checker-0.1.7/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3286 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/README.md
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:40:19.333630 gog_price_checker-0.1.7/gog_price_checker/
+-rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/gog_price_checker/__init__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3227 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/gog_price_checker/__main__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/gog_price_checker/countries.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:40:19.334565 gog_price_checker-0.1.7/gog_price_checker.egg-info/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 15:40:19.335128 gog_price_checker-0.1.7/setup.cfg
+-rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 15:40:08.000000 gog_price_checker-0.1.7/setup.py
```

### Comparing `gog_price_checker-0.1.6/PKG-INFO` & `gog_price_checker-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gog_price_checker
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gog_price_checker-0.1.6/README.md` & `gog_price_checker-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.6/gog_price_checker/__main__.py` & `gog_price_checker-0.1.7/gog_price_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.6/gog_price_checker/countries.py` & `gog_price_checker-0.1.7/gog_price_checker/countries.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.6/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.7/gog_price_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gog_price_checker-0.1.6/setup.py` & `gog_price_checker-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.6",
+    version="0.1.7",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
```

