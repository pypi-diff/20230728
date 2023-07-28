# Comparing `tmp/abbyPython-2.0.0.tar.gz` & `tmp/abbyPython-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abbyPython-2.0.0.tar", last modified: Wed Jul  5 12:36:22 2023, max compression
+gzip compressed data, was "abbyPython-2.2.0.tar", last modified: Fri Jul 28 09:45:35 2023, max compression
```

## Comparing `abbyPython-2.0.0.tar` & `abbyPython-2.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2023-07-05 12:36:22.627028 abbyPython-2.0.0/
--rw-r--r--   0 julian    (1000) julian    (1000)      313 2023-07-05 12:36:22.627028 abbyPython-2.0.0/PKG-INFO
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2023-07-05 12:36:22.627028 abbyPython-2.0.0/abbyPython.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)      313 2023-07-05 12:36:22.000000 abbyPython-2.0.0/abbyPython.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      144 2023-07-05 12:36:22.000000 abbyPython-2.0.0/abbyPython.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2023-07-05 12:36:22.000000 abbyPython-2.0.0/abbyPython.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2023-07-05 12:36:22.000000 abbyPython-2.0.0/abbyPython.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2023-07-05 12:36:22.627028 abbyPython-2.0.0/setup.cfg
--rw-r--r--   0 julian    (1000) julian    (1000)      500 2023-07-05 12:35:00.000000 abbyPython-2.0.0/setup.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2023-07-28 09:45:35.629194 abbyPython-2.2.0/
+-rw-r--r--   0 julian    (1000) julian    (1000)      313 2023-07-28 09:45:35.629194 abbyPython-2.2.0/PKG-INFO
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2023-07-28 09:45:35.629194 abbyPython-2.2.0/abbyPython.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)      313 2023-07-28 09:45:35.000000 abbyPython-2.2.0/abbyPython.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      144 2023-07-28 09:45:35.000000 abbyPython-2.2.0/abbyPython.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2023-07-28 09:45:35.000000 abbyPython-2.2.0/abbyPython.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2023-07-28 09:45:35.000000 abbyPython-2.2.0/abbyPython.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2023-07-28 09:45:35.629194 abbyPython-2.2.0/setup.cfg
+-rw-r--r--   0 julian    (1000) julian    (1000)      500 2023-07-28 09:42:34.000000 abbyPython-2.2.0/setup.py
```

