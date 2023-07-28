# Comparing `tmp/passwordP-1.1.1.1.tar.gz` & `tmp/passwordP-1.1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordP-1.1.1.1.tar", last modified: Tue Jul 25 11:18:07 2023, max compression
+gzip compressed data, was "passwordP-1.1.7.7.tar", last modified: Fri Jul 28 09:50:12 2023, max compression
```

## Comparing `passwordP-1.1.1.1.tar` & `passwordP-1.1.7.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:18:07.436388 passwordP-1.1.1.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1066 2023-07-14 10:08:16.000000 passwordP-1.1.1.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)      346 2023-07-25 11:18:07.432388 passwordP-1.1.1.1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:18:07.432388 passwordP-1.1.1.1/passwordP/
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 11:17:34.000000 passwordP-1.1.1.1/passwordP/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      721 2023-07-25 11:09:45.000000 passwordP-1.1.1.1/passwordP/passwordPP.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:18:07.432388 passwordP-1.1.1.1/passwordP.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      346 2023-07-25 11:18:07.000000 passwordP-1.1.1.1/passwordP.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      198 2023-07-25 11:18:07.000000 passwordP-1.1.1.1/passwordP.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 11:18:07.000000 passwordP-1.1.1.1/passwordP.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-07-25 11:18:07.000000 passwordP-1.1.1.1/passwordP.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 11:18:07.436388 passwordP-1.1.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      966 2023-07-25 11:17:44.000000 passwordP-1.1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:50:12.596634 passwordP-1.1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 09:50:03.000000 passwordP-1.1.7.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 09:50:12.596634 passwordP-1.1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-28 09:50:03.000000 passwordP-1.1.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:50:12.592634 passwordP-1.1.7.7/passwordP/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:50:03.000000 passwordP-1.1.7.7/passwordP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 09:50:03.000000 passwordP-1.1.7.7/passwordP/passwordPP.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:50:12.592634 passwordP-1.1.7.7/passwordP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 09:50:12.000000 passwordP-1.1.7.7/passwordP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 09:50:12.000000 passwordP-1.1.7.7/passwordP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:50:12.000000 passwordP-1.1.7.7/passwordP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 09:50:12.000000 passwordP-1.1.7.7/passwordP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:50:12.596634 passwordP-1.1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-28 09:50:03.000000 passwordP-1.1.7.7/setup.py
```

### Comparing `passwordP-1.1.1.1/LICENSE.txt` & `passwordP-1.1.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `passwordP-1.1.1.1/setup.py` & `passwordP-1.1.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="passwordP",                     # This is the name of the package
-    version="1.1.1.1",                        # The initial release version
+    version="1.1.7.7",                        # The initial release version
     author="Nipun dogra",                     # Full name of the author
     description="password generator package",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

