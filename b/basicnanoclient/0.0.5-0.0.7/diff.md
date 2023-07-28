# Comparing `tmp/basicnanoclient-0.0.5.tar.gz` & `tmp/basicnanoclient-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicnanoclient-0.0.5.tar", last modified: Tue Apr 18 04:09:57 2023, max compression
+gzip compressed data, was "basicnanoclient-0.0.7.tar", last modified: Fri Jul 28 03:13:05 2023, max compression
```

## Comparing `basicnanoclient-0.0.5.tar` & `basicnanoclient-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 04:09:57.226399 basicnanoclient-0.0.5/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 02:36:25.000000 basicnanoclient-0.0.5/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 04:09:57.226282 basicnanoclient-0.0.5/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      844 2023-04-18 03:14:16.000000 basicnanoclient-0.0.5/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 04:09:57.226149 basicnanoclient-0.0.5/basicnanoclient.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       60 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      675 2023-04-18 04:06:33.000000 basicnanoclient-0.0.5/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 04:09:57.226429 basicnanoclient-0.0.5/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      943 2023-04-18 04:06:28.000000 basicnanoclient-0.0.5/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-28 03:13:05.811622 basicnanoclient-0.0.7/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-07-28 01:29:38.000000 basicnanoclient-0.0.7/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-07-28 03:13:05.811501 basicnanoclient-0.0.7/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      844 2023-07-28 01:29:38.000000 basicnanoclient-0.0.7/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-28 03:13:05.810666 basicnanoclient-0.0.7/basicnanoclient/
+-rw-r--r--   0 nate       (501) staff       (20)      104 2023-07-28 03:09:02.000000 basicnanoclient-0.0.7/basicnanoclient/__init__.py
+-rw-r--r--   0 nate       (501) staff       (20)    10922 2023-07-28 02:23:13.000000 basicnanoclient-0.0.7/basicnanoclient/nano.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-28 03:13:05.811244 basicnanoclient-0.0.7/basicnanoclient.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      287 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       60 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)       16 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      738 2023-07-28 03:12:47.000000 basicnanoclient-0.0.7/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-28 03:13:05.811654 basicnanoclient-0.0.7/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     1034 2023-07-28 03:08:55.000000 basicnanoclient-0.0.7/setup.py
```

### Comparing `basicnanoclient-0.0.5/LICENSE` & `basicnanoclient-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.5/PKG-INFO` & `basicnanoclient-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.5
+Version: 0.0.7
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `basicnanoclient-0.0.5/README.md` & `basicnanoclient-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.5/basicnanoclient.egg-info/PKG-INFO` & `basicnanoclient-0.0.7/basicnanoclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.5
+Version: 0.0.7
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `basicnanoclient-0.0.5/pyproject.toml` & `basicnanoclient-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.coverage.paths]
 source = ["basicnanoclient", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
+[build-system]
+requires = ["setuptools", "wheel", "requests"]
+
 [project]
 name = "basicnanoclient"
-version = "0.0.5"
+version = "0.0.7"
 description = "Nano RPC python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/basicnanoclient/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `basicnanoclient-0.0.5/setup.py` & `basicnanoclient-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Setup."""
 from setuptools import find_packages, setup
+from basicnanoclient import __version__
 
 
 def load_long_description(filename: str) -> str:
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="basicnanoclient",
-    version="0.0.5",
+    version=__version__,
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="Nano Cryptocurrency RPC Client",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/basicnanoclient",
     project_urls={
         "Bug Tracker": "https://github.com/nanoswap/basicnanoclient/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: The Unlicense (Unlicense)"
     ],
     package_dir={'basicnanoclient': "basicnanoclient"},
-    packages=find_packages("basicnanoclient"),
-    python_requires=">=3.11"
+    packages=find_packages(exclude=['tests', 'tests.*']),
+    python_requires=">=3.11",
+    install_requires=["requests"],
 )
```

