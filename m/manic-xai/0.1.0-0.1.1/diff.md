# Comparing `tmp/manic-xai-0.1.0.tar.gz` & `tmp/manic-xai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manic-xai-0.1.0.tar", last modified: Wed Jul 26 16:12:22 2023, max compression
+gzip compressed data, was "manic-xai-0.1.1.tar", last modified: Fri Jul 28 00:13:42 2023, max compression
```

## Comparing `manic-xai-0.1.0.tar` & `manic-xai-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,37 @@
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-26 16:12:22.800165 manic-xai-0.1.0/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-0.1.0/LICENSE
--rw-r--r--   0 craigpirie   (501) staff       (20)      468 2023-07-26 16:12:22.799936 manic-xai-0.1.0/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-26 16:00:50.000000 manic-xai-0.1.0/README.md
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-26 16:12:22.797664 manic-xai-0.1.0/manic/
--rw-r--r--   0 craigpirie   (501) staff       (20)       96 2023-07-26 15:55:43.000000 manic-xai-0.1.0/manic/__init__.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    16309 2023-07-26 15:48:18.000000 manic-xai-0.1.0/manic/manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1847 2023-07-26 15:49:10.000000 manic-xai-0.1.0/manic/test.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-26 16:12:22.799594 manic-xai-0.1.0/manic_xai.egg-info/
--rw-r--r--   0 craigpirie   (501) staff       (20)      468 2023-07-26 16:12:22.000000 manic-xai-0.1.0/manic_xai.egg-info/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)      237 2023-07-26 16:12:22.000000 manic-xai-0.1.0/manic_xai.egg-info/SOURCES.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-07-26 16:12:22.000000 manic-xai-0.1.0/manic_xai.egg-info/dependency_links.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       35 2023-07-26 16:12:22.000000 manic-xai-0.1.0/manic_xai.egg-info/requires.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-07-26 16:12:22.000000 manic-xai-0.1.0/manic_xai.egg-info/top_level.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-07-26 16:12:22.800236 manic-xai-0.1.0/setup.cfg
--rw-r--r--   0 craigpirie   (501) staff       (20)      641 2023-07-26 16:10:42.000000 manic-xai-0.1.0/setup.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.517598 manic-xai-0.1.1/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-0.1.1/LICENSE
+-rw-r--r--   0 craigpirie   (501) staff       (20)      315 2023-07-28 00:13:42.517204 manic-xai-0.1.1/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-0.1.1/README.md
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.509385 manic-xai-0.1.1/manic/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1305 2023-07-27 14:07:07.000000 manic-xai-0.1.1/manic/Baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2774 2023-07-27 23:07:34.000000 manic-xai-0.1.1/manic/Crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4367 2023-07-27 21:11:16.000000 manic-xai-0.1.1/manic/Disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3050 2023-07-27 23:06:27.000000 manic-xai-0.1.1/manic/Evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 10:52:56.000000 manic-xai-0.1.1/manic/Fitness.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5392 2023-07-27 15:42:32.000000 manic-xai-0.1.1/manic/Initialise.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     8602 2023-07-27 23:08:52.000000 manic-xai-0.1.1/manic/Manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1688 2023-07-27 10:14:30.000000 manic-xai-0.1.1/manic/Mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2009 2023-07-27 23:52:30.000000 manic-xai-0.1.1/manic/Selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      379 2023-07-27 13:22:11.000000 manic-xai-0.1.1/manic/Termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5620 2023-07-27 20:53:42.000000 manic-xai-0.1.1/manic/Utility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      400 2023-07-27 23:27:35.000000 manic-xai-0.1.1/manic/__init__.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.514073 manic-xai-0.1.1/manic/__tests__/
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-0.1.1/manic/__tests__/__init__.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     8075 2023-07-26 16:51:28.000000 manic-xai-0.1.1/manic/__tests__/test_attributes.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2021 2023-07-26 16:47:08.000000 manic-xai-0.1.1/manic/__tests__/test_crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3400 2023-07-26 16:45:04.000000 manic-xai-0.1.1/manic/__tests__/test_initialise.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5512 2023-07-26 16:39:06.000000 manic-xai-0.1.1/manic/__tests__/test_initialise_population.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-0.1.1/manic/__tests__/test_manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2309 2023-07-26 16:41:56.000000 manic-xai-0.1.1/manic/__tests__/test_manic_reproducibility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2106 2023-07-26 16:40:49.000000 manic-xai-0.1.1/manic/__tests__/test_mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2645 2023-07-28 00:03:18.000000 manic-xai-0.1.1/manic/__tests__/test_selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4412 2023-07-26 17:01:13.000000 manic-xai-0.1.1/manic/__tests__/test_validity.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1833 2023-07-27 09:50:27.000000 manic-xai-0.1.1/manic/test.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.516597 manic-xai-0.1.1/manic_xai.egg-info/
+-rw-r--r--   0 craigpirie   (501) staff       (20)      315 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)      782 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       35 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/requires.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/top_level.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-07-28 00:13:42.517717 manic-xai-0.1.1/setup.cfg
+-rw-r--r--   0 craigpirie   (501) staff       (20)      492 2023-07-28 00:13:17.000000 manic-xai-0.1.1/setup.py
```

### Comparing `manic-xai-0.1.0/LICENSE` & `manic-xai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.0/manic/test.py` & `manic-xai-0.1.1/manic/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import random
 import numpy as np
 
 from Manic import Manic
 
 # Example binary classification model
 def predict_fn(instance):
     CLASS = rf_classifier.predict([instance])
```

