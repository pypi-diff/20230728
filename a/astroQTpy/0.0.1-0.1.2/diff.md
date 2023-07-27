# Comparing `tmp/astroQTpy-0.0.1.tar.gz` & `tmp/astroQTpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroQTpy-0.0.1.tar", last modified: Wed Jul 26 21:58:58 2023, max compression
+gzip compressed data, was "astroQTpy-0.1.2.tar", last modified: Thu Jul 27 23:23:40 2023, max compression
```

## Comparing `astroQTpy-0.0.1.tar` & `astroQTpy-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-26 21:58:58.748423 astroQTpy-0.0.1/
--rw-r--r--   0 calebharada   (501) staff       (20)     1069 2023-07-15 16:01:20.000000 astroQTpy-0.0.1/LICENSE
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-26 21:58:58.748154 astroQTpy-0.0.1/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      172 2023-07-21 21:51:14.000000 astroQTpy-0.0.1/README.md
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-26 21:58:58.742520 astroQTpy-0.0.1/astroQTpy.egg-info/
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-26 21:58:58.000000 astroQTpy-0.0.1/astroQTpy.egg-info/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      381 2023-07-26 21:58:58.000000 astroQTpy-0.0.1/astroQTpy.egg-info/SOURCES.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-26 21:58:58.000000 astroQTpy-0.0.1/astroQTpy.egg-info/dependency_links.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       25 2023-07-26 21:58:58.000000 astroQTpy-0.0.1/astroQTpy.egg-info/requires.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       16 2023-07-26 21:58:58.000000 astroQTpy-0.0.1/astroQTpy.egg-info/top_level.txt
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-26 21:58:58.745818 astroQTpy-0.0.1/astroqtpy/
--rw-r--r--   0 calebharada   (501) staff       (20)      222 2023-07-26 21:36:53.000000 astroQTpy-0.0.1/astroqtpy/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)    16457 2023-07-25 22:58:47.000000 astroQTpy-0.0.1/astroqtpy/basetree.py
--rw-r--r--   0 calebharada   (501) staff       (20)     8904 2023-07-25 17:29:51.000000 astroQTpy-0.0.1/astroqtpy/quadnode.py
--rw-r--r--   0 calebharada   (501) staff       (20)      831 2023-07-24 21:49:59.000000 astroQTpy-0.0.1/astroqtpy/quadpoint.py
--rw-r--r--   0 calebharada   (501) staff       (20)    14141 2023-07-26 02:02:46.000000 astroQTpy-0.0.1/astroqtpy/quadtree.py
--rw-r--r--   0 calebharada   (501) staff       (20)       79 2023-07-20 23:04:56.000000 astroQTpy-0.0.1/pyproject.toml
--rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-26 21:58:58.748494 astroQTpy-0.0.1/setup.cfg
--rw-r--r--   0 calebharada   (501) staff       (20)      876 2023-07-26 21:58:15.000000 astroQTpy-0.0.1/setup.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-26 21:58:58.747451 astroQTpy-0.0.1/tests/
--rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-20 22:59:55.000000 astroQTpy-0.0.1/tests/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1383 2023-07-25 17:31:37.000000 astroQTpy-0.0.1/tests/test_quadnode.py
--rw-r--r--   0 calebharada   (501) staff       (20)      721 2023-07-20 01:38:47.000000 astroQTpy-0.0.1/tests/test_quadpoint.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-27 23:23:40.099168 astroQTpy-0.1.2/
+-rw-r--r--   0 calebharada   (501) staff       (20)     1069 2023-07-15 16:01:20.000000 astroQTpy-0.1.2/LICENSE
+-rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-27 23:23:40.098912 astroQTpy-0.1.2/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      484 2023-07-27 22:43:58.000000 astroQTpy-0.1.2/README.md
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-27 23:23:40.094617 astroQTpy-0.1.2/astroQTpy.egg-info/
+-rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-27 23:23:40.000000 astroQTpy-0.1.2/astroQTpy.egg-info/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      381 2023-07-27 23:23:40.000000 astroQTpy-0.1.2/astroQTpy.egg-info/SOURCES.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-27 23:23:40.000000 astroQTpy-0.1.2/astroQTpy.egg-info/dependency_links.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       39 2023-07-27 23:23:40.000000 astroQTpy-0.1.2/astroQTpy.egg-info/requires.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       16 2023-07-27 23:23:40.000000 astroQTpy-0.1.2/astroQTpy.egg-info/top_level.txt
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-27 23:23:40.097048 astroQTpy-0.1.2/astroqtpy/
+-rw-r--r--   0 calebharada   (501) staff       (20)      186 2023-07-27 23:20:54.000000 astroQTpy-0.1.2/astroqtpy/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    16457 2023-07-26 22:04:11.000000 astroQTpy-0.1.2/astroqtpy/basetree.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     8904 2023-07-26 22:04:11.000000 astroQTpy-0.1.2/astroqtpy/quadnode.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      831 2023-07-26 22:04:11.000000 astroQTpy-0.1.2/astroqtpy/quadpoint.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    14141 2023-07-26 22:04:11.000000 astroQTpy-0.1.2/astroqtpy/quadtree.py
+-rw-r--r--   0 calebharada   (501) staff       (20)       79 2023-07-26 22:04:11.000000 astroQTpy-0.1.2/pyproject.toml
+-rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-27 23:23:40.099239 astroQTpy-0.1.2/setup.cfg
+-rw-r--r--   0 calebharada   (501) staff       (20)      876 2023-07-26 23:07:18.000000 astroQTpy-0.1.2/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-27 23:23:40.098264 astroQTpy-0.1.2/tests/
+-rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-20 22:59:55.000000 astroQTpy-0.1.2/tests/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1383 2023-07-26 22:04:11.000000 astroQTpy-0.1.2/tests/test_quadnode.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      721 2023-07-20 01:38:47.000000 astroQTpy-0.1.2/tests/test_quadpoint.py
```

### Comparing `astroQTpy-0.0.1/LICENSE` & `astroQTpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.0.1/astroqtpy/basetree.py` & `astroQTpy-0.1.2/astroqtpy/basetree.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.0.1/astroqtpy/quadnode.py` & `astroQTpy-0.1.2/astroqtpy/quadnode.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.0.1/astroqtpy/quadpoint.py` & `astroQTpy-0.1.2/astroqtpy/quadpoint.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.0.1/astroqtpy/quadtree.py` & `astroQTpy-0.1.2/astroqtpy/quadtree.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.0.1/setup.py` & `astroQTpy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="astroQTpy",
-    version=get_property("__version__", "astroQTpy"),
+    version=get_property("__version__", "astroqtpy"),
     description="astroQTpy implements a quadtree data structure to explore 2D parameter space",
     url="https://github.com/CalebHarada/astroQTpy",
     author="Caleb K. Harada",
     author_email="charad@berkeley.edu",
     license="MIT",
     packages=find_packages(),
     keywords="Quadtree Astronomy",
```

### Comparing `astroQTpy-0.0.1/tests/test_quadnode.py` & `astroQTpy-0.1.2/tests/test_quadnode.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.0.1/tests/test_quadpoint.py` & `astroQTpy-0.1.2/tests/test_quadpoint.py`

 * *Files identical despite different names*

