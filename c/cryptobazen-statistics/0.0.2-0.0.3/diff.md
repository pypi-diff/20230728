# Comparing `tmp/cryptobazen_statistics-0.0.2.tar.gz` & `tmp/cryptobazen_statistics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptobazen_statistics-0.0.2.tar", last modified: Fri Jul 28 12:56:40 2023, max compression
+gzip compressed data, was "cryptobazen_statistics-0.0.3.tar", last modified: Fri Jul 28 13:31:05 2023, max compression
```

## Comparing `cryptobazen_statistics-0.0.2.tar` & `cryptobazen_statistics-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:40.716318 cryptobazen_statistics-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 12:56:28.000000 cryptobazen_statistics-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 12:56:40.716318 cryptobazen_statistics-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 12:56:28.000000 cryptobazen_statistics-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:40.712317 cryptobazen_statistics-0.0.2/cryptobazen_statistics/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 12:56:28.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-28 12:56:28.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics/statistic_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:40.712317 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 12:56:40.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 12:56:40.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:56:40.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:56:40.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 12:56:40.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 12:56:40.000000 cryptobazen_statistics-0.0.2/cryptobazen_statistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:56:40.716318 cryptobazen_statistics-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 12:56:28.000000 cryptobazen_statistics-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:31:05.179846 cryptobazen_statistics-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 13:30:56.000000 cryptobazen_statistics-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 13:31:05.179846 cryptobazen_statistics-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:30:56.000000 cryptobazen_statistics-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:31:05.179846 cryptobazen_statistics-0.0.3/cryptobazen_statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:30:56.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-28 13:30:56.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics/statistic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:31:05.179846 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 13:31:05.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 13:31:05.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:31:05.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:31:05.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:31:05.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 13:31:05.000000 cryptobazen_statistics-0.0.3/cryptobazen_statistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:31:05.179846 cryptobazen_statistics-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 13:30:56.000000 cryptobazen_statistics-0.0.3/setup.py
```

### Comparing `cryptobazen_statistics-0.0.2/LICENSE` & `cryptobazen_statistics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptobazen_statistics-0.0.2/cryptobazen_statistics/statistic_functions.py` & `cryptobazen_statistics-0.0.3/cryptobazen_statistics/statistic_functions.py`

 * *Files identical despite different names*

### Comparing `cryptobazen_statistics-0.0.2/setup.py` & `cryptobazen_statistics-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cryptobazen_statistics',
-    version='0.0.2',
+    version='0.0.3',
     description='Statistic functions for Transformer models',
     long_description='The PyToch Transformer model needs sometimes a custom statistic function. This package contains some of these functions.',
     author='Cryptobazen',
     author_email='erwinvink@outlook.com',
     packages=["cryptobazen_statistics"],
     license='MIT License',
     install_requires=[
```

