# Comparing `tmp/autoparaselenium-0.3.0.tar.gz` & `tmp/autoparaselenium-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoparaselenium-0.3.0.tar", last modified: Fri Jul 28 04:25:45 2023, max compression
+gzip compressed data, was "autoparaselenium-0.3.1.tar", last modified: Fri Jul 28 04:54:38 2023, max compression
```

## Comparing `autoparaselenium-0.3.0.tar` & `autoparaselenium-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/autoparaselenium/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browser_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/autoparaselenium/browsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browsers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browsers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/autoparaselenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/tests/test_browsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/tests/test_everything.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/tests/test_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.568804 autoparaselenium-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.564804 autoparaselenium-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.564804 autoparaselenium-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-28 04:54:38.568804 autoparaselenium-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.564804 autoparaselenium-0.3.1/autoparaselenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/browser_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.568804 autoparaselenium-0.3.1/autoparaselenium/browsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/browsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/browsers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/browsers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/autoparaselenium/setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.568804 autoparaselenium-0.3.1/autoparaselenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-28 04:54:38.000000 autoparaselenium-0.3.1/autoparaselenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 04:54:38.000000 autoparaselenium-0.3.1/autoparaselenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:54:38.000000 autoparaselenium-0.3.1/autoparaselenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 04:54:38.000000 autoparaselenium-0.3.1/autoparaselenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 04:54:38.000000 autoparaselenium-0.3.1/autoparaselenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:54:38.568804 autoparaselenium-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:38.568804 autoparaselenium-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/tests/test_browsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/tests/test_everything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 04:54:17.000000 autoparaselenium-0.3.1/tests/test_pool.py
```

### Comparing `autoparaselenium-0.3.0/.github/workflows/pypi-publish.yml` & `autoparaselenium-0.3.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/LICENSE` & `autoparaselenium-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/PKG-INFO` & `autoparaselenium-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoparaselenium
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library to make parallel selenium tests that automatically download and setup webdrivers
 Author-email: Ronak Badhe <ronak.badhe@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autoparaselenium-0.3.0/README.md` & `autoparaselenium-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/autoparaselenium/__init__.py` & `autoparaselenium-0.3.1/autoparaselenium/__init__.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/autoparaselenium/browser_pool.py` & `autoparaselenium-0.3.1/autoparaselenium/browser_pool.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/autoparaselenium/browsers/chrome.py` & `autoparaselenium-0.3.1/autoparaselenium/browsers/chrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     return browser
 
 
 def setup_driver(pwd: Path) -> None:
     chrome_version = __get_chrome_version()
     driver_version = __get_chromedriver_version(pwd)
     if driver_version is None or driver_version < chrome_version:
-        print(driver_version, chrome_version)
         # chromedriver changed its LATEST_RELEASE_{version} api and download link
         # for chrome >= 115
         if chrome_version < 115:
             r = requests.get(
                 "https://chromedriver.storage.googleapis.com"
                 f"/LATEST_RELEASE_{chrome_version}"
             )
```

### Comparing `autoparaselenium-0.3.0/autoparaselenium/browsers/firefox.py` & `autoparaselenium-0.3.1/autoparaselenium/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/autoparaselenium/setup_utils.py` & `autoparaselenium-0.3.1/autoparaselenium/setup_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import sys
 import tarfile
 from pathlib import Path
 from typing import Callable, Dict, List
 from zipfile import ZipFile
 
 import requests
@@ -35,16 +36,17 @@
 
 def setup_driver(platform_install, platform_drivers, pwd: Path) -> None:
     if not Path(pwd / platform_drivers[platform]).exists():
         __download_and_extract(*platform_install[platform], pwd)
 
     # sometimes webdriver is nested in a folder after zip extraction
     if not Path(pwd / platform_drivers[platform]).exists():
-        (pwd / platform_drivers[platform]).hardlink_to(
-            next(pwd.rglob(platform_drivers[platform]))
+        os.link(
+            next(pwd.rglob(platform_drivers[platform])),
+            pwd / platform_drivers[platform]
         )
 
 
 def __download_and_extract(
     url: str, extract: Callable[[str, str], None], pwd: Path
 ) -> None:
     download(url, pwd / "temp")
```

### Comparing `autoparaselenium-0.3.0/autoparaselenium.egg-info/PKG-INFO` & `autoparaselenium-0.3.1/autoparaselenium.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoparaselenium
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library to make parallel selenium tests that automatically download and setup webdrivers
 Author-email: Ronak Badhe <ronak.badhe@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autoparaselenium-0.3.0/autoparaselenium.egg-info/SOURCES.txt` & `autoparaselenium-0.3.1/autoparaselenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/pyproject.toml` & `autoparaselenium-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/tests/test_browsers.py` & `autoparaselenium-0.3.1/tests/test_browsers.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.3.0/tests/test_everything.py` & `autoparaselenium-0.3.1/tests/test_everything.py`

 * *Files identical despite different names*

