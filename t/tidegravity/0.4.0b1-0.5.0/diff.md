# Comparing `tmp/tidegravity-0.4.0b1.tar.gz` & `tmp/tidegravity-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tidegravity-0.4.0b1.tar", last modified: Mon Jun  8 03:15:05 2020, max compression
+gzip compressed data, was "tidegravity-0.5.0.tar", last modified: Fri Jul 28 21:31:20 2023, max compression
```

## Comparing `tidegravity-0.4.0b1.tar` & `tidegravity-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2020-06-08 03:15:05.058782 tidegravity-0.4.0b1/
--rw-rw-rw-   0        0        0     1106 2020-06-08 03:07:08.000000 tidegravity-0.4.0b1/LICENSE
--rw-rw-rw-   0        0        0      100 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     5332 2020-06-08 03:15:05.058950 tidegravity-0.4.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     3417 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/README.rst
--rw-rw-rw-   0        0        0       80 2020-06-08 03:15:05.060877 tidegravity-0.4.0b1/setup.cfg
--rw-rw-rw-   0        0        0     1652 2020-06-08 03:05:44.000000 tidegravity-0.4.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2020-06-08 03:15:05.039116 tidegravity-0.4.0b1/tests/
--rw-rw-rw-   0        0        0      751 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/tests/conftest.py
--rw-rw-rw-   0        0        0    49236 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/tests/matlab_synthetic.csv
--rw-rw-rw-   0        0        0     2253 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/tests/test_longman.py
-drwxrwxrwx   0        0        0        0 2020-06-08 03:15:05.044808 tidegravity-0.4.0b1/tidegravity/
--rw-rw-rw-   0        0        0      100 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/tidegravity/__init__.py
--rw-rw-rw-   0        0        0    14913 2020-06-08 03:02:09.000000 tidegravity-0.4.0b1/tidegravity/tidegravity.py
--rw-rw-rw-   0        0        0     6670 2020-06-08 02:07:11.000000 tidegravity-0.4.0b1/tidegravity/trajectory_utils.py
-drwxrwxrwx   0        0        0        0 2020-06-08 03:15:05.057030 tidegravity-0.4.0b1/tidegravity.egg-info/
--rw-rw-rw-   0        0        0     5332 2020-06-08 03:15:04.000000 tidegravity-0.4.0b1/tidegravity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2020-06-08 03:15:04.000000 tidegravity-0.4.0b1/tidegravity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-08 03:15:04.000000 tidegravity-0.4.0b1/tidegravity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2020-06-08 03:15:04.000000 tidegravity-0.4.0b1/tidegravity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2020-06-08 03:15:04.000000 tidegravity-0.4.0b1/tidegravity.egg-info/top_level.txt
+drwxr-xr-x   0 bradyzp    (501) staff       (20)        0 2023-07-28 21:31:20.699701 tidegravity-0.5.0/
+-rw-r--r--   0 bradyzp    (501) staff       (20)     1106 2023-07-28 21:14:59.000000 tidegravity-0.5.0/LICENSE
+-rw-r--r--   0 bradyzp    (501) staff       (20)      100 2023-07-28 20:52:42.000000 tidegravity-0.5.0/MANIFEST.in
+-rw-r--r--   0 bradyzp    (501) staff       (20)     4424 2023-07-28 21:31:20.699851 tidegravity-0.5.0/PKG-INFO
+-rw-r--r--   0 bradyzp    (501) staff       (20)     3417 2023-07-28 20:52:42.000000 tidegravity-0.5.0/README.rst
+-rw-r--r--   0 bradyzp    (501) staff       (20)       73 2023-07-28 21:31:20.700502 tidegravity-0.5.0/setup.cfg
+-rw-r--r--   0 bradyzp    (501) staff       (20)     1643 2023-07-28 21:31:09.000000 tidegravity-0.5.0/setup.py
+drwxr-xr-x   0 bradyzp    (501) staff       (20)        0 2023-07-28 21:31:20.695818 tidegravity-0.5.0/tests/
+-rw-r--r--   0 bradyzp    (501) staff       (20)      751 2023-07-28 20:52:42.000000 tidegravity-0.5.0/tests/conftest.py
+-rw-r--r--   0 bradyzp    (501) staff       (20)    49236 2023-07-28 20:52:42.000000 tidegravity-0.5.0/tests/matlab_synthetic.csv
+-rw-r--r--   0 bradyzp    (501) staff       (20)     2253 2023-07-28 20:52:42.000000 tidegravity-0.5.0/tests/test_longman.py
+drwxr-xr-x   0 bradyzp    (501) staff       (20)        0 2023-07-28 21:31:20.697477 tidegravity-0.5.0/tidegravity/
+-rw-r--r--   0 bradyzp    (501) staff       (20)      100 2023-07-28 20:52:42.000000 tidegravity-0.5.0/tidegravity/__init__.py
+-rw-r--r--   0 bradyzp    (501) staff       (20)    14913 2023-07-28 20:52:42.000000 tidegravity-0.5.0/tidegravity/tidegravity.py
+-rw-r--r--   0 bradyzp    (501) staff       (20)     6670 2023-07-28 20:52:42.000000 tidegravity-0.5.0/tidegravity/trajectory_utils.py
+drwxr-xr-x   0 bradyzp    (501) staff       (20)        0 2023-07-28 21:31:20.699295 tidegravity-0.5.0/tidegravity.egg-info/
+-rw-r--r--   0 bradyzp    (501) staff       (20)     4424 2023-07-28 21:31:20.000000 tidegravity-0.5.0/tidegravity.egg-info/PKG-INFO
+-rw-r--r--   0 bradyzp    (501) staff       (20)      373 2023-07-28 21:31:20.000000 tidegravity-0.5.0/tidegravity.egg-info/SOURCES.txt
+-rw-r--r--   0 bradyzp    (501) staff       (20)        1 2023-07-28 21:31:20.000000 tidegravity-0.5.0/tidegravity.egg-info/dependency_links.txt
+-rw-r--r--   0 bradyzp    (501) staff       (20)       53 2023-07-28 21:31:20.000000 tidegravity-0.5.0/tidegravity.egg-info/requires.txt
+-rw-r--r--   0 bradyzp    (501) staff       (20)       12 2023-07-28 21:31:20.000000 tidegravity-0.5.0/tidegravity.egg-info/top_level.txt
```

### Comparing `tidegravity-0.4.0b1/LICENSE` & `tidegravity-0.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
 Copyright (c) 2017 John Leeman
