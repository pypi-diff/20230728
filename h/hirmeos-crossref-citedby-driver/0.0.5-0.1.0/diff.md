# Comparing `tmp/hirmeos-crossref-citedby-driver-0.0.5.tar.gz` & `tmp/hirmeos-crossref-citedby-driver-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hirmeos-crossref-citedby-driver-0.0.5.tar", last modified: Wed Jul 26 16:39:42 2023, max compression
+gzip compressed data, was "hirmeos-crossref-citedby-driver-0.1.0.tar", last modified: Fri Jul 28 09:52:37 2023, max compression
```

## Comparing `hirmeos-crossref-citedby-driver-0.0.5.tar` & `hirmeos-crossref-citedby-driver-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1077 2023-07-26 16:14:03.000000 hirmeos-crossref-citedby-driver-0.0.5/LICENSE
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1121 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)      691 2023-07-26 16:39:31.000000 hirmeos-crossref-citedby-driver-0.0.5/README.rst
--rw-r--r--   0 rowan     (1000) rowan     (1000)      616 2023-07-26 16:19:37.000000 hirmeos-crossref-citedby-driver-0.0.5/pyproject.toml
--rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/setup.cfg
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/src/
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/src/crossref_citedby_driver/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     3982 2023-07-26 16:25:12.000000 hirmeos-crossref-citedby-driver-0.0.5/src/crossref_citedby_driver/__init__.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)     2898 2023-07-26 16:06:07.000000 hirmeos-crossref-citedby-driver-0.0.5/src/crossref_citedby_driver/doi_date.py
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/src/hirmeos_crossref_citedby_driver.egg-info/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1121 2023-07-26 16:39:42.000000 hirmeos-crossref-citedby-driver-0.0.5/src/hirmeos_crossref_citedby_driver.egg-info/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)      422 2023-07-26 16:39:42.000000 hirmeos-crossref-citedby-driver-0.0.5/src/hirmeos_crossref_citedby_driver.egg-info/SOURCES.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2023-07-26 16:39:42.000000 hirmeos-crossref-citedby-driver-0.0.5/src/hirmeos_crossref_citedby_driver.egg-info/dependency_links.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       63 2023-07-26 16:39:42.000000 hirmeos-crossref-citedby-driver-0.0.5/src/hirmeos_crossref_citedby_driver.egg-info/requires.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       24 2023-07-26 16:39:42.000000 hirmeos-crossref-citedby-driver-0.0.5/src/hirmeos_crossref_citedby_driver.egg-info/top_level.txt
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-26 16:39:42.752943 hirmeos-crossref-citedby-driver-0.0.5/tests/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     4926 2023-06-09 15:33:17.000000 hirmeos-crossref-citedby-driver-0.0.5/tests/tests.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1077 2023-07-26 16:14:03.000000 hirmeos-crossref-citedby-driver-0.1.0/LICENSE
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1444 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1014 2023-07-28 09:51:33.000000 hirmeos-crossref-citedby-driver-0.1.0/README.rst
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      616 2023-07-28 08:04:23.000000 hirmeos-crossref-citedby-driver-0.1.0/pyproject.toml
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/setup.cfg
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.930683 hirmeos-crossref-citedby-driver-0.1.0/src/
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.930683 hirmeos-crossref-citedby-driver-0.1.0/src/crossref_citedby_driver/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     6286 2023-07-28 09:41:19.000000 hirmeos-crossref-citedby-driver-0.1.0/src/crossref_citedby_driver/__init__.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1444 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      382 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       63 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/requires.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       24 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/top_level.txt
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/tests/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     4926 2023-06-09 15:33:17.000000 hirmeos-crossref-citedby-driver-0.1.0/tests/tests.py
```

### Comparing `hirmeos-crossref-citedby-driver-0.0.5/LICENSE` & `hirmeos-crossref-citedby-driver-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hirmeos-crossref-citedby-driver-0.0.5/pyproject.toml` & `hirmeos-crossref-citedby-driver-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hirmeos-crossref-citedby-driver"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Rowan Hatherley", email="rowan.hatherley@ubiquitypress.com" },
 ]
 description = "Functions required by the crossref-citedby-driver"
 readme = "README.rst"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `hirmeos-crossref-citedby-driver-0.0.5/tests/tests.py` & `hirmeos-crossref-citedby-driver-0.1.0/tests/tests.py`

 * *Files identical despite different names*

