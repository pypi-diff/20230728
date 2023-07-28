# Comparing `tmp/ATTools-0.3.tar.gz` & `tmp/ATTools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATTools-0.3.tar", last modified: Fri Jul 28 10:40:18 2023, max compression
+gzip compressed data, was "ATTools-0.4.tar", last modified: Fri Jul 28 10:51:55 2023, max compression
```

## Comparing `ATTools-0.3.tar` & `ATTools-0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:40:18.510405 ATTools-0.3/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:40:18.507407 ATTools-0.3/ATTools.egg-info/
--rw-rw-rw-   0        0        0      173 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      173 2023-07-28 10:40:18.509404 ATTools-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-28 10:40:18.510405 ATTools-0.3/setup.cfg
--rw-rw-rw-   0        0        0      914 2023-07-28 10:40:08.000000 ATTools-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:51:55.739752 ATTools-0.4/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:51:55.736754 ATTools-0.4/ATTools.egg-info/
+-rw-rw-rw-   0        0        0      173 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      173 2023-07-28 10:51:55.738754 ATTools-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 10:51:55.740752 ATTools-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      914 2023-07-28 10:51:42.000000 ATTools-0.4/setup.py
```

### Comparing `ATTools-0.3/setup.py` & `ATTools-0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ATTools',
-    version='0.3',
+    version='0.4',
     author='NEVNORME',
     author_email='dev.nevermore696@gmail.com',
     description='Tools for The Open Network',
     packages=find_packages(),
     install_requires=[
         'asyncio',
         'aiohttp',
```

