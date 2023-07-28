# Comparing `tmp/modgen-0.2.tar.gz` & `tmp/modgen-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgen-0.2.tar", last modified: Fri Jul 28 12:55:20 2023, max compression
+gzip compressed data, was "modgen-0.3.tar", last modified: Fri Jul 28 14:15:47 2023, max compression
```

## Comparing `modgen-0.2.tar` & `modgen-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:55:20.953183 modgen-0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-28 11:24:33.000000 modgen-0.2/LICENSE
--rw-rw-rw-   0        0        0      274 2023-07-28 12:55:20.953183 modgen-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-07-28 12:50:15.000000 modgen-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 12:55:20.935189 modgen-0.2/modgen/
--rw-rw-rw-   0        0        0       26 2023-07-28 12:43:17.000000 modgen-0.2/modgen/__init__.py
--rw-rw-rw-   0        0        0      357 2023-07-28 12:43:07.000000 modgen-0.2/modgen/modgen.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:55:20.951187 modgen-0.2/modgen.egg-info/
--rw-rw-rw-   0        0        0      274 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 12:55:20.953183 modgen-0.2/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-07-28 12:54:36.000000 modgen-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:15:47.164993 modgen-0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-28 11:24:33.000000 modgen-0.3/LICENSE
+-rw-rw-rw-   0        0        0      284 2023-07-28 14:15:47.163994 modgen-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-07-28 12:50:15.000000 modgen-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 14:15:47.149668 modgen-0.3/modgen/
+-rw-rw-rw-   0        0        0       26 2023-07-28 12:43:17.000000 modgen-0.3/modgen/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-07-28 14:13:44.000000 modgen-0.3/modgen/modgen.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:15:47.163994 modgen-0.3/modgen.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-07-28 14:15:46.000000 modgen-0.3/modgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-28 14:15:47.000000 modgen-0.3/modgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:15:46.000000 modgen-0.3/modgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 14:15:46.000000 modgen-0.3/modgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 14:15:47.164993 modgen-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      303 2023-07-28 14:15:37.000000 modgen-0.3/setup.py
```

### Comparing `modgen-0.2/LICENSE` & `modgen-0.3/LICENSE`

 * *Files identical despite different names*

