# Comparing `tmp/pkgAnant-3.3.3.tar.gz` & `tmp/pkgAnant-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgAnant-3.3.3.tar", last modified: Fri Jul 28 09:26:58 2023, max compression
+gzip compressed data, was "pkgAnant-3.3.4.tar", last modified: Fri Jul 28 11:05:30 2023, max compression
```

## Comparing `pkgAnant-3.3.3.tar` & `pkgAnant-3.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:26:58.335106 pkgAnant-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 09:26:44.000000 pkgAnant-3.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 09:26:58.335106 pkgAnant-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-28 09:26:44.000000 pkgAnant-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:26:58.335106 pkgAnant-3.3.3/pkgAnant/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 09:26:44.000000 pkgAnant-3.3.3/pkgAnant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 09:26:44.000000 pkgAnant-3.3.3/pkgAnant/passwd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:26:58.335106 pkgAnant-3.3.3/pkgAnant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 09:26:58.000000 pkgAnant-3.3.3/pkgAnant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 09:26:58.000000 pkgAnant-3.3.3/pkgAnant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:26:58.000000 pkgAnant-3.3.3/pkgAnant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 09:26:58.000000 pkgAnant-3.3.3/pkgAnant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:26:58.335106 pkgAnant-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 09:26:44.000000 pkgAnant-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:05:30.113588 pkgAnant-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 11:05:22.000000 pkgAnant-3.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 11:05:30.113588 pkgAnant-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-28 11:05:22.000000 pkgAnant-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:05:30.113588 pkgAnant-3.3.4/pkgAnant/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 11:05:22.000000 pkgAnant-3.3.4/pkgAnant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 11:05:22.000000 pkgAnant-3.3.4/pkgAnant/passwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:05:30.113588 pkgAnant-3.3.4/pkgAnant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 11:05:29.000000 pkgAnant-3.3.4/pkgAnant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 11:05:30.000000 pkgAnant-3.3.4/pkgAnant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:05:29.000000 pkgAnant-3.3.4/pkgAnant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 11:05:29.000000 pkgAnant-3.3.4/pkgAnant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:05:30.113588 pkgAnant-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-28 11:05:22.000000 pkgAnant-3.3.4/setup.py
```

### Comparing `pkgAnant-3.3.3/LICENSE.txt` & `pkgAnant-3.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.3.3/README.md` & `pkgAnant-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.3.3/pkgAnant/passwd.py` & `pkgAnant-3.3.4/pkgAnant/passwd.py`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.3.3/setup.py` & `pkgAnant-3.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import setuptools
+VERSION = "3.3.4" 
 
 setuptools.setup(
     name="pkgAnant",                     # This is the name of the package
-    version="3.3.3",                        # The initial release version
+    version=VERSION,                        # The initial release version
     author="Anant Chaudhary",                     # Full name of the author
     description="password generator package",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

