# Comparing `tmp/gog_price_checker-0.1.4.tar.gz` & `tmp/gog_price_checker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.4.tar", last modified: Fri Jul 28 14:41:34 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.5.tar", last modified: Fri Jul 28 15:24:14 2023, max compression
```

## Comparing `gog_price_checker-0.1.4.tar` & `gog_price_checker-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:41:34.386656 gog_price_checker-0.1.4/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:41:34.386401 gog_price_checker-0.1.4/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)     3119 2023-07-28 13:18:52.000000 gog_price_checker-0.1.4/README.md
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:41:34.385227 gog_price_checker-0.1.4/gog_price_checker/
--rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 14:12:13.000000 gog_price_checker-0.1.4/gog_price_checker/__init__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     3245 2023-07-28 14:38:23.000000 gog_price_checker-0.1.4/gog_price_checker/__main__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 14:07:57.000000 gog_price_checker-0.1.4/gog_price_checker/countries.py
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:41:34.386127 gog_price_checker-0.1.4/gog_price_checker.egg-info/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:41:34.000000 gog_price_checker-0.1.4/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 14:41:34.000000 gog_price_checker-0.1.4/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 14:41:34.000000 gog_price_checker-0.1.4/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 14:41:34.000000 gog_price_checker-0.1.4/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 14:41:34.000000 gog_price_checker-0.1.4/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 14:41:34.386724 gog_price_checker-0.1.4/setup.cfg
--rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 14:40:30.000000 gog_price_checker-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/gog_price_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/gog_price_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/gog_price_checker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/gog_price_checker/countries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/gog_price_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/setup.py
```

### Comparing `gog_price_checker-0.1.4/PKG-INFO` & `gog_price_checker-0.1.5/gog_price_checker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 Metadata-Version: 2.1
-Name: gog_price_checker
-Version: 0.1.4
+Name: gog-price-checker
+Version: 0.1.5
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
+[![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
 
 The **Game Price Checker** is a Python script that allows you to extract a URL from the clipboard, download the web page content, and retrieve the price of a game from the GOG API. The script is designed to work on macOS systems.
 
 ## Requirements
 
 - Python 3.x
 - Requests library (for making HTTP requests)
 - Regular expressions (re) module
 - Threading module (for concurrent requests)
 - Logging module (for logging)
 
+## Installation
+```
+pip instal gog_price_checker
+```
+
 ## How to Use
 
 1. Copy a URL containing a game page (e.g., `https://www.gog.com/game/diablo`) to the clipboard.
 
 2. Run the Python script with the following arguments:
 
     - `-u`, `--url`: The URL of the game page to scrape (required).
     - `-n`, `--normalize`: (Optional) Normalize currencies to USD.
     - `-c`, `--count` : (Optional) default = 10, number of countries to show in sorted prices result
     - `-p`, `--pretty` : (Optional) shows result as pretty table
 
 Example:
 ```
-python app.py -u https://www.gog.com/game/diablo -n -p
->>>...
->>>
+gog_price_checker -u https://www.gog.com/game/diablo -n -p
+```
+Output:
+```
 Country                   Price      Currency
 ---------------------------------------------
 Ukraine                   5.51       USD
 Moldova                   5.51       USD
 Kazakhstan                5.51       USD
 Armenia                   5.51       USD
 China                     5.57       USD
@@ -76,9 +81,7 @@
 ## License
 
 - The **Game Price Checker** Python script is released under the [MIT License](LICENSE). Feel free to modify and distribute the script according to the terms of the license.
 
 ## Disclaimer
 
 - The author of this script is not responsible for any misuse or consequences of using the script on unauthorized websites. Always make sure you have the right to access and use the data from the websites you interact with.
-
-
```

### Comparing `gog_price_checker-0.1.4/README.md` & `gog_price_checker-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 # Game Price Checker 💵
+[![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
 
 The **Game Price Checker** is a Python script that allows you to extract a URL from the clipboard, download the web page content, and retrieve the price of a game from the GOG API. The script is designed to work on macOS systems.
 
 ## Requirements
 
 - Python 3.x
 - Requests library (for making HTTP requests)
 - Regular expressions (re) module
 - Threading module (for concurrent requests)
 - Logging module (for logging)
 
+## Installation
+```
+pip instal gog_price_checker
+```
+
 ## How to Use
 
 1. Copy a URL containing a game page (e.g., `https://www.gog.com/game/diablo`) to the clipboard.
 
 2. Run the Python script with the following arguments:
 
     - `-u`, `--url`: The URL of the game page to scrape (required).
     - `-n`, `--normalize`: (Optional) Normalize currencies to USD.
     - `-c`, `--count` : (Optional) default = 10, number of countries to show in sorted prices result
     - `-p`, `--pretty` : (Optional) shows result as pretty table
 
 Example:
 ```
-python app.py -u https://www.gog.com/game/diablo -n -p
->>>...
->>>
+gog_price_checker -u https://www.gog.com/game/diablo -n -p
+```
+Output:
+```
 Country                   Price      Currency
 ---------------------------------------------
 Ukraine                   5.51       USD
 Moldova                   5.51       USD
 Kazakhstan                5.51       USD
 Armenia                   5.51       USD
 China                     5.57       USD
```

### Comparing `gog_price_checker-0.1.4/gog_price_checker/__main__.py` & `gog_price_checker-0.1.5/gog_price_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.4/gog_price_checker/countries.py` & `gog_price_checker-0.1.5/gog_price_checker/countries.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.4/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 Metadata-Version: 2.1
-Name: gog-price-checker
-Version: 0.1.4
+Name: gog_price_checker
+Version: 0.1.5
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
+[![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
 
 The **Game Price Checker** is a Python script that allows you to extract a URL from the clipboard, download the web page content, and retrieve the price of a game from the GOG API. The script is designed to work on macOS systems.
 
 ## Requirements
 
 - Python 3.x
 - Requests library (for making HTTP requests)
 - Regular expressions (re) module
 - Threading module (for concurrent requests)
 - Logging module (for logging)
 
+## Installation
+```
+pip instal gog_price_checker
+```
+
 ## How to Use
 
 1. Copy a URL containing a game page (e.g., `https://www.gog.com/game/diablo`) to the clipboard.
 
 2. Run the Python script with the following arguments:
 
     - `-u`, `--url`: The URL of the game page to scrape (required).
     - `-n`, `--normalize`: (Optional) Normalize currencies to USD.
     - `-c`, `--count` : (Optional) default = 10, number of countries to show in sorted prices result
     - `-p`, `--pretty` : (Optional) shows result as pretty table
 
 Example:
 ```
-python app.py -u https://www.gog.com/game/diablo -n -p
->>>...
->>>
+gog_price_checker -u https://www.gog.com/game/diablo -n -p
+```
+Output:
+```
 Country                   Price      Currency
 ---------------------------------------------
 Ukraine                   5.51       USD
 Moldova                   5.51       USD
 Kazakhstan                5.51       USD
 Armenia                   5.51       USD
 China                     5.57       USD
@@ -76,9 +81,7 @@
 ## License
 
 - The **Game Price Checker** Python script is released under the [MIT License](LICENSE). Feel free to modify and distribute the script according to the terms of the license.
 
 ## Disclaimer
 
 - The author of this script is not responsible for any misuse or consequences of using the script on unauthorized websites. Always make sure you have the right to access and use the data from the websites you interact with.
-
-
```

### Comparing `gog_price_checker-0.1.4/setup.py` & `gog_price_checker-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.4",
+    version="0.1.5",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
```