-Copyright (c) 2018-2020 Zachery Brady
+Copyright (c) 2018-2023 Zachery Brady
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tidegravity-0.4.0b1/README.rst` & `tidegravity-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `tidegravity-0.4.0b1/setup.py` & `tidegravity-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import os
 from setuptools import setup
 
-__version__ = '0.4.0-beta.1'
+__version__ = '0.5.0'
 requirements = [
-    'numpy == 1.18.5',
-    'pandas == 1.0.4'
+    'numpy == 1.25.0',
+    'pandas == 1.5.3'
 ]
 
 
 def join_relpath(file):
     return os.path.join(os.path.dirname(__file__), file)
 
 
@@ -25,15 +25,15 @@
     version=__version__,
     packages=['tidegravity'],
     install_requires=requirements,
     extras_require={
         'MPL': ['matplotlib>=2.2.0']
     },
     tests_require=['pytest'],
-    python_requires='>=3.5.*',
+    python_requires='>=3.5',
     description="Tide gravitational correction based on I.M. Longman's Formulas for "
                 "Computing the Tidal Accelerations Due to the Moon and the Sun",
     author='Zachery P. Brady, John R. Leeman',
     author_email='bradyzp@dynamicgravitysystems.com',
     url='https://github.com/bradyzp/LongmanTide/',
     download_url='https://github.com/bradyzp/LongmanTide',
     classifiers=[
```

### Comparing `tidegravity-0.4.0b1/tests/conftest.py` & `tidegravity-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tidegravity-0.4.0b1/tests/matlab_synthetic.csv` & `tidegravity-0.5.0/tests/matlab_synthetic.csv`

 * *Files identical despite different names*

### Comparing `tidegravity-0.4.0b1/tests/test_longman.py` & `tidegravity-0.5.0/tests/test_longman.py`

 * *Files identical despite different names*

### Comparing `tidegravity-0.4.0b1/tidegravity/tidegravity.py` & `tidegravity-0.5.0/tidegravity/tidegravity.py`

 * *Files identical despite different names*

### Comparing `tidegravity-0.4.0b1/tidegravity/trajectory_utils.py` & `tidegravity-0.5.0/tidegravity/trajectory_utils.py`

 * *Files identical despite different names*

