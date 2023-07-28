# Comparing `tmp/describealign-0.1.1.tar.gz` & `tmp/describealign-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describealign-0.1.1.tar", last modified: Thu Jul 27 07:12:11 2023, max compression
+gzip compressed data, was "describealign-0.1.2.tar", last modified: Fri Jul 28 02:57:41 2023, max compression
```

## Comparing `describealign-0.1.1.tar` & `describealign-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 07:12:11.699163 describealign-0.1.1/
--rw-rw-rw-   0        0        0    35149 2023-07-26 20:20:51.000000 describealign-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      807 2023-07-27 07:12:11.699163 describealign-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-26 19:29:21.000000 describealign-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 07:12:11.693163 describealign-0.1.1/describealign/
--rw-rw-rw-   0        0        0        0 2023-07-26 19:20:51.000000 describealign-0.1.1/describealign/__init__.py
--rw-rw-rw-   0        0        0    40156 2023-07-27 07:05:59.000000 describealign-0.1.1/describealign/describealign.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:12:11.698163 describealign-0.1.1/describealign.egg-info/
--rw-rw-rw-   0        0        0      807 2023-07-27 07:12:11.000000 describealign-0.1.1/describealign.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-07-27 07:12:11.000000 describealign-0.1.1/describealign.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 07:12:11.000000 describealign-0.1.1/describealign.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-27 07:12:11.000000 describealign-0.1.1/describealign.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2023-07-27 07:12:11.000000 describealign-0.1.1/describealign.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-27 07:12:11.000000 describealign-0.1.1/describealign.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      964 2023-07-27 06:58:33.000000 describealign-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 07:12:11.700163 describealign-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 02:57:41.915980 describealign-0.1.2/
+-rw-rw-rw-   0        0        0    35149 2023-07-26 20:20:51.000000 describealign-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      807 2023-07-28 02:57:41.914980 describealign-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-26 19:29:21.000000 describealign-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 02:57:41.913980 describealign-0.1.2/describealign.egg-info/
+-rw-rw-rw-   0        0        0      807 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40156 2023-07-27 07:05:59.000000 describealign-0.1.2/describealign.py
+-rw-rw-rw-   0        0        0      950 2023-07-28 02:55:44.000000 describealign-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:57:41.915980 describealign-0.1.2/setup.cfg
```

### Comparing `describealign-0.1.1/LICENSE` & `describealign-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `describealign-0.1.1/PKG-INFO` & `describealign-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describealign
-Version: 0.1.1
+Version: 0.1.2
 Summary: Combines videos with matching audio files (e.g. audio descriptions)
 Author-email: Julian Brown <julbean@proton.me>
 Project-URL: Homepage, https://github.com/julbean/describealign
 Project-URL: Bug Tracker, https://github.com/julbean/describealign/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `describealign-0.1.1/describealign/describealign.py` & `describealign-0.1.2/describealign.py`

 * *Files identical despite different names*

### Comparing `describealign-0.1.1/describealign.egg-info/PKG-INFO` & `describealign-0.1.2/describealign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describealign
-Version: 0.1.1
+Version: 0.1.2
 Summary: Combines videos with matching audio files (e.g. audio descriptions)
 Author-email: Julian Brown <julbean@proton.me>
 Project-URL: Homepage, https://github.com/julbean/describealign
 Project-URL: Bug Tracker, https://github.com/julbean/describealign/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `describealign-0.1.1/pyproject.toml` & `describealign-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "describealign"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Julian Brown", email="julbean@proton.me" },
 ]
 description = "Combines videos with matching audio files (e.g. audio descriptions)"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -22,13 +22,13 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-describealign = "describealign.describealign:command_line_interface"
+describealign = "describealign:command_line_interface"
 
 [project.urls]
 "Homepage" = "https://github.com/julbean/describealign"
 "Bug Tracker" = "https://github.com/julbean/describealign/issues"
```

