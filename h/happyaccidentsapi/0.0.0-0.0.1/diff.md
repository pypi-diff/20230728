# Comparing `tmp/happyaccidentsapi-0.0.0.tar.gz` & `tmp/happyaccidentsapi-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyaccidentsapi-0.0.0.tar", max compression
+gzip compressed data, was "happyaccidentsapi-0.0.1.tar", max compression
```

## Comparing `happyaccidentsapi-0.0.0.tar` & `happyaccidentsapi-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10198 2023-07-27 11:31:34.153331 happyaccidentsapi-0.0.0/LICENSE
--rw-r--r--   0        0        0     2902 2023-07-28 16:20:56.841138 happyaccidentsapi-0.0.0/README.md
--rw-r--r--   0        0        0      288 2023-07-28 14:05:49.494814 happyaccidentsapi-0.0.0/happyaccidentsapi/__init__.py
--rw-r--r--   0        0        0     8051 2023-07-28 15:44:14.084288 happyaccidentsapi-0.0.0/happyaccidentsapi/_happyaccidentsapi.py
--rw-r--r--   0        0        0      520 2023-07-28 14:05:19.811055 happyaccidentsapi-0.0.0/happyaccidentsapi/_token.py
--rw-r--r--   0        0        0     2847 2023-07-28 13:23:32.859138 happyaccidentsapi-0.0.0/happyaccidentsapi/enums.py
--rw-r--r--   0        0        0      805 2023-07-28 14:05:33.284581 happyaccidentsapi-0.0.0/happyaccidentsapi/errors.py
--rw-r--r--   0        0        0    12581 2023-07-28 16:15:56.041644 happyaccidentsapi-0.0.0/happyaccidentsapi/models.py
--rw-r--r--   0        0        0     1118 2023-07-28 15:17:57.504115 happyaccidentsapi-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 happyaccidentsapi-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10198 2023-07-27 11:31:34.153331 happyaccidentsapi-0.0.1/LICENSE
+-rw-r--r--   0        0        0     1831 2023-07-28 17:01:49.246542 happyaccidentsapi-0.0.1/PYPI.md
+-rw-r--r--   0        0        0      288 2023-07-28 14:05:49.494814 happyaccidentsapi-0.0.1/happyaccidentsapi/__init__.py
+-rw-r--r--   0        0        0     8051 2023-07-28 15:44:14.084288 happyaccidentsapi-0.0.1/happyaccidentsapi/_happyaccidentsapi.py
+-rw-r--r--   0        0        0      520 2023-07-28 14:05:19.811055 happyaccidentsapi-0.0.1/happyaccidentsapi/_token.py
+-rw-r--r--   0        0        0     2847 2023-07-28 13:23:32.859138 happyaccidentsapi-0.0.1/happyaccidentsapi/enums.py
+-rw-r--r--   0        0        0      805 2023-07-28 14:05:33.284581 happyaccidentsapi-0.0.1/happyaccidentsapi/errors.py
+-rw-r--r--   0        0        0    12581 2023-07-28 16:15:56.041644 happyaccidentsapi-0.0.1/happyaccidentsapi/models.py
+-rw-r--r--   0        0        0     1117 2023-07-28 17:05:56.665202 happyaccidentsapi-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 happyaccidentsapi-0.0.1/PKG-INFO
```

### Comparing `happyaccidentsapi-0.0.0/LICENSE` & `happyaccidentsapi-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.0/README.md` & `happyaccidentsapi-0.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-<p align="center">
-  <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/hoopengo/hoopengo/master/images/HappyAccidentsAPI/banner-dark.svg">
-    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/hoopengo/hoopengo/master/images/HappyAccidentsAPI/banner-light.svg">
-    <img alt="banner" src="https://raw.githubusercontent.com/hoopengo/hoopengo/master/images/HappyAccidentsAPI/banner-light.svg" style="max-width: 100%;">
-  </picture>
-</p>
-
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Pypi](https://img.shields.io/pypi/v/happyaccidentsapi.svg)](https://pypi.org/project/happyaccidentsapi/)
-[![Pypi Downloads](https://img.shields.io/pypi/dm/happyaccidentsapi?color=informational&label=pypi%20downloads)](https://pypi.org/project/happyaccidentsapi/)
-[![Python version](https://img.shields.io/pypi/pyversions/happyaccidentsapi.svg)](https://pypi.org/pypi/happyaccidentsapi/)
+Metadata-Version: 2.1
+Name: happyaccidentsapi
+Version: 0.0.1
+Summary: API Wrapper for HappyAccidents
+Home-page: https://github.com/hoopengo/happyaccidentsapi
+License: Apache-2.0
+Keywords: api,happyaccidents,ai
+Author: hoopengo
+Author-email: hoopengo@yandex.ru
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0)
+Requires-Dist: pydantic (==2.0.0)
+Project-URL: Repository, https://github.com/hoopengo/happyaccidentsapi
+Description-Content-Type: text/markdown
+
+<img alt="banner" src="https://raw.githubusercontent.com/hoopengo/hoopengo/master/images/HappyAccidentsAPI/banner-light.svg" style="max-width: 100%;">
 
 ## HappyAccidentsAPI
 
 > At the moment, HappyAccidents has not provided an official API and the library is built on the basis of the client API. Because of this, you may find bugs and shortcomings, if this happened, please provide a report in [Issues.](https://github.com/hoopengo/HappyAccidentsAPI/issues)
 
-## Installation
-
-```sh
-# Via pip
-## Linux/macOS
-python3 -m pip install -U happyaccidentsapi
-
-## Windows
-py -3 -m pip install -U happyaccidentsapi
-
-# Via poetry
-poetry add happyaccideentsapi
-
-# [SOON]Via pacman
-# pacman -Sy python-happyaccidentsapi
-
-```
-
 ## Quick example
 
 ```python
 import asyncio
 
 from happyaccidentsapi import ClientAPI
 from happyaccidentsapi.models import CreateInferenceParams
@@ -62,12 +61,14 @@
     asyncio.run(main())
 ```
 
 NOTE: It is not advised to leave your token directly in your code, as it allows anyone with it to access your account. If you intend to make your code public you should store it securely.
 
 ## Links
 
+- [Repository](https://github.com/hoopengo/HappyAccidentsAPI)
 - [Documentation](https://github.com/hoopengo/HappyAccidentsAPI/tree/master/docs/)
 - [Examples](https://github.com/hoopengo/HappyAccidentsAPI/tree/master/examples/)
 - [How to get token?](https://github.com/hoopengo/HappyAccidentsAPI/blob/master/docs/get_token.md)
 
 [//]: <- [Try it Out](https://t.me/HotBebrasBot)>
+
```

### Comparing `happyaccidentsapi-0.0.0/happyaccidentsapi/_happyaccidentsapi.py` & `happyaccidentsapi-0.0.1/happyaccidentsapi/_happyaccidentsapi.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.0/happyaccidentsapi/_token.py` & `happyaccidentsapi-0.0.1/happyaccidentsapi/_token.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.0/happyaccidentsapi/enums.py` & `happyaccidentsapi-0.0.1/happyaccidentsapi/enums.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.0/happyaccidentsapi/errors.py` & `happyaccidentsapi-0.0.1/happyaccidentsapi/errors.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.0/happyaccidentsapi/models.py` & `happyaccidentsapi-0.0.1/happyaccidentsapi/models.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.0/pyproject.toml` & `happyaccidentsapi-0.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "happyaccidentsapi"
-version = "0.0.0"
+version = "0.0.1"
 description = "API Wrapper for HappyAccidents"
 authors = ["hoopengo <hoopengo@yandex.ru>"]
-readme = ["README.md"]
+readme = ["PYPI.md"]
 license = "Apache-2.0"
 repository = "https://github.com/hoopengo/happyaccidentsapi"
 keywords = ["api", "happyaccidents", "ai"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Libraries",
@@ -19,16 +19,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^2.1.1"
-aiohttp = {extras = ["speedups"], version = "^3.8.5"}
+pydantic = "2.0.0"
+aiohttp = { extras = ["speedups"], version = "^3.8.5" }
 aiofiles = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 
 [build-system]
```

