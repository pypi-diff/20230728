# Comparing `tmp/modgen-0.1.tar.gz` & `tmp/modgen-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgen-0.1.tar", last modified: Fri Jul 28 12:43:33 2023, max compression
+gzip compressed data, was "modgen-0.2.tar", last modified: Fri Jul 28 12:55:20 2023, max compression
```

## Comparing `modgen-0.1.tar` & `modgen-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:43:33.513652 modgen-0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-28 11:24:33.000000 modgen-0.1/LICENSE
--rw-rw-rw-   0        0        0      287 2023-07-28 12:43:33.513652 modgen-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-07-28 11:26:00.000000 modgen-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 12:43:33.489357 modgen-0.1/modgen/
--rw-rw-rw-   0        0        0       26 2023-07-28 12:43:17.000000 modgen-0.1/modgen/__init__.py
--rw-rw-rw-   0        0        0      357 2023-07-28 12:43:07.000000 modgen-0.1/modgen/modgen.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:43:33.512654 modgen-0.1/modgen.egg-info/
--rw-rw-rw-   0        0        0      287 2023-07-28 12:43:32.000000 modgen-0.1/modgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-28 12:43:33.000000 modgen-0.1/modgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:43:33.000000 modgen-0.1/modgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 12:43:33.000000 modgen-0.1/modgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 12:43:33.514646 modgen-0.1/setup.cfg
--rw-rw-rw-   0        0        0      306 2023-07-28 12:40:08.000000 modgen-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:55:20.953183 modgen-0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-28 11:24:33.000000 modgen-0.2/LICENSE
+-rw-rw-rw-   0        0        0      274 2023-07-28 12:55:20.953183 modgen-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-07-28 12:50:15.000000 modgen-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:55:20.935189 modgen-0.2/modgen/
+-rw-rw-rw-   0        0        0       26 2023-07-28 12:43:17.000000 modgen-0.2/modgen/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-07-28 12:43:07.000000 modgen-0.2/modgen/modgen.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:55:20.951187 modgen-0.2/modgen.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 12:55:20.000000 modgen-0.2/modgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:55:20.953183 modgen-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-07-28 12:54:36.000000 modgen-0.2/setup.py
```

### Comparing `modgen-0.1/LICENSE` & `modgen-0.2/LICENSE`

 * *Files identical despite different names*

