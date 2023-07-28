# Comparing `tmp/ATTools-0.4.tar.gz` & `tmp/ATTools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATTools-0.4.tar", last modified: Fri Jul 28 10:51:55 2023, max compression
+gzip compressed data, was "ATTools-0.4.1.tar", last modified: Fri Jul 28 10:56:20 2023, max compression
```

## Comparing `ATTools-0.4.tar` & `ATTools-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:51:55.739752 ATTools-0.4/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:51:55.736754 ATTools-0.4/ATTools.egg-info/
--rw-rw-rw-   0        0        0      173 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:51:55.000000 ATTools-0.4/ATTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      173 2023-07-28 10:51:55.738754 ATTools-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-28 10:51:55.740752 ATTools-0.4/setup.cfg
--rw-rw-rw-   0        0        0      914 2023-07-28 10:51:42.000000 ATTools-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:56:20.043500 ATTools-0.4.1/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:56:20.010513 ATTools-0.4.1/ATTools/
+-rw-rw-rw-   0        0        0     8446 2023-07-28 10:03:32.000000 ATTools-0.4.1/ATTools/ATTools.py
+-rw-rw-rw-   0        0        0      914 2023-07-28 10:51:42.000000 ATTools-0.4.1/ATTools/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:56:20.040501 ATTools-0.4.1/ATTools.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-07-28 10:56:19.000000 ATTools-0.4.1/ATTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-28 10:56:19.000000 ATTools-0.4.1/ATTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:56:19.000000 ATTools-0.4.1/ATTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-28 10:56:19.000000 ATTools-0.4.1/ATTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 10:56:19.000000 ATTools-0.4.1/ATTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      175 2023-07-28 10:56:20.041502 ATTools-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 10:56:20.044498 ATTools-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-07-28 10:56:09.000000 ATTools-0.4.1/setup.py
```

### Comparing `ATTools-0.4/setup.py` & `ATTools-0.4.1/ATTools/setup.py`

 * *Files identical despite different names*

