# Comparing `tmp/idev-pystatistics-1.0.0.tar.gz` & `tmp/idev-pystatistics-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idev-pystatistics-1.0.0.tar", last modified: Fri Jul 28 20:29:35 2023, max compression
+gzip compressed data, was "idev-pystatistics-1.0.1.tar", last modified: Fri Jul 28 20:44:16 2023, max compression
```

## Comparing `idev-pystatistics-1.0.0.tar` & `idev-pystatistics-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 20:29:35.101454 idev-pystatistics-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    15940 2023-07-28 20:29:35.101454 idev-pystatistics-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    15215 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 20:29:35.065869 idev-pystatistics-1.0.0/idev-pystatistics/
-drwxrwxrwx   0        0        0        0 2023-07-28 20:29:35.081869 idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/
--rw-rw-rw-   0        0        0     2106 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/Conversions.py
--rw-rw-rw-   0        0        0     1180 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/Factoring.py
--rw-rw-rw-   0        0        0     5571 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/Lists.py
--rw-rw-rw-   0        0        0    15646 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/NumberTypes.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 20:29:35.100444 idev-pystatistics-1.0.0/idev-pystatistics/idev_pystatistics.egg-info/
--rw-rw-rw-   0        0        0    15940 2023-07-28 20:29:35.000000 idev-pystatistics-1.0.0/idev-pystatistics/idev_pystatistics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-07-28 20:29:35.000000 idev-pystatistics-1.0.0/idev-pystatistics/idev_pystatistics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:29:35.000000 idev-pystatistics-1.0.0/idev-pystatistics/idev_pystatistics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 20:29:35.000000 idev-pystatistics-1.0.0/idev-pystatistics/idev_pystatistics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2023-07-28 20:26:46.000000 idev-pystatistics-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      884 2023-07-28 20:29:35.107458 idev-pystatistics-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      971 2023-07-28 20:28:38.000000 idev-pystatistics-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:44:16.111970 idev-pystatistics-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    16062 2023-07-28 20:44:16.111970 idev-pystatistics-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15335 2023-07-28 20:42:15.000000 idev-pystatistics-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 20:44:16.080653 idev-pystatistics-1.0.1/idev-pystatistics/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:44:16.095026 idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/
+-rw-rw-rw-   0        0        0     2106 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/Conversions.py
+-rw-rw-rw-   0        0        0     1180 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/Factoring.py
+-rw-rw-rw-   0        0        0     5571 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/Lists.py
+-rw-rw-rw-   0        0        0    15646 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/NumberTypes.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:09:26.000000 idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:44:16.110970 idev-pystatistics-1.0.1/idev-pystatistics/idev_pystatistics.egg-info/
+-rw-rw-rw-   0        0        0    16062 2023-07-28 20:44:16.000000 idev-pystatistics-1.0.1/idev-pystatistics/idev_pystatistics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-07-28 20:44:16.000000 idev-pystatistics-1.0.1/idev-pystatistics/idev_pystatistics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:44:16.000000 idev-pystatistics-1.0.1/idev-pystatistics/idev_pystatistics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 20:44:16.000000 idev-pystatistics-1.0.1/idev-pystatistics/idev_pystatistics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2023-07-28 20:42:22.000000 idev-pystatistics-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      884 2023-07-28 20:44:16.113970 idev-pystatistics-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      971 2023-07-28 20:42:35.000000 idev-pystatistics-1.0.1/setup.py
```

### Comparing `idev-pystatistics-1.0.0/LICENSE` & `idev-pystatistics-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idev-pystatistics-1.0.0/PKG-INFO` & `idev-pystatistics-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pystatistics
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python collection of classes and functions to help with numbers along with collections of numbers i.e., statistics.
 Home-page: https://github.com/IrtsaDevelopment/PyStatistics
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyStatistics
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyStatistics/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **PyStatistics**
 A [**python**](https://www.python.org) collection of classes and functions to help with numbers along with collections of numbers i.e., **statistics**.
 <br />
 <br />
+​<br />
+# Installation
+With `git` [GitHub](https://github.com):
+```
+git clone https://github.com/IrtsaDevelopment/PyStatistics.git
+```
+With `pip` [PyPi](https://pypi.org/project/idev-pystatistics/)
+```
+pip install idev-pystatistics
+```
+<br />
+<br />
 <br />
 <br />
 <br />
 
 # Usage
 To import:
 ```py
@@ -473,18 +485,7 @@
 ​
 <br />
 <br />
 <br />
 <br />
 # Additional Notes
 Accuracy may be lost at times when converting between number formats.
-
-​
-<br />
-<br />
-​<br />
-<br />
-<br />
-# Installation
-```sh
-git clone https://github.com/IrtsaDevelopment/PyStatistics.git
-```
```

### Comparing `idev-pystatistics-1.0.0/README.md` & `idev-pystatistics-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # **PyStatistics**
 A [**python**](https://www.python.org) collection of classes and functions to help with numbers along with collections of numbers i.e., **statistics**.
 <br />
 <br />
+​<br />
+# Installation
+With `git` [GitHub](https://github.com):
+```
+git clone https://github.com/IrtsaDevelopment/PyStatistics.git
+```
+With `pip` [PyPi](https://pypi.org/project/idev-pystatistics/)
+```
+pip install idev-pystatistics
+```
+<br />
+<br />
 <br />
 <br />
 <br />
 
 # Usage
 To import:
 ```py
@@ -456,19 +468,8 @@
 ```
 ​
 <br />
 <br />
 <br />
 <br />
 # Additional Notes
-Accuracy may be lost at times when converting between number formats.
-
-​
-<br />
-<br />
-​<br />
-<br />
-<br />
-# Installation
-```sh
-git clone https://github.com/IrtsaDevelopment/PyStatistics.git
-```
+Accuracy may be lost at times when converting between number formats.
```

### Comparing `idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/Conversions.py` & `idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/Conversions.py`

 * *Files identical despite different names*

### Comparing `idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/Factoring.py` & `idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/Factoring.py`

 * *Files identical despite different names*

### Comparing `idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/Lists.py` & `idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/Lists.py`

 * *Files identical despite different names*

### Comparing `idev-pystatistics-1.0.0/idev-pystatistics/PyStatistics/NumberTypes.py` & `idev-pystatistics-1.0.1/idev-pystatistics/PyStatistics/NumberTypes.py`

 * *Files identical despite different names*

### Comparing `idev-pystatistics-1.0.0/idev-pystatistics/idev_pystatistics.egg-info/PKG-INFO` & `idev-pystatistics-1.0.1/idev-pystatistics/idev_pystatistics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pystatistics
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python collection of classes and functions to help with numbers along with collections of numbers i.e., statistics.
 Home-page: https://github.com/IrtsaDevelopment/PyStatistics
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyStatistics
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyStatistics/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **PyStatistics**
 A [**python**](https://www.python.org) collection of classes and functions to help with numbers along with collections of numbers i.e., **statistics**.
 <br />
 <br />
+​<br />
+# Installation
+With `git` [GitHub](https://github.com):
+```
+git clone https://github.com/IrtsaDevelopment/PyStatistics.git
+```
+With `pip` [PyPi](https://pypi.org/project/idev-pystatistics/)
+```
+pip install idev-pystatistics
+```
+<br />
+<br />
 <br />
 <br />
 <br />
 
 # Usage
 To import:
 ```py
@@ -473,18 +485,7 @@
 ​
 <br />
 <br />
 <br />
 <br />
 # Additional Notes
 Accuracy may be lost at times when converting between number formats.
-
-​
-<br />
-<br />
-​<br />
-<br />
-<br />
-# Installation
-```sh
-git clone https://github.com/IrtsaDevelopment/PyStatistics.git
-```
```

### Comparing `idev-pystatistics-1.0.0/pyproject.toml` & `idev-pystatistics-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "idev-pystatistics"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to help with numbers along with collections of numbers i.e., statistics."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `idev-pystatistics-1.0.0/setup.cfg` & `idev-pystatistics-1.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6465 762d 7079 7374 6174 6973   = idev-pystatis
 00000020: 7469 6373 0d0a 7665 7273 696f 6e20 3d20  tics..version = 
-00000030: 312e 302e 300d 0a61 7574 686f 7220 3d20  1.0.0..author = 
+00000030: 312e 302e 310d 0a61 7574 686f 7220 3d20  1.0.1..author = 
 00000040: 4972 7473 6144 6576 656c 6f70 6d65 6e74  IrtsaDevelopment
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2069 7274 7361 2e64 6576 656c 6f70 6d65   irtsa.developme
 00000070: 6e74 4067 6d61 696c 2e63 6f6d 0d0a 6465  nt@gmail.com..de
 00000080: 7363 7269 7074 696f 6e20 3d20 4120 7079  scription = A py
 00000090: 7468 6f6e 2063 6f6c 6c65 6374 696f 6e20  thon collection 
 000000a0: 6f66 2063 6c61 7373 6573 2061 6e64 2066  of classes and f
```

### Comparing `idev-pystatistics-1.0.0/setup.py` & `idev-pystatistics-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "idev-pystatistics",
-    version = "1.0.0",
+    version = "1.0.1",
     author = "IrtsaDevelopment",
     author_email = "irtsa.development@gmail.com",
     description = "A python collection of classes and functions to help with numbers along with collections of numbers i.e., statistics.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IrtsaDevelopment/PyStatistics",
     project_urls = {
```

