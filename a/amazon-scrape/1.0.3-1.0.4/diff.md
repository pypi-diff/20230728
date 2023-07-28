# Comparing `tmp/amazon_scrape-1.0.3.tar.gz` & `tmp/amazon_scrape-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-1.0.3.tar", last modified: Fri Jul 28 09:11:17 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-1.0.4.tar", last modified: Fri Jul 28 09:53:51 2023, max compression
```

## Comparing `amazon_scrape-1.0.3.tar` & `amazon_scrape-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:11:17.614519 amazon_scrape-1.0.3/
--rw-r--r--   0 finn       (501) staff       (20)     5107 2023-07-28 09:11:17.614924 amazon_scrape-1.0.3/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2368 2023-07-28 09:10:39.000000 amazon_scrape-1.0.3/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:11:17.611540 amazon_scrape-1.0.3/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5107 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:11:17.613782 amazon_scrape-1.0.3/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.3/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     8368 2023-07-28 09:06:51.000000 amazon_scrape-1.0.3/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 09:07:22.000000 amazon_scrape-1.0.3/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 09:11:17.616136 amazon_scrape-1.0.3/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 09:07:22.000000 amazon_scrape-1.0.3/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:53:51.189551 amazon_scrape-1.0.4/
+-rw-r--r--   0 finn       (501) staff       (20)     5107 2023-07-28 09:53:51.189883 amazon_scrape-1.0.4/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2368 2023-07-28 09:51:13.000000 amazon_scrape-1.0.4/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:53:51.184992 amazon_scrape-1.0.4/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5107 2023-07-28 09:53:51.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 09:53:51.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 09:53:51.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 09:53:51.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 09:53:51.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 09:53:51.000000 amazon_scrape-1.0.4/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:53:51.188374 amazon_scrape-1.0.4/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.4/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     8368 2023-07-28 09:06:51.000000 amazon_scrape-1.0.4/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 09:51:23.000000 amazon_scrape-1.0.4/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 09:53:51.190710 amazon_scrape-1.0.4/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 09:51:23.000000 amazon_scrape-1.0.4/setup.py
```

### Comparing `amazon_scrape-1.0.3/PKG-INFO` & `amazon_scrape-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 1.0.3
+Version: 1.0.4
 Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -44,15 +44,15 @@
         Scraper Help
         ------------
         
         Execute this command `amazon_scraper --help` in the terminal.
         
         .. code-block:: text
         
-            usage: amazon_scraper [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES]
+            usage: amazon.py [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES] [-r]
         
             optional arguments:
             -h, --help            show this help message and exit
             --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
             --keywords KEYWORDS   Search keywords
             --url URL             Amazon URL
             --proxy_api_key       Scraper API Key
```

### Comparing `amazon_scrape-1.0.3/README.md` & `amazon_scrape-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ## or `sudo python setup.py install` to install the package for all users
 ```
 
 ## Scraper Help
 Execute this command `amazon_scraper --help` in the terminal.
 
 ```text
-usage: amazon_scraper [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES]
+usage: amazon.py [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES] [-r]
 
 optional arguments:
   -h, --help            show this help message and exit
   --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
   --keywords KEYWORDS   Search keywords
   --url URL             Amazon URL
   --proxy_api_key       Scraper API Key
```

### Comparing `amazon_scrape-1.0.3/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-1.0.4/amazon_scrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 1.0.3
+Version: 1.0.4
 Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -44,15 +44,15 @@
         Scraper Help
         ------------
         
         Execute this command `amazon_scraper --help` in the terminal.
         
         .. code-block:: text
         
-            usage: amazon_scraper [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES]
+            usage: amazon.py [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES] [-r]
         
             optional arguments:
             -h, --help            show this help message and exit
             --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
             --keywords KEYWORDS   Search keywords
             --url URL             Amazon URL
             --proxy_api_key       Scraper API Key
```

### Comparing `amazon_scrape-1.0.3/amazon_scraper/scraper.py` & `amazon_scrape-1.0.4/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_scrape-1.0.3/setup.py` & `amazon_scrape-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

