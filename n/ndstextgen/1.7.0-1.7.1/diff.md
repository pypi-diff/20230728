# Comparing `tmp/ndstextgen-1.7.0.tar.gz` & `tmp/ndstextgen-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndstextgen-1.7.0.tar", last modified: Thu Jul 13 10:57:52 2023, max compression
+gzip compressed data, was "ndstextgen-1.7.1.tar", last modified: Fri Jul 28 17:35:25 2023, max compression
```

## Comparing `ndstextgen-1.7.0.tar` & `ndstextgen-1.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/ndstextgen/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/ndstextgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/ndstextgen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/ndstextgen/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/ndstextgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:35:25.876196 ndstextgen-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 17:35:18.000000 ndstextgen-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-28 17:35:25.876196 ndstextgen-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-28 17:35:18.000000 ndstextgen-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:35:25.876196 ndstextgen-1.7.1/ndstextgen/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-28 17:35:18.000000 ndstextgen-1.7.1/ndstextgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 17:35:18.000000 ndstextgen-1.7.1/ndstextgen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-28 17:35:18.000000 ndstextgen-1.7.1/ndstextgen/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:35:25.876196 ndstextgen-1.7.1/ndstextgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-28 17:35:25.000000 ndstextgen-1.7.1/ndstextgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 17:35:25.000000 ndstextgen-1.7.1/ndstextgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:35:25.000000 ndstextgen-1.7.1/ndstextgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 17:35:25.000000 ndstextgen-1.7.1/ndstextgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 17:35:25.000000 ndstextgen-1.7.1/ndstextgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 17:35:25.000000 ndstextgen-1.7.1/ndstextgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:35:25.876196 ndstextgen-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 17:35:18.000000 ndstextgen-1.7.1/setup.py
```

### Comparing `ndstextgen-1.7.0/LICENSE` & `ndstextgen-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ndstextgen-1.7.0/PKG-INFO` & `ndstextgen-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndstextgen
-Version: 1.7.0
+Version: 1.7.1
 Summary: Command line tool to render text from NDS .NFTR fonts.
 Home-page: https://github.com/Illidanz/ndstextgen
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ndstextgen-1.7.0/README.md` & `ndstextgen-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ndstextgen-1.7.0/ndstextgen/__init__.py` & `ndstextgen-1.7.1/ndstextgen/__init__.py`

 * *Files identical despite different names*

### Comparing `ndstextgen-1.7.0/ndstextgen/cli.py` & `ndstextgen-1.7.1/ndstextgen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,9 +98,9 @@
         final.paste(img, (0, 0), img)
     if out != "":
         final.save(out, "PNG")
     return final
 
 
 def main():
-    click.echo("ndstextgen version 1.7.0")
+    click.echo("ndstextgen version 1.7.1")
     gen()
```

### Comparing `ndstextgen-1.7.0/ndstextgen.egg-info/PKG-INFO` & `ndstextgen-1.7.1/ndstextgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndstextgen
-Version: 1.7.0
+Version: 1.7.1
 Summary: Command line tool to render text from NDS .NFTR fonts.
 Home-page: https://github.com/Illidanz/ndstextgen
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ndstextgen-1.7.0/setup.py` & `ndstextgen-1.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ndstextgen",
-    version="1.7.0",
+    version="1.7.1",
     author="Illidan",
     description="Command line tool to render text from NDS .NFTR fonts.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Illidanz/ndstextgen",
     packages=["ndstextgen"],
     classifiers=[
```

