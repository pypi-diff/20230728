# Comparing `tmp/turboyaml-0.0.1.tar.gz` & `tmp/turboyaml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turboyaml-0.0.1.tar", last modified: Wed Jul 26 04:32:18 2023, max compression
+gzip compressed data, was "turboyaml-0.0.2.tar", last modified: Fri Jul 28 02:54:25 2023, max compression
```

## Comparing `turboyaml-0.0.1.tar` & `turboyaml-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-26 04:32:18.028668 turboyaml-0.0.1/
--rw-r--r--   0 fredbrowne   (501) staff       (20)     1067 2023-07-26 03:34:01.000000 turboyaml-0.0.1/LICENSE
--rw-r--r--   0 fredbrowne   (501) staff       (20)     3038 2023-07-26 04:32:18.028529 turboyaml-0.0.1/PKG-INFO
--rw-r--r--   0 fredbrowne   (501) staff       (20)     2465 2023-07-26 04:27:30.000000 turboyaml-0.0.1/README.md
--rw-r--r--   0 fredbrowne   (501) staff       (20)       38 2023-07-26 04:32:18.028709 turboyaml-0.0.1/setup.cfg
--rw-r--r--   0 fredbrowne   (501) staff       (20)      906 2023-07-26 04:27:31.000000 turboyaml-0.0.1/setup.py
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-26 04:32:18.027555 turboyaml-0.0.1/turboyaml/
--rw-r--r--   0 fredbrowne   (501) staff       (20)        0 2023-07-26 03:30:30.000000 turboyaml-0.0.1/turboyaml/__init__.py
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5393 2023-07-26 04:27:32.000000 turboyaml-0.0.1/turboyaml/cli.py
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-26 04:32:18.028337 turboyaml-0.0.1/turboyaml.egg-info/
--rw-r--r--   0 fredbrowne   (501) staff       (20)     3038 2023-07-26 04:32:18.000000 turboyaml-0.0.1/turboyaml.egg-info/PKG-INFO
--rw-r--r--   0 fredbrowne   (501) staff       (20)      265 2023-07-26 04:32:18.000000 turboyaml-0.0.1/turboyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)        1 2023-07-26 04:32:18.000000 turboyaml-0.0.1/turboyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       50 2023-07-26 04:32:18.000000 turboyaml-0.0.1/turboyaml.egg-info/entry_points.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)        7 2023-07-26 04:32:18.000000 turboyaml-0.0.1/turboyaml.egg-info/requires.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       10 2023-07-26 04:32:18.000000 turboyaml-0.0.1/turboyaml.egg-info/top_level.txt
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 02:54:25.099517 turboyaml-0.0.2/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     1067 2023-07-26 03:34:01.000000 turboyaml-0.0.2/LICENSE
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5689 2023-07-28 02:54:25.099332 turboyaml-0.0.2/PKG-INFO
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5116 2023-07-28 02:27:59.000000 turboyaml-0.0.2/README.md
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       38 2023-07-28 02:54:25.099587 turboyaml-0.0.2/setup.cfg
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      914 2023-07-28 02:09:59.000000 turboyaml-0.0.2/setup.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 02:54:25.098470 turboyaml-0.0.2/turboyaml/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       22 2023-07-28 02:21:13.000000 turboyaml-0.0.2/turboyaml/__init__.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     9193 2023-07-28 02:27:09.000000 turboyaml-0.0.2/turboyaml/cli.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 02:54:25.099159 turboyaml-0.0.2/turboyaml.egg-info/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5689 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      265 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)        1 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       50 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/entry_points.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       15 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/requires.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       10 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/top_level.txt
```

### Comparing `turboyaml-0.0.1/LICENSE` & `turboyaml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `turboyaml-0.0.1/setup.py` & `turboyaml-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="turboyaml",
-    version="0.0.1",
+    version="0.0.2",
     author="Fred Setra",
     author_email="fred.setra@gmail.com",
     description="An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredbrowne/turboyaml",
     packages=find_packages(),
     install_requires=[
-        "openai",
+        "openai==0.27.8",
     ],
     entry_points={
         "console_scripts": [
             "turboyaml=turboyaml.cli:main",
         ],
     },
     classifiers=[
```

