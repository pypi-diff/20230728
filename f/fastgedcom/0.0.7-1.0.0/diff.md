# Comparing `tmp/fastgedcom-0.0.7.tar.gz` & `tmp/fastgedcom-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-0.0.7.tar", last modified: Mon Jun 26 17:27:15 2023, max compression
+gzip compressed data, was "fastgedcom-1.0.0.tar", last modified: Fri Jul 28 18:55:14 2023, max compression
```

## Comparing `fastgedcom-0.0.7.tar` & `fastgedcom-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.758745 fastgedcom-0.0.7/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4562 2023-06-26 17:27:15.752748 fastgedcom-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2023-06-25 20:57:19.000000 fastgedcom-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.706748 fastgedcom-0.0.7/fastgedcom/
--rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-0.0.7/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0     9663 2023-06-25 22:07:46.000000 fastgedcom-0.0.7/fastgedcom/base.py
--rw-rw-rw-   0        0        0    10946 2023-06-25 22:04:48.000000 fastgedcom-0.0.7/fastgedcom/family_link.py
--rw-rw-rw-   0        0        0     9568 2023-06-19 15:12:18.000000 fastgedcom-0.0.7/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     5215 2023-06-19 15:00:32.000000 fastgedcom-0.0.7/fastgedcom/parser.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.7/fastgedcom/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.741782 fastgedcom-0.0.7/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     4562 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1116 2023-06-26 17:21:40.000000 fastgedcom-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 17:27:15.758745 fastgedcom-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.750746 fastgedcom-0.0.7/test/
--rw-rw-rw-   0        0        0     2144 2023-06-26 16:00:30.000000 fastgedcom-0.0.7/test/test_base.py
--rw-rw-rw-   0        0        0     7527 2023-06-19 15:25:59.000000 fastgedcom-0.0.7/test/test_date_helpers.py
--rw-rw-rw-   0        0        0     4859 2023-06-25 22:04:27.000000 fastgedcom-0.0.7/test/test_family_link.py
--rw-rw-rw-   0        0        0     1670 2023-06-19 15:00:32.000000 fastgedcom-0.0.7/test/test_helpers.py
--rw-rw-rw-   0        0        0     4605 2023-06-19 15:00:32.000000 fastgedcom-0.0.7/test/test_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:55:14.537484 fastgedcom-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4853 2023-07-28 18:55:14.531040 fastgedcom-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3921 2023-07-27 18:32:38.000000 fastgedcom-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 18:55:14.505470 fastgedcom-1.0.0/fastgedcom/
+-rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-1.0.0/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0     9663 2023-07-27 18:54:39.000000 fastgedcom-1.0.0/fastgedcom/base.py
+-rw-rw-rw-   0        0        0    10946 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/fastgedcom/family_link.py
+-rw-rw-rw-   0        0        0     9568 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     5215 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/fastgedcom/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:55:14.520667 fastgedcom-1.0.0/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     4853 2023-07-28 18:55:14.000000 fastgedcom-1.0.0/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-07-28 18:55:14.000000 fastgedcom-1.0.0/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:55:14.000000 fastgedcom-1.0.0/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-28 18:55:14.000000 fastgedcom-1.0.0/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 18:55:14.000000 fastgedcom-1.0.0/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1128 2023-07-28 18:37:09.000000 fastgedcom-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:55:14.537484 fastgedcom-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 18:55:14.531040 fastgedcom-1.0.0/test/
+-rw-rw-rw-   0        0        0     2144 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/test/test_base.py
+-rw-rw-rw-   0        0        0     7527 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/test/test_date_helpers.py
+-rw-rw-rw-   0        0        0     4859 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/test/test_family_link.py
+-rw-rw-rw-   0        0        0     1670 2023-06-30 21:00:00.000000 fastgedcom-1.0.0/test/test_helpers.py
+-rw-rw-rw-   0        0        0     4605 2023-07-27 18:48:31.000000 fastgedcom-1.0.0/test/test_parser.py
```

### Comparing `fastgedcom-0.0.7/LICENSE` & `fastgedcom-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/PKG-INFO` & `fastgedcom-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.7
+Version: 1.0.0
 Summary: A lightweight tool to parse, browse and edit gedcom files.
 Author-email: Gatien Bouyer <gatien.bouyer.dev@gmail.com>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
 Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
 Keywords: fastgedcom,gedcom,parser,genealogy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastGedcom
 
 A lightweight tool to parse, browse and edit gedcom files.
 
