# Comparing `tmp/amazon_scrape-1.0.1.tar.gz` & `tmp/amazon_scrape-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-1.0.1.tar", last modified: Fri Jul 28 06:23:05 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-1.0.2.tar", last modified: Fri Jul 28 06:33:10 2023, max compression
```

## Comparing `amazon_scrape-1.0.1.tar` & `amazon_scrape-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:23:05.084725 amazon_scrape-1.0.1/
--rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:23:05.085188 amazon_scrape-1.0.1/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2204 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:23:05.081539 amazon_scrape-1.0.1/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:22:13.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:23:05.084068 amazon_scrape-1.0.1/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     6484 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 06:23:05.086370 amazon_scrape-1.0.1/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:33:10.767798 amazon_scrape-1.0.2/
+-rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:33:10.768176 amazon_scrape-1.0.2/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2204 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:33:10.763759 amazon_scrape-1.0.2/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:33:10.766997 amazon_scrape-1.0.2/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     6484 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 06:33:10.769150 amazon_scrape-1.0.2/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/setup.py
```

### Comparing `amazon_scrape-1.0.1/PKG-INFO` & `amazon_scrape-1.0.2/amazon_scrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: amazon_scrape
-Version: 1.0.1
-Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
+Name: amazon-scrape
+Version: 1.0.2
+Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
@@ -13,15 +13,15 @@
 Description: Amazon Products Scraper
         =======================
         
         .. image:: https://badge.fury.io/py/amazon-scrape.svg
             :target: https://badge.fury.io/py/amazon-scrape
             :alt: amazon-scrape Python Package Version
         
-        Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
+        Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
         
         Requirements
         ------------
         
         Python 2.7 and later.
```

### Comparing `amazon_scrape-1.0.1/README.md` & `amazon_scrape-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Amazon Products Scraper
 
 [![PyPI version](https://badge.fury.io/py/amazon-scrape.svg)](https://badge.fury.io/py/amazon-scrape)
 
-Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
+Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 
 ## Requirements
 
 Python 2.7 and later.
 
 ## Setup
```

### Comparing `amazon_scrape-1.0.1/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: amazon-scrape
-Version: 1.0.1
-Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
+Name: amazon_scrape
+Version: 1.0.2
+Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
@@ -13,15 +13,15 @@
 Description: Amazon Products Scraper
         =======================
         
         .. image:: https://badge.fury.io/py/amazon-scrape.svg
             :target: https://badge.fury.io/py/amazon-scrape
             :alt: amazon-scrape Python Package Version
         
-        Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
+        Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
         
         Requirements
         ------------
         
         Python 2.7 and later.
```

### Comparing `amazon_scrape-1.0.1/amazon_scraper/scraper.py` & `amazon_scrape-1.0.2/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_scrape-1.0.1/setup.py` & `amazon_scrape-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
@@ -19,15 +19,15 @@
     macros.append(('PLATFORM_BSD', '1'))
 elif 'linux' in sys.platform:
     macros.append(('_GNU_SOURCE', ''))
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.",
+    description="Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Finbarrs Oketunji",
     author_email="f@finbarrs.eu",
     url="https://finbarrs.eu",
     packages=find_packages(),
     include_package_data=True,
```

