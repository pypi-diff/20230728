# Comparing `tmp/rt2-0.0.1.tar.gz` & `tmp/rt2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt2-0.0.1.tar", last modified: Fri Jul 28 15:29:31 2023, max compression
+gzip compressed data, was "rt2-0.0.2.tar", last modified: Fri Jul 28 19:11:18 2023, max compression
```

## Comparing `rt2-0.0.1.tar` & `rt2-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:29:31.233244 rt2-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 15:29:21.000000 rt2-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 15:29:31.233244 rt2-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-28 15:29:21.000000 rt2-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:29:31.233244 rt2-0.0.1/rt2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 15:29:31.000000 rt2-0.0.1/rt2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 15:29:31.000000 rt2-0.0.1/rt2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:29:31.000000 rt2-0.0.1/rt2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 15:29:31.000000 rt2-0.0.1/rt2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:29:31.000000 rt2-0.0.1/rt2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:29:31.233244 rt2-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 15:29:21.000000 rt2-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:18.746004 rt2-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 19:11:06.000000 rt2-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 19:11:18.746004 rt2-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-28 19:11:06.000000 rt2-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:18.746004 rt2-0.0.2/rt2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 19:11:18.000000 rt2-0.0.2/rt2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 19:11:18.000000 rt2-0.0.2/rt2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:11:18.000000 rt2-0.0.2/rt2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 19:11:18.000000 rt2-0.0.2/rt2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:11:18.000000 rt2-0.0.2/rt2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:11:18.746004 rt2-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 19:11:06.000000 rt2-0.0.2/setup.py
```

### Comparing `rt2-0.0.1/LICENSE` & `rt2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rt2-0.0.1/PKG-INFO` & `rt2-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt2
-Version: 0.0.1
+Version: 0.0.2
 Summary: rt-2 - PyTorch
 Home-page: https://github.com/kyegomez/rt-2
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rt2-0.0.1/rt2.egg-info/PKG-INFO` & `rt2-0.0.2/rt2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt2
-Version: 0.0.1
+Version: 0.0.2
 Summary: rt-2 - PyTorch
 Home-page: https://github.com/kyegomez/rt-2
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rt2-0.0.1/setup.py` & `rt2-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rt2',
     packages=find_packages(exclude=[]),
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     description='rt-2 - PyTorch',
     author='Kye Gomez',
     author_email='kye@apac.ai',
     long_description_content_type='text/markdown',
     url='https://github.com/kyegomez/rt-2',
     keywords=[
```

