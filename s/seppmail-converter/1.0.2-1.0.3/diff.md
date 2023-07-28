# Comparing `tmp/seppmail_converter-1.0.2.tar.gz` & `tmp/seppmail_converter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-1.0.2.tar", max compression
+gzip compressed data, was "seppmail_converter-1.0.3.tar", max compression
```

## Comparing `seppmail_converter-1.0.2.tar` & `seppmail_converter-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-07-28 11:22:56.105512 seppmail_converter-1.0.2/README.md
--rw-r--r--   0        0        0      839 2023-07-28 11:23:27.177927 seppmail_converter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-28 11:23:27.261928 seppmail_converter-1.0.2/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-07-28 11:22:56.105512 seppmail_converter-1.0.2/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     5394 2023-07-28 11:22:56.105512 seppmail_converter-1.0.2/seppmail_converter/main.py
--rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 seppmail_converter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1061 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/README.md
+-rw-r--r--   0        0        0      911 2023-07-28 11:47:10.143686 seppmail_converter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-28 11:47:10.247696 seppmail_converter-1.0.3/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5394 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/seppmail_converter/main.py
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 seppmail_converter-1.0.3/PKG-INFO
```

### Comparing `seppmail_converter-1.0.2/README.md` & `seppmail_converter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.0.2/pyproject.toml` & `seppmail_converter-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "seppmail-converter"
-version = "1.0.2"
+version = "1.0.3"
 description = "Decode SEPPMail emails into EML files"
-license = "MIT"
+license = "AGPL-3.0-or-later"
 authors = ["Daniel Malik <daniel.malik@mhsp.solutions>"]
 readme = "README.md"
 classifiers = ["Environment :: Console"]
+repository = "https://github.com/mhsp/seppmail-converter"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31"
 click = "^8.1.6"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.3"
```

### Comparing `seppmail_converter-1.0.2/seppmail_converter/main.py` & `seppmail_converter-1.0.3/seppmail_converter/main.py`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.0.2/PKG-INFO` & `seppmail_converter-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Decode SEPPMail emails into EML files
-License: MIT
+Home-page: https://github.com/mhsp/seppmail-converter
+License: AGPL-3.0-or-later
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: requests (>=2.31,<3.0)
+Project-URL: Repository, https://github.com/mhsp/seppmail-converter
 Description-Content-Type: text/markdown
 
 # SEPPMail Converter
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
```

