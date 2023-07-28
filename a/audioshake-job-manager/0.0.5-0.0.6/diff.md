# Comparing `tmp/audioshake_job_manager-0.0.5.tar.gz` & `tmp/audioshake_job_manager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioshake_job_manager-0.0.5.tar", last modified: Fri Jul 28 15:03:50 2023, max compression
+gzip compressed data, was "audioshake_job_manager-0.0.6.tar", last modified: Fri Jul 28 21:39:36 2023, max compression
```

## Comparing `audioshake_job_manager-0.0.5.tar` & `audioshake_job_manager-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 15:03:50.718555 audioshake_job_manager-0.0.5/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-28 15:03:50.718163 audioshake_job_manager-0.0.5/PKG-INFO
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 15:03:50.716057 audioshake_job_manager-0.0.5/audioshake_job_manager/
--rw-r--r--   0 theslyguy   (501) staff       (20)     3783 2023-07-28 15:01:47.000000 audioshake_job_manager-0.0.5/audioshake_job_manager/__init__.py
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 15:03:50.717666 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/PKG-INFO
--rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/SOURCES.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/dependency_links.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/requires.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/top_level.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-28 15:03:31.000000 audioshake_job_manager-0.0.5/pyproject.toml
--rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-28 15:03:50.718662 audioshake_job_manager-0.0.5/setup.cfg
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 21:39:36.802188 audioshake_job_manager-0.0.6/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-28 21:39:36.801806 audioshake_job_manager-0.0.6/PKG-INFO
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 21:39:36.799310 audioshake_job_manager-0.0.6/audioshake_job_manager/
+-rw-r--r--   0 theslyguy   (501) staff       (20)     3783 2023-07-28 15:05:42.000000 audioshake_job_manager-0.0.6/audioshake_job_manager/__init__.py
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 21:39:36.801319 audioshake_job_manager-0.0.6/audioshake_job_manager.egg-info/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-28 21:39:36.000000 audioshake_job_manager-0.0.6/audioshake_job_manager.egg-info/PKG-INFO
+-rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-28 21:39:36.000000 audioshake_job_manager-0.0.6/audioshake_job_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-28 21:39:36.000000 audioshake_job_manager-0.0.6/audioshake_job_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-28 21:39:36.000000 audioshake_job_manager-0.0.6/audioshake_job_manager.egg-info/requires.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-28 21:39:36.000000 audioshake_job_manager-0.0.6/audioshake_job_manager.egg-info/top_level.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-28 21:39:23.000000 audioshake_job_manager-0.0.6/pyproject.toml
+-rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-28 21:39:36.802291 audioshake_job_manager-0.0.6/setup.cfg
```

### Comparing `audioshake_job_manager-0.0.5/audioshake_job_manager/__init__.py` & `audioshake_job_manager-0.0.6/audioshake_job_manager/__init__.py`

 * *Files identical despite different names*

