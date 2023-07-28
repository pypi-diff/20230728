# Comparing `tmp/gog_price_checker-0.1.0.tar.gz` & `tmp/gog_price_checker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.0.tar", last modified: Fri Jul 28 14:20:15 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.1.tar", last modified: Fri Jul 28 14:23:41 2023, max compression
```

## Comparing `gog_price_checker-0.1.0.tar` & `gog_price_checker-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:20:15.324955 gog_price_checker-0.1.0/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3566 2023-07-28 14:20:15.324792 gog_price_checker-0.1.0/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)     3119 2023-07-28 13:18:52.000000 gog_price_checker-0.1.0/README.md
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:20:15.323674 gog_price_checker-0.1.0/gog_price_checker/
--rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 14:12:13.000000 gog_price_checker-0.1.0/gog_price_checker/__init__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     3217 2023-07-28 14:09:47.000000 gog_price_checker-0.1.0/gog_price_checker/__main__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 14:07:57.000000 gog_price_checker-0.1.0/gog_price_checker/countries.py
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:20:15.324536 gog_price_checker-0.1.0/gog_price_checker.egg-info/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3566 2023-07-28 14:20:15.000000 gog_price_checker-0.1.0/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 14:20:15.000000 gog_price_checker-0.1.0/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 14:20:15.000000 gog_price_checker-0.1.0/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 14:20:15.000000 gog_price_checker-0.1.0/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 14:20:15.000000 gog_price_checker-0.1.0/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 14:20:15.325016 gog_price_checker-0.1.0/setup.cfg
--rw-r--r--   0 alexpopov   (501) staff       (20)      786 2023-07-28 14:14:48.000000 gog_price_checker-0.1.0/setup.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:23:41.370661 gog_price_checker-0.1.1/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:23:41.370337 gog_price_checker-0.1.1/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3119 2023-07-28 13:18:52.000000 gog_price_checker-0.1.1/README.md
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:23:41.368472 gog_price_checker-0.1.1/gog_price_checker/
+-rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 14:12:13.000000 gog_price_checker-0.1.1/gog_price_checker/__init__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3217 2023-07-28 14:09:47.000000 gog_price_checker-0.1.1/gog_price_checker/__main__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 14:07:57.000000 gog_price_checker-0.1.1/gog_price_checker/countries.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:23:41.369494 gog_price_checker-0.1.1/gog_price_checker.egg-info/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:23:41.000000 gog_price_checker-0.1.1/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 14:23:41.000000 gog_price_checker-0.1.1/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 14:23:41.000000 gog_price_checker-0.1.1/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 14:23:41.000000 gog_price_checker-0.1.1/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 14:23:41.000000 gog_price_checker-0.1.1/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 14:23:41.370750 gog_price_checker-0.1.1/setup.cfg
+-rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 14:23:32.000000 gog_price_checker-0.1.1/setup.py
```

### Comparing `gog_price_checker-0.1.0/PKG-INFO` & `gog_price_checker-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gog_price_checker
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to check game prices from GOG API
-Home-page: https://github.com/iampopovich/game_price_checker
+Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gog_price_checker-0.1.0/README.md` & `gog_price_checker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.0/gog_price_checker/__main__.py` & `gog_price_checker-0.1.1/gog_price_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.0/gog_price_checker/countries.py` & `gog_price_checker-0.1.1/gog_price_checker/countries.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.0/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.1/gog_price_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to check game prices from GOG API
-Home-page: https://github.com/iampopovich/game_price_checker
+Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gog_price_checker-0.1.0/setup.py` & `gog_price_checker-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.0",
+    version="0.1.1",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/iampopovich/game_price_checker",
+    url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
     entry_points={
         "console_scripts": [
             "gog_price_checker = gog_price_checker.__main__:main"
         ]
     },
     classifiers=[
```