+Install FastGedcom using pip from [its PyPI page](https://pypi.org/project/fastgedcom/):
 ```bash
 pip install fastgedcom
 ```
 
 ## Features
 Easy to write! Free choice of fields, data, and formatting.
 ```python
@@ -40,15 +41,15 @@
 print(format_date(birth_date))
 ```
 
 The syntax is flexible and permissive. If you don't like magic operator overloads, you can use standard methods!
 
 It supports gedcom files encoded in UTF-8 (with and without BOM), UTF-16 (also named UNICODE), ANSI, and ANSEL.
 
-If a field is missing, you will get a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) containing an empty string. This reduces the boiler plate code. You can differentiate [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) and [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine) with a simple boolean check.
+If a field is missing, you will get a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) containing an empty string. This help reducing the boiler plate code massively. And, you can differentiate a [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine) from a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) with a simple boolean check.
 ```python
 
 indi = document["@I13@"]
 death = indi > "DEAT"
 if not death:
 	print("No DEAT field. The person is alive")
 # Can continue anyway
@@ -58,24 +59,24 @@
 Typehints for salvation! Autocompletion and type checking make development so much easier.
 
 - There are only 3 main classes: [Document](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Document), [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine), and [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine).
 - There are type aliases for code clarity: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
 
 ## Why FastGedcom ?
 
-FastGedcom's aim is to keep the code close to your gedcom files. So, you don't have to learn what FastGedcom does for you. The content of your gedcom file is what you get. The data processing is optional to best suit your needs.
+FastGedcom's aim is to keep the code close to your gedcom files. So, you don't have to learn what FastGedcom does, the data you have, is the data you get. The content of the gedcom file is unchanged. The data processing is optional to best suit your needs. FastGedcom is more of a starting point of your data processing than a all-round full-featured librairy.
 
-The name **FastGedcom** doesn't just come from its ease of use. Getting relatives can be done quickly. That's what the [FamilyLink](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/family_link/index.html#fastgedcom.family_link.FamilyLink) class is all about. [Here](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) are the benchmark I used.
+The name **FastGedcom** doesn't just come from its ease of use. Parsing is really fast. And, for getting the relatives of a person as fast as possible, there is the [FamilyLink](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/family_link/index.html#fastgedcom.family_link.FamilyLink) class. [Here](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) are the benchmark I used.
 
 ## Documentation and examples
 
 Want to see more code? [Here are some examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)
 
 The documentation of FastGedcom is available [here](https://fastgedcom.readthedocs.io/en/latest/) on ReadTheDocs.
 
-## Feedbacks
+## Feedback
 
-Feedbacks are welcome, and they will be greatly appreciated!
+Feedback are welcome, and they will be greatly appreciated!
 
 If you like this project, consider putting a star on [Github](https://github.com/GatienBouyer/fastgedcom), thank you!
 
 For any feedback or question, please feel free to contact me by email at gatien.bouyer.dev@gmail.com or via [Github issues](https://github.com/GatienBouyer/fastgedcom/issues).
```

### Comparing `fastgedcom-0.0.7/README.md` & `fastgedcom-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # FastGedcom
 
 A lightweight tool to parse, browse and edit gedcom files.
 
