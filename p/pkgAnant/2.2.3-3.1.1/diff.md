# Comparing `tmp/pkgAnant-2.2.3.tar.gz` & `tmp/pkgAnant-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pkgAnant-2.2.3.tar", last modified: Fri Jul 28 08:20:15 2023, max compression
+gzip compressed data, was "dist/pkgAnant-3.1.1.tar", last modified: Fri Jul 28 07:41:12 2023, max compression
```

## Comparing `pkgAnant-2.2.3.tar` & `pkgAnant-3.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 08:20:02.000000 pkgAnant-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/pkgAnant/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 08:20:02.000000 pkgAnant-2.2.3/pkgAnant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 08:20:02.000000 pkgAnant-2.2.3/pkgAnant/passwd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/pkgAnant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/pkgAnant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/pkgAnant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/pkgAnant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/pkgAnant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:20:15.000000 pkgAnant-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 08:20:02.000000 pkgAnant-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:41:12.000000 pkgAnant-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 07:41:12.000000 pkgAnant-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 07:40:56.000000 pkgAnant-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:41:12.000000 pkgAnant-3.1.1/pkgAnant/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 07:40:56.000000 pkgAnant-3.1.1/pkgAnant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-28 07:40:56.000000 pkgAnant-3.1.1/pkgAnant/passwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:41:12.000000 pkgAnant-3.1.1/pkgAnant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 07:41:11.000000 pkgAnant-3.1.1/pkgAnant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-28 07:41:12.000000 pkgAnant-3.1.1/pkgAnant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:41:11.000000 pkgAnant-3.1.1/pkgAnant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 07:41:11.000000 pkgAnant-3.1.1/pkgAnant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 07:41:12.000000 pkgAnant-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 07:41:10.000000 pkgAnant-3.1.1/setup.py
```

### Comparing `pkgAnant-2.2.3/pkgAnant/passwd.py` & `pkgAnant-3.1.1/pkgAnant/passwd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import string
 
-def gen_pass():
+def generate_pass():
 
     # using random for range
-    len=random.randint(5, 10)
+    len=random.randint(6, 10)
 
     # using string to generate characters
     lower=string.ascii_lowercase
     upper=string.ascii_uppercase
     num=string.digits
 
     # to select at least one lower, one upper, one number
```

### Comparing `pkgAnant-2.2.3/setup.py` & `pkgAnant-3.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="pkgAnant",                     # This is the name of the package
-    version="2.2.3",                        # The initial release version
+    version="3.1.1",                        # The initial release version
     author="Anant Chaudhary",                     # Full name of the author
     description="password generator package",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

