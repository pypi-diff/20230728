# Comparing `tmp/chichicha-2.4.0.tar.gz` & `tmp/chichicha-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chichicha-2.4.0.tar", last modified: Fri Jul 28 01:58:31 2023, max compression
+gzip compressed data, was "chichicha-2.5.0.tar", last modified: Fri Jul 28 02:14:15 2023, max compression
```

## Comparing `chichicha-2.4.0.tar` & `chichicha-2.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 01:58:31.584085 chichicha-2.4.0/
--rw-rw-rw-   0        0        0     1074 2022-08-31 06:39:42.000000 chichicha-2.4.0/LICENSE
--rw-rw-rw-   0        0        0       33 2022-08-31 08:45:36.000000 chichicha-2.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2023-07-28 01:58:31.581805 chichicha-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2022-10-14 02:43:05.000000 chichicha-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 01:58:31.556624 chichicha-2.4.0/chichicha/
--rw-rw-rw-   0        0        0        0 2022-10-06 06:11:11.000000 chichicha-2.4.0/chichicha/__init__.py
--rw-rw-rw-   0        0        0  8180224 2023-07-27 04:39:02.000000 chichicha-2.4.0/chichicha/pywpc.pyd
--rw-rw-rw-   0        0        0       17 2023-07-28 01:53:34.000000 chichicha-2.4.0/chichicha/version.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:58:31.579637 chichicha-2.4.0/chichicha.egg-info/
--rw-rw-rw-   0        0        0      262 2023-07-28 01:58:31.000000 chichicha-2.4.0/chichicha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-28 01:58:31.000000 chichicha-2.4.0/chichicha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 01:58:31.000000 chichicha-2.4.0/chichicha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      145 2023-07-28 01:58:31.000000 chichicha-2.4.0/chichicha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-28 01:58:31.000000 chichicha-2.4.0/chichicha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 01:58:31.584085 chichicha-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-07-28 01:58:26.000000 chichicha-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:14:15.989712 chichicha-2.5.0/
+-rw-rw-rw-   0        0        0     1074 2022-08-31 06:39:42.000000 chichicha-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-08-31 08:45:36.000000 chichicha-2.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2023-07-28 02:14:15.986734 chichicha-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1557 2022-10-14 02:43:05.000000 chichicha-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 02:14:15.957980 chichicha-2.5.0/chichicha/
+-rw-rw-rw-   0        0        0        0 2022-10-06 06:11:11.000000 chichicha-2.5.0/chichicha/__init__.py
+-rw-rw-rw-   0        0        0  8180224 2023-07-27 04:39:02.000000 chichicha-2.5.0/chichicha/pywpc.pyd
+-rw-rw-rw-   0        0        0       17 2023-07-28 02:13:33.000000 chichicha-2.5.0/chichicha/version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:14:15.984695 chichicha-2.5.0/chichicha.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-07-28 02:14:15.000000 chichicha-2.5.0/chichicha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-28 02:14:15.000000 chichicha-2.5.0/chichicha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:14:15.000000 chichicha-2.5.0/chichicha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2023-07-28 02:14:15.000000 chichicha-2.5.0/chichicha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 02:14:15.000000 chichicha-2.5.0/chichicha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:14:15.989712 chichicha-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-07-28 01:58:26.000000 chichicha-2.5.0/setup.py
```

### Comparing `chichicha-2.4.0/LICENSE` & `chichicha-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chichicha-2.4.0/README.md` & `chichicha-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `chichicha-2.4.0/setup.py` & `chichicha-2.5.0/setup.py`

 * *Files identical despite different names*