+Install FastGedcom using pip from [its PyPI page](https://pypi.org/project/fastgedcom/):
 ```bash
 pip install fastgedcom
 ```
 
 ## Features
 Easy to write! Free choice of fields, data, and formatting.
 ```python
@@ -18,15 +19,15 @@
 print(format_date(birth_date))
 ```
 
 The syntax is flexible and permissive. If you don't like magic operator overloads, you can use standard methods!
 
 It supports gedcom files encoded in UTF-8 (with and without BOM), UTF-16 (also named UNICODE), ANSI, and ANSEL.
 
-If a field is missing, you will get a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) containing an empty string. This reduces the boiler plate code. You can differentiate [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) and [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine) with a simple boolean check.
+If a field is missing, you will get a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) containing an empty string. This help reducing the boiler plate code massively. And, you can differentiate a [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine) from a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) with a simple boolean check.
 ```python
 
 indi = document["@I13@"]
 death = indi > "DEAT"
 if not death:
 	print("No DEAT field. The person is alive")
 # Can continue anyway
@@ -36,24 +37,24 @@
 Typehints for salvation! Autocompletion and type checking make development so much easier.
 
 - There are only 3 main classes: [Document](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Document), [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine), and [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine).
 - There are type aliases for code clarity: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
 
 ## Why FastGedcom ?
 
-FastGedcom's aim is to keep the code close to your gedcom files. So, you don't have to learn what FastGedcom does for you. The content of your gedcom file is what you get. The data processing is optional to best suit your needs.
+FastGedcom's aim is to keep the code close to your gedcom files. So, you don't have to learn what FastGedcom does, the data you have, is the data you get. The content of the gedcom file is unchanged. The data processing is optional to best suit your needs. FastGedcom is more of a starting point of your data processing than a all-round full-featured librairy.
 
-The name **FastGedcom** doesn't just come from its ease of use. Getting relatives can be done quickly. That's what the [FamilyLink](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/family_link/index.html#fastgedcom.family_link.FamilyLink) class is all about. [Here](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) are the benchmark I used.
+The name **FastGedcom** doesn't just come from its ease of use. Parsing is really fast. And, for getting the relatives of a person as fast as possible, there is the [FamilyLink](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/family_link/index.html#fastgedcom.family_link.FamilyLink) class. [Here](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) are the benchmark I used.
 
 ## Documentation and examples
 
 Want to see more code? [Here are some examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)
 
 The documentation of FastGedcom is available [here](https://fastgedcom.readthedocs.io/en/latest/) on ReadTheDocs.
 
-## Feedbacks
+## Feedback
 
-Feedbacks are welcome, and they will be greatly appreciated!
+Feedback are welcome, and they will be greatly appreciated!
 
 If you like this project, consider putting a star on [Github](https://github.com/GatienBouyer/fastgedcom), thank you!
 
 For any feedback or question, please feel free to contact me by email at gatien.bouyer.dev@gmail.com or via [Github issues](https://github.com/GatienBouyer/fastgedcom/issues).
```

### Comparing `fastgedcom-0.0.7/fastgedcom/base.py` & `fastgedcom-1.0.0/fastgedcom/base.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/fastgedcom/family_link.py` & `fastgedcom-1.0.0/fastgedcom/family_link.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/fastgedcom/helpers.py` & `fastgedcom-1.0.0/fastgedcom/helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/fastgedcom/parser.py` & `fastgedcom-1.0.0/fastgedcom/parser.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/fastgedcom.egg-info/PKG-INFO` & `fastgedcom-1.0.0/fastgedcom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.7
+Version: 1.0.0
 Summary: A lightweight tool to parse, browse and edit gedcom files.
 Author-email: Gatien Bouyer <gatien.bouyer.dev@gmail.com>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
 Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
 Keywords: fastgedcom,gedcom,parser,genealogy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastGedcom
 
 A lightweight tool to parse, browse and edit gedcom files.
 
