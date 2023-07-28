# Comparing `tmp/pkgAnant-3.4.5.tar.gz` & `tmp/pkgAnant-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgAnant-3.4.5.tar", last modified: Fri Jul 28 17:48:16 2023, max compression
+gzip compressed data, was "pkgAnant-3.5.5.tar", last modified: Fri Jul 28 17:50:27 2023, max compression
```

## Comparing `pkgAnant-3.4.5.tar` & `pkgAnant-3.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:48:16.024250 pkgAnant-3.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 17:48:00.000000 pkgAnant-3.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 17:48:16.024250 pkgAnant-3.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-28 17:48:00.000000 pkgAnant-3.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:48:16.024250 pkgAnant-3.4.5/pkgAnant/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 17:48:00.000000 pkgAnant-3.4.5/pkgAnant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 17:48:00.000000 pkgAnant-3.4.5/pkgAnant/passwd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:48:16.024250 pkgAnant-3.4.5/pkgAnant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 17:48:15.000000 pkgAnant-3.4.5/pkgAnant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 17:48:15.000000 pkgAnant-3.4.5/pkgAnant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:48:15.000000 pkgAnant-3.4.5/pkgAnant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 17:48:15.000000 pkgAnant-3.4.5/pkgAnant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:48:16.024250 pkgAnant-3.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 17:48:13.000000 pkgAnant-3.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:50:27.489654 pkgAnant-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 17:50:12.000000 pkgAnant-3.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 17:50:27.489654 pkgAnant-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-28 17:50:12.000000 pkgAnant-3.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:50:27.489654 pkgAnant-3.5.5/pkgAnant/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 17:50:12.000000 pkgAnant-3.5.5/pkgAnant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 17:50:12.000000 pkgAnant-3.5.5/pkgAnant/passwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:50:27.489654 pkgAnant-3.5.5/pkgAnant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 17:50:27.000000 pkgAnant-3.5.5/pkgAnant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 17:50:27.000000 pkgAnant-3.5.5/pkgAnant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:50:27.000000 pkgAnant-3.5.5/pkgAnant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 17:50:27.000000 pkgAnant-3.5.5/pkgAnant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:50:27.489654 pkgAnant-3.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 17:50:12.000000 pkgAnant-3.5.5/setup.py
```

### Comparing `pkgAnant-3.4.5/LICENSE.txt` & `pkgAnant-3.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.4.5/README.md` & `pkgAnant-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.4.5/pkgAnant/passwd.py` & `pkgAnant-3.5.5/pkgAnant/passwd.py`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.4.5/setup.py` & `pkgAnant-3.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="pkgAnant",                     # This is the name of the package
-    version="3.4.5",                        # The initial release version
+    version="3.5.5",                        # The initial release version
     author="Anant Chaudhary",                     # Full name of the author
     description="password generator package",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

