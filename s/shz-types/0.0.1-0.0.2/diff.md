# Comparing `tmp/shz_types-0.0.1.tar.gz` & `tmp/shz_types-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shz_types-0.0.1.tar", last modified: Thu Jul 27 14:50:26 2023, max compression
+gzip compressed data, was "shz_types-0.0.2.tar", last modified: Fri Jul 28 02:16:38 2023, max compression
```

## Comparing `shz_types-0.0.1.tar` & `shz_types-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 14:50:26.138417 shz_types-0.0.1/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-25 13:56:48.000000 shz_types-0.0.1/LICENSE
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      275 2023-07-27 14:50:26.138190 shz_types-0.0.1/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-25 13:57:15.000000 shz_types-0.0.1/README.md
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-27 14:50:26.138484 shz_types-0.0.1/setup.cfg
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      525 2023-07-27 14:48:09.000000 shz_types-0.0.1/setup.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 14:50:26.135487 shz_types-0.0.1/shz_types/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 14:18:08.000000 shz_types-0.0.1/shz_types/__init__.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 14:50:26.137720 shz_types-0.0.1/shz_types.egg-info/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      275 2023-07-27 14:50:26.000000 shz_types-0.0.1/shz_types.egg-info/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      212 2023-07-27 14:50:26.000000 shz_types-0.0.1/shz_types.egg-info/SOURCES.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-27 14:50:26.000000 shz_types-0.0.1/shz_types.egg-info/dependency_links.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       28 2023-07-27 14:50:26.000000 shz_types-0.0.1/shz_types.egg-info/requires.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       10 2023-07-27 14:50:26.000000 shz_types-0.0.1/shz_types.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.690714 shz_types-0.0.2/
+-rw-rw-rw-   0        0        0     1078 2023-07-25 13:56:48.000000 shz_types-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      285 2023-07-28 02:16:38.690714 shz_types-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:57:15.000000 shz_types-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:16:38.691804 shz_types-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      564 2023-07-28 02:16:29.000000 shz_types-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.672319 shz_types-0.0.2/shz_types/
+-rw-rw-rw-   0        0        0        0 2023-07-27 14:18:08.000000 shz_types-0.0.2/shz_types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.690714 shz_types-0.0.2/shz_types/datasets/
+-rw-rw-rw-   0        0        0       25 2023-07-27 14:43:20.000000 shz_types-0.0.2/shz_types/datasets/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-07-27 14:39:45.000000 shz_types-0.0.2/shz_types/datasets/anyDataset.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.689703 shz_types-0.0.2/shz_types.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/top_level.txt
```

### Comparing `shz_types-0.0.1/LICENSE` & `shz_types-0.0.2/LICENSE`

 * *Files identical despite different names*