+Install FastGedcom using pip from [its PyPI page](https://pypi.org/project/fastgedcom/):
 ```bash
 pip install fastgedcom
 ```
 
 ## Features
 Easy to write! Free choice of fields, data, and formatting.
 ```python
@@ -40,15 +41,15 @@
 print(format_date(birth_date))
 ```
 
 The syntax is flexible and permissive. If you don't like magic operator overloads, you can use standard methods!
 
 It supports gedcom files encoded in UTF-8 (with and without BOM), UTF-16 (also named UNICODE), ANSI, and ANSEL.
 
-If a field is missing, you will get a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) containing an empty string. This reduces the boiler plate code. You can differentiate [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) and [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine) with a simple boolean check.
+If a field is missing, you will get a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) containing an empty string. This help reducing the boiler plate code massively. And, you can differentiate a [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine) from a [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine) with a simple boolean check.
 ```python
 
 indi = document["@I13@"]
 death = indi > "DEAT"
 if not death:
 	print("No DEAT field. The person is alive")
 # Can continue anyway
@@ -58,24 +59,24 @@
 Typehints for salvation! Autocompletion and type checking make development so much easier.
 
 - There are only 3 main classes: [Document](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Document), [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine), and [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine).
 - There are type aliases for code clarity: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
 
 ## Why FastGedcom ?
 
-FastGedcom's aim is to keep the code close to your gedcom files. So, you don't have to learn what FastGedcom does for you. The content of your gedcom file is what you get. The data processing is optional to best suit your needs.
+FastGedcom's aim is to keep the code close to your gedcom files. So, you don't have to learn what FastGedcom does, the data you have, is the data you get. The content of the gedcom file is unchanged. The data processing is optional to best suit your needs. FastGedcom is more of a starting point of your data processing than a all-round full-featured librairy.
 
-The name **FastGedcom** doesn't just come from its ease of use. Getting relatives can be done quickly. That's what the [FamilyLink](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/family_link/index.html#fastgedcom.family_link.FamilyLink) class is all about. [Here](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) are the benchmark I used.
+The name **FastGedcom** doesn't just come from its ease of use. Parsing is really fast. And, for getting the relatives of a person as fast as possible, there is the [FamilyLink](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/family_link/index.html#fastgedcom.family_link.FamilyLink) class. [Here](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) are the benchmark I used.
 
 ## Documentation and examples
 
 Want to see more code? [Here are some examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)
 
 The documentation of FastGedcom is available [here](https://fastgedcom.readthedocs.io/en/latest/) on ReadTheDocs.
 
-## Feedbacks
+## Feedback
 
-Feedbacks are welcome, and they will be greatly appreciated!
+Feedback are welcome, and they will be greatly appreciated!
 
 If you like this project, consider putting a star on [Github](https://github.com/GatienBouyer/fastgedcom), thank you!
 
 For any feedback or question, please feel free to contact me by email at gatien.bouyer.dev@gmail.com or via [Github issues](https://github.com/GatienBouyer/fastgedcom/issues).
```

### Comparing `fastgedcom-0.0.7/pyproject.toml` & `fastgedcom-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastgedcom"
-version = "0.0.7"
+version = "1.0.0"
 description = "A lightweight tool to parse, browse and edit gedcom files."
 keywords = ["fastgedcom", "gedcom", "parser", "genealogy"]
 authors = [
 	{name="Gatien Bouyer", email="gatien.bouyer.dev@gmail.com"},
 ]
 readme = "README.md"
 license = {text = "MIT License"}
@@ -15,15 +15,15 @@
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Topic :: Sociology :: Genealogy",
 	"Intended Audience :: Developers",
 	"Operating System :: OS Independent",
-	"Development Status :: 3 - Alpha",
+	"Development Status :: 5 - Production/Stable",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/GatienBouyer/fastgedcom/issues"
 "Source" = "https://github.com/GatienBouyer/fastgedcom"
 "Documentation" = "https://fastgedcom.readthedocs.io/en/latest/"
```

### Comparing `fastgedcom-0.0.7/test/test_base.py` & `fastgedcom-1.0.0/test/test_base.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/test/test_date_helpers.py` & `fastgedcom-1.0.0/test/test_date_helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/test/test_family_link.py` & `fastgedcom-1.0.0/test/test_family_link.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/test/test_helpers.py` & `fastgedcom-1.0.0/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.7/test/test_parser.py` & `fastgedcom-1.0.0/test/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 			guess_lower = guess.lower() if guess else None
 			self.assertEqual(guess_lower, encoding, f"File: {filename}")
 
 	def test_string_io_parsing(self) -> None:
 		stream = StringIO("0 HEAD\n1 GEDC\n2 VERS 5.5\n1 CHAR UTF-8\n0 @I1@ INDI\n1 NAME éàç /ÉÀÇ/\n2 SURN ÉÀÇ\n2 GIVN éàç\n1 SEX M")
 		self._test_parsing(stream, 9)
 	
-	def test_test_parsing(self) -> None:
+	def test_text_parsing(self) -> None:
 		text = """
 		0 HEAD
 		1 GEDC
 		2 VERS 5.5
 		1 CHAR UTF-8
 		0 @I1@ INDI
 		1 NAME éàç /ÉÀÇ/
```

