# Comparing `tmp/pkgUdit-1.1.5.5.tar.gz` & `tmp/pkgUdit-1.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgUdit-1.1.5.5.tar", last modified: Fri Jul 28 09:06:14 2023, max compression
+gzip compressed data, was "pkgUdit-1.1.5.6.tar", last modified: Fri Jul 28 09:14:47 2023, max compression
```

## Comparing `pkgUdit-1.1.5.5.tar` & `pkgUdit-1.1.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:06:14.673104 pkgUdit-1.1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:06:14.673104 pkgUdit-1.1.5.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:06:14.669104 pkgUdit-1.1.5.5/pkgUdit/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:05:59.000000 pkgUdit-1.1.5.5/pkgUdit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:06:14.673104 pkgUdit-1.1.5.5/pkgUdit/data/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 09:05:59.000000 pkgUdit-1.1.5.5/pkgUdit/data/names.csv
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 09:05:59.000000 pkgUdit-1.1.5.5/pkgUdit/data/places.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 09:05:59.000000 pkgUdit-1.1.5.5/pkgUdit/pswdGen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 09:05:59.000000 pkgUdit-1.1.5.5/pkgUdit/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:06:14.673104 pkgUdit-1.1.5.5/pkgUdit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:06:14.000000 pkgUdit-1.1.5.5/pkgUdit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:06:14.000000 pkgUdit-1.1.5.5/pkgUdit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:06:14.000000 pkgUdit-1.1.5.5/pkgUdit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:06:14.000000 pkgUdit-1.1.5.5/pkgUdit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 09:06:14.000000 pkgUdit-1.1.5.5/pkgUdit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:06:14.673104 pkgUdit-1.1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 09:05:59.000000 pkgUdit-1.1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:14:47.623295 pkgUdit-1.1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:14:47.623295 pkgUdit-1.1.5.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:14:47.623295 pkgUdit-1.1.5.6/pkgUdit/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:14:26.000000 pkgUdit-1.1.5.6/pkgUdit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:14:47.623295 pkgUdit-1.1.5.6/pkgUdit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 09:14:26.000000 pkgUdit-1.1.5.6/pkgUdit/data/names.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 09:14:26.000000 pkgUdit-1.1.5.6/pkgUdit/data/places.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 09:14:26.000000 pkgUdit-1.1.5.6/pkgUdit/pswdGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 09:14:26.000000 pkgUdit-1.1.5.6/pkgUdit/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:14:47.623295 pkgUdit-1.1.5.6/pkgUdit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:14:47.000000 pkgUdit-1.1.5.6/pkgUdit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:14:47.000000 pkgUdit-1.1.5.6/pkgUdit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:14:47.000000 pkgUdit-1.1.5.6/pkgUdit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:14:47.000000 pkgUdit-1.1.5.6/pkgUdit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 09:14:47.000000 pkgUdit-1.1.5.6/pkgUdit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:14:47.623295 pkgUdit-1.1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 09:14:26.000000 pkgUdit-1.1.5.6/setup.py
```

### Comparing `pkgUdit-1.1.5.5/pkgUdit/pswdGen.py` & `pkgUdit-1.1.5.6/pkgUdit/pswdGen.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 def make_random():
     """
     Generate a random password that is not present in the name or place list.
 
     Returns:
         str: A randomly generated password.
     """
-    pass_length = random.randint(6, 12)
+    pass_length = random.randint(6, 10)
     password = [custom_choice(combined_chars) for _ in range(pass_length)]
     password.insert(0, random.choice(numerals))  # Include one numeric value
     random.shuffle(password)
     pswd = "".join(password)
     return pswd if password_checker(pswd) else make_random()
 
 def password_checker(created_pass):
```

### Comparing `pkgUdit-1.1.5.5/pkgUdit/test.py` & `pkgUdit-1.1.5.6/pkgUdit/test.py`

 * *Files identical despite different names*

### Comparing `pkgUdit-1.1.5.5/setup.py` & `pkgUdit-1.1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="pkgUdit",                     # This is the name of the package
-    version="1.1.5.5",                        # The current release version
+    version="1.1.5.6",                        # The current release version
     author="Udit Sharma",                     # Full name of the author
     description="The is a sample package",
     zip_safe=False,
     package_data={'pkgUdit': ['data/*.csv']},
     include_package_data=True,
     # long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
```

