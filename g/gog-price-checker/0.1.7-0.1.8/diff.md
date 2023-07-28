# Comparing `tmp/gog_price_checker-0.1.7.tar.gz` & `tmp/gog_price_checker-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.7.tar", last modified: Fri Jul 28 15:40:19 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.8.tar", last modified: Fri Jul 28 16:22:59 2023, max compression
```

## Comparing `gog_price_checker-0.1.7.tar` & `gog_price_checker-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:40:19.335054 gog_price_checker-0.1.7/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:40:19.334859 gog_price_checker-0.1.7/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)     3286 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/README.md
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:40:19.333630 gog_price_checker-0.1.7/gog_price_checker/
--rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/gog_price_checker/__init__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     3227 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/gog_price_checker/__main__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 15:39:30.000000 gog_price_checker-0.1.7/gog_price_checker/countries.py
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:40:19.334565 gog_price_checker-0.1.7/gog_price_checker.egg-info/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 15:40:19.000000 gog_price_checker-0.1.7/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 15:40:19.335128 gog_price_checker-0.1.7/setup.cfg
--rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 15:40:08.000000 gog_price_checker-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/gog_price_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/gog_price_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/gog_price_checker/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/gog_price_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/setup.py
```

### Comparing `gog_price_checker-0.1.7/PKG-INFO` & `gog_price_checker-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: gog_price_checker
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
@@ -23,15 +21,15 @@
 - Requests library (for making HTTP requests)
 - Regular expressions (re) module
 - Threading module (for concurrent requests)
 - Logging module (for logging)
 
 ## Installation
 ```
-pip instal gog_price_checker
+pip install gog-price-checker
 ```
 
 ## How to Use
 
 1. Copy a URL containing a game page (e.g., `https://www.gog.com/game/diablo`) to the clipboard.
 
 2. Run the Python script with the following arguments:
@@ -83,9 +81,7 @@
 ## License
 
 - The **Game Price Checker** Python script is released under the [MIT License](LICENSE). Feel free to modify and distribute the script according to the terms of the license.
 
 ## Disclaimer
 
 - The author of this script is not responsible for any misuse or consequences of using the script on unauthorized websites. Always make sure you have the right to access and use the data from the websites you interact with.
-
-
```

### Comparing `gog_price_checker-0.1.7/README.md` & `gog_price_checker-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - Requests library (for making HTTP requests)
 - Regular expressions (re) module
 - Threading module (for concurrent requests)
 - Logging module (for logging)
 
 ## Installation
 ```
-pip instal gog_price_checker
+pip install gog-price-checker
 ```
 
 ## How to Use
 
 1. Copy a URL containing a game page (e.g., `https://www.gog.com/game/diablo`) to the clipboard.
 
 2. Run the Python script with the following arguments:
```

### Comparing `gog_price_checker-0.1.7/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.8/gog_price_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
@@ -23,15 +21,15 @@
 - Requests library (for making HTTP requests)
 - Regular expressions (re) module
 - Threading module (for concurrent requests)
 - Logging module (for logging)
 
 ## Installation
 ```
-pip instal gog_price_checker
+pip install gog-price-checker
 ```
 
 ## How to Use
 
 1. Copy a URL containing a game page (e.g., `https://www.gog.com/game/diablo`) to the clipboard.
 
 2. Run the Python script with the following arguments:
@@ -83,9 +81,7 @@
 ## License
 
 - The **Game Price Checker** Python script is released under the [MIT License](LICENSE). Feel free to modify and distribute the script according to the terms of the license.
 
 ## Disclaimer
 
 - The author of this script is not responsible for any misuse or consequences of using the script on unauthorized websites. Always make sure you have the right to access and use the data from the websites you interact with.
-
-
```

### Comparing `gog_price_checker-0.1.7/setup.py` & `gog_price_checker-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.7",
+    version="0.1.8",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
```

