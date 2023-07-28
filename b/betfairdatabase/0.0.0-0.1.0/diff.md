# Comparing `tmp/betfairdatabase-0.0.0.tar.gz` & `tmp/betfairdatabase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfairdatabase-0.0.0.tar", last modified: Wed Jul 26 18:34:12 2023, max compression
+gzip compressed data, was "betfairdatabase-0.1.0.tar", last modified: Fri Jul 28 18:24:21 2023, max compression
```

## Comparing `betfairdatabase-0.0.0.tar` & `betfairdatabase-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:12.145530 betfairdatabase-0.0.0/
--rw-rw-rw-   0        0        0     1067 2023-07-26 17:11:33.000000 betfairdatabase-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      795 2023-07-26 18:34:12.145530 betfairdatabase-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       96 2023-07-26 17:10:06.000000 betfairdatabase-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:12.136556 betfairdatabase-0.0.0/betfairdatabase/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:12:01.000000 betfairdatabase-0.0.0/betfairdatabase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:12.143536 betfairdatabase-0.0.0/betfairdatabase.egg-info/
--rw-rw-rw-   0        0        0      795 2023-07-26 18:34:12.000000 betfairdatabase-0.0.0/betfairdatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-26 18:34:12.000000 betfairdatabase-0.0.0/betfairdatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:34:12.000000 betfairdatabase-0.0.0/betfairdatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-26 18:34:12.000000 betfairdatabase-0.0.0/betfairdatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      853 2023-07-26 18:32:26.000000 betfairdatabase-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 18:34:12.146528 betfairdatabase-0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.225482 betfairdatabase-0.1.0/
+-rw-rw-rw-   0        0        0     1067 2023-07-26 17:11:33.000000 betfairdatabase-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4687 2023-07-28 18:24:21.225482 betfairdatabase-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3900 2023-07-28 18:17:23.000000 betfairdatabase-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.214837 betfairdatabase-0.1.0/betfairdatabase/
+-rw-rw-rw-   0        0        0       48 2023-07-28 15:32:44.000000 betfairdatabase-0.1.0/betfairdatabase/__init__.py
+-rw-rw-rw-   0        0        0     2369 2023-07-28 16:03:10.000000 betfairdatabase-0.1.0/betfairdatabase/api.py
+-rw-rw-rw-   0        0        0     6714 2023-07-28 15:23:05.000000 betfairdatabase-0.1.0/betfairdatabase/core.py
+-rw-rw-rw-   0        0        0      709 2023-07-27 22:17:23.000000 betfairdatabase-0.1.0/betfairdatabase/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.221492 betfairdatabase-0.1.0/betfairdatabase.egg-info/
+-rw-rw-rw-   0        0        0     4687 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      853 2023-07-28 18:08:09.000000 betfairdatabase-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:24:21.226479 betfairdatabase-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.223486 betfairdatabase-0.1.0/tests/
+-rw-rw-rw-   0        0        0    12295 2023-07-28 17:32:13.000000 betfairdatabase-0.1.0/tests/test_integration.py
```

### Comparing `betfairdatabase-0.0.0/LICENSE` & `betfairdatabase-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `betfairdatabase-0.0.0/pyproject.toml` & `betfairdatabase-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages=["betfairdatabase"]
 
 [project]
 name = "betfairdatabase"
-version = "0.0.0"
+version = "0.1.0"
 authors = [
   { name="Mario Zaja", email="mzaja0@gmail.com" },
 ]
 description = "Turns a collection of historical Betfair data into a queryable SQL database."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
```

