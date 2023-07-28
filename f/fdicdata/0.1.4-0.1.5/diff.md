# Comparing `tmp/fdicdata-0.1.4.tar.gz` & `tmp/fdicdata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdicdata-0.1.4.tar", last modified: Fri Jul 28 19:03:42 2023, max compression
+gzip compressed data, was "fdicdata-0.1.5.tar", last modified: Fri Jul 28 19:06:32 2023, max compression
```

## Comparing `fdicdata-0.1.4.tar` & `fdicdata-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 19:03:42.068469 fdicdata-0.1.4/
--rw-rw-rw-   0        0        0     2317 2023-07-28 19:03:42.068469 fdicdata-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2023-07-28 18:59:18.000000 fdicdata-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 19:03:42.039462 fdicdata-0.1.4/fdicdata/
--rw-rw-rw-   0        0        0      522 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/__init__.py
--rw-rw-rw-   0        0        0     1780 2023-07-11 18:32:51.000000 fdicdata-0.1.4/fdicdata/dataTaxonomy.py
--rw-rw-rw-   0        0        0     1128 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getFailures.py
--rw-rw-rw-   0        0        0     1310 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getFinancials.py
--rw-rw-rw-   0        0        0      893 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getHistory.py
--rw-rw-rw-   0        0        0     1380 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getInstitution.py
--rw-rw-rw-   0        0        0      437 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getInstitutionsAll.py
--rw-rw-rw-   0        0        0      611 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getLocation.py
--rw-rw-rw-   0        0        0     1299 2023-07-11 20:55:35.000000 fdicdata-0.1.4/fdicdata/getSummary.py
--rw-rw-rw-   0        0        0      508 2023-07-11 18:31:24.000000 fdicdata-0.1.4/fdicdata/getTaxonomy.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:03:42.066468 fdicdata-0.1.4/fdicdata.egg-info/
--rw-rw-rw-   0        0        0     2317 2023-07-28 19:03:41.000000 fdicdata-0.1.4/fdicdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-07-28 19:03:41.000000 fdicdata-0.1.4/fdicdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 19:03:41.000000 fdicdata-0.1.4/fdicdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-28 19:03:41.000000 fdicdata-0.1.4/fdicdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 19:03:41.000000 fdicdata-0.1.4/fdicdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 19:03:42.069469 fdicdata-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-07-28 18:28:49.000000 fdicdata-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:06:32.384773 fdicdata-0.1.5/
+-rw-rw-rw-   0        0        0     2318 2023-07-28 19:06:32.384773 fdicdata-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2023-07-28 18:59:18.000000 fdicdata-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 19:06:32.364231 fdicdata-0.1.5/fdicdata/
+-rw-rw-rw-   0        0        0      522 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/__init__.py
+-rw-rw-rw-   0        0        0     1780 2023-07-11 18:32:51.000000 fdicdata-0.1.5/fdicdata/dataTaxonomy.py
+-rw-rw-rw-   0        0        0     1128 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getFailures.py
+-rw-rw-rw-   0        0        0     1310 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getFinancials.py
+-rw-rw-rw-   0        0        0      893 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getHistory.py
+-rw-rw-rw-   0        0        0     1380 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getInstitution.py
+-rw-rw-rw-   0        0        0      437 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getInstitutionsAll.py
+-rw-rw-rw-   0        0        0      611 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getLocation.py
+-rw-rw-rw-   0        0        0     1299 2023-07-11 20:55:35.000000 fdicdata-0.1.5/fdicdata/getSummary.py
+-rw-rw-rw-   0        0        0      508 2023-07-11 18:31:24.000000 fdicdata-0.1.5/fdicdata/getTaxonomy.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:06:32.382799 fdicdata-0.1.5/fdicdata.egg-info/
+-rw-rw-rw-   0        0        0     2318 2023-07-28 19:06:32.000000 fdicdata-0.1.5/fdicdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-07-28 19:06:32.000000 fdicdata-0.1.5/fdicdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 19:06:32.000000 fdicdata-0.1.5/fdicdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-28 19:06:32.000000 fdicdata-0.1.5/fdicdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 19:06:32.000000 fdicdata-0.1.5/fdicdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 19:06:32.384773 fdicdata-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-07-28 19:06:20.000000 fdicdata-0.1.5/setup.py
```

### Comparing `fdicdata-0.1.4/PKG-INFO` & `fdicdata-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fdicdata
-Version: 0.1.4
+Version: 0.1.5
 Summary: The fdicdata package provides a set of functions for working with data from the Federal Deposit Insurance Corporation(FDIC), including retrieving financial data for FDIC-insured institutions and accessing the data taxonomy
 Home-page: https://github.com/Visbanking/fdicdataPy
-Author: rian Pillmore, Boray Yildiz, Ugur Dar
+Author: Brian Pillmore, Boray Yildiz, Ugur Dar
 Author-email: brian.pillmore@gmail.com, boray.yldz@gmail.com, ugurdarr@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fdicdata-0.1.4/README.md` & `fdicdata-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/__init__.py` & `fdicdata-0.1.5/fdicdata/__init__.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/dataTaxonomy.py` & `fdicdata-0.1.5/fdicdata/dataTaxonomy.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/getFailures.py` & `fdicdata-0.1.5/fdicdata/getFailures.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/getFinancials.py` & `fdicdata-0.1.5/fdicdata/getFinancials.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/getHistory.py` & `fdicdata-0.1.5/fdicdata/getHistory.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/getInstitution.py` & `fdicdata-0.1.5/fdicdata/getInstitution.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/getLocation.py` & `fdicdata-0.1.5/fdicdata/getLocation.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata/getSummary.py` & `fdicdata-0.1.5/fdicdata/getSummary.py`

 * *Files identical despite different names*

### Comparing `fdicdata-0.1.4/fdicdata.egg-info/PKG-INFO` & `fdicdata-0.1.5/fdicdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fdicdata
-Version: 0.1.4
+Version: 0.1.5
 Summary: The fdicdata package provides a set of functions for working with data from the Federal Deposit Insurance Corporation(FDIC), including retrieving financial data for FDIC-insured institutions and accessing the data taxonomy
 Home-page: https://github.com/Visbanking/fdicdataPy
-Author: rian Pillmore, Boray Yildiz, Ugur Dar
+Author: Brian Pillmore, Boray Yildiz, Ugur Dar
 Author-email: brian.pillmore@gmail.com, boray.yldz@gmail.com, ugurdarr@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fdicdata-0.1.4/setup.py` & `fdicdata-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fdicdata",
-    version="0.1.4",
+    version="0.1.5",
     description="The fdicdata package provides a set of functions for working with data from the Federal Deposit Insurance Corporation(FDIC), including retrieving financial data for FDIC-insured institutions and accessing the data taxonomy",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    author="rian Pillmore, Boray Yildiz, Ugur Dar",
+    author="Brian Pillmore, Boray Yildiz, Ugur Dar",
     author_email="brian.pillmore@gmail.com, boray.yldz@gmail.com, ugurdarr@gmail.com", 
     url="https://github.com/Visbanking/fdicdataPy",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
```

