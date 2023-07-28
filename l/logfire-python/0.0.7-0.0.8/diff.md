# Comparing `tmp/logfire-python-0.0.7.tar.gz` & `tmp/logfire-python-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-python-0.0.7.tar", last modified: Tue Jun 20 15:29:30 2023, max compression
+gzip compressed data, was "logfire-python-0.0.8.tar", last modified: Fri Jul 28 07:24:23 2023, max compression
```

## Comparing `logfire-python-0.0.7.tar` & `logfire-python-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 15:29:30.038343 logfire-python-0.0.7/
--rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3861 2023-06-20 15:29:30.037341 logfire-python-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 15:29:30.018965 logfire-python-0.0.7/logfire/
--rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.7/logfire/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:29:30.022965 logfire-python-0.0.7/logfire/__pycache__/
--rw-rw-rw-   0        0        0      539 2023-06-20 11:04:18.000000 logfire-python-0.0.7/logfire/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      406 2023-06-20 11:04:18.000000 logfire-python-0.0.7/logfire/__pycache__/compat.cpython-311.pyc
--rw-rw-rw-   0        0        0     3574 2023-06-20 11:04:18.000000 logfire-python-0.0.7/logfire/__pycache__/flusher.cpython-311.pyc
--rw-rw-rw-   0        0        0     1462 2023-06-20 11:04:18.000000 logfire-python-0.0.7/logfire/__pycache__/formatter.cpython-311.pyc
--rw-rw-rw-   0        0        0     3854 2023-06-20 13:22:56.000000 logfire-python-0.0.7/logfire/__pycache__/frame.cpython-311.pyc
--rw-rw-rw-   0        0        0     3800 2023-06-20 13:22:56.000000 logfire-python-0.0.7/logfire/__pycache__/handler.cpython-311.pyc
--rw-rw-rw-   0        0        0     2627 2023-06-20 11:04:18.000000 logfire-python-0.0.7/logfire/__pycache__/helpers.cpython-311.pyc
--rw-rw-rw-   0        0        0     1367 2023-06-20 11:04:18.000000 logfire-python-0.0.7/logfire/__pycache__/uploader.cpython-311.pyc
--rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.7/logfire/compat.py
--rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.7/logfire/flusher.py
--rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.7/logfire/formatter.py
--rw-rw-rw-   0        0        0     2758 2023-06-20 13:21:38.000000 logfire-python-0.0.7/logfire/frame.py
--rw-rw-rw-   0        0        0     2680 2023-06-20 12:19:35.000000 logfire-python-0.0.7/logfire/handler.py
--rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.7/logfire/helpers.py
--rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.7/logfire/uploader.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:29:30.032999 logfire-python-0.0.7/logfire_python.egg-info/
--rw-rw-rw-   0        0        0     3861 2023-06-20 15:29:29.000000 logfire-python-0.0.7/logfire_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-06-20 15:29:29.000000 logfire-python-0.0.7/logfire_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 15:29:29.000000 logfire-python-0.0.7/logfire_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-06-20 15:29:29.000000 logfire-python-0.0.7/logfire_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 15:29:29.000000 logfire-python-0.0.7/logfire_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1357 2023-06-20 15:29:26.000000 logfire-python-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 15:29:30.038343 logfire-python-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:29:30.037341 logfire-python-0.0.7/tests/
--rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0     5206 2023-06-06 06:50:49.000000 logfire-python-0.0.7/tests/test_flusher.py
--rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.7/tests/test_formatter.py
--rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.7/tests/test_frame.py
--rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.7/tests/test_handler.py
--rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.7/tests/test_helpers.py
--rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.7/tests/test_uploader.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-06-22 13:06:58.000000 logfire-python-0.0.8/LICENSE.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-22 13:06:58.000000 logfire-python-0.0.8/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-07-28 07:24:23.797150 logfire-python-0.0.8/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-28 07:22:25.000000 logfire-python-0.0.8/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/logfire/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      141 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/compat.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2998 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/flusher.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/formatter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2023-06-22 13:08:01.000000 logfire-python-0.0.8/logfire/frame.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-07-28 07:09:44.000000 logfire-python-0.0.8/logfire/handler.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/helpers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      588 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/uploader.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/logfire_python.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1318 2023-07-28 07:22:26.000000 logfire-python-0.0.8/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      222 2023-06-22 13:06:58.000000 logfire-python-0.0.8/requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-28 07:24:23.797150 logfire-python-0.0.8/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-06-22 13:06:58.000000 logfire-python-0.0.8/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5062 2023-07-28 07:22:24.000000 logfire-python-0.0.8/tests/test_flusher.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5264 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_formatter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1955 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_frame.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4337 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_handler.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1846 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_helpers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_uploader.py
```

### Comparing `logfire-python-0.0.7/LICENSE.md` & `logfire-python-0.0.8/LICENSE.md`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-# License
-
-Copyright 2023 Logfire
-
-Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
-
+# License
+
+Copyright 2023 Logfire
+
+Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
+
 THE SOFTWARE IS PROVIDED “AS IS” AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `logfire-python-0.0.7/PKG-INFO` & `logfire-python-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-Metadata-Version: 2.1
-Name: logfire-python
-Version: 0.0.7
-Summary: Logfire.sh client library
-Author-email: Logfire <support@logfire.sh>
-Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
-Keywords: api,logfire,logging,client
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-# Logfire - Python Logging Made Easy
-
-
-[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
-[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
-
-
-Collect logs directly from any Python code, including Django.
-
-[Logfire](https://logfire.sh) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.sh/). 
-
-### Features
-- Simple integration. Integrates with the Python `logging` library.
-- Support for structured logging and events.
-- Automatically captures useful context.
-- Performant, light weight, with a thoughtful design.
-
-### Supported language versions
-- Python 3.6.5 or newer
-- `pip` 20.0.2 or newer
-
-# Installation
-Install the Logfire Python client library using the `pip` command:
-
-```bash
-pip install logfire-python
-```
-
-*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
-
----
-
-# Example project
-
-To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
-
-## Download and install the example project
-
-You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
-
-```bash
-pip install logfire-python
-```
-
- ## Run the example project
- 
- To run the example application, simply run the following command:
-
-```bash
-python main.py <source-token>
-```
-
-*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
-
-
-If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
-
-```
-Output:
-All done! You can check your logs now.
-```
-
-This example project will create a total of 6 logs. Each corresponding to its respective method.
-
-## Explore how example project works
- 
-Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
- 
----
- 
-## Get in touch
-
-Have any questions? Please explore the Logfire [documentation](https://docs.logfire.sh/) or contact our [support](https://support@logfire.sh).
+Metadata-Version: 2.1
+Name: logfire-python
+Version: 0.0.8
+Summary: Logfire.ai client library
+Author-email: Logfire <support@logfire.ai>
+Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
+Keywords: api,logfire,logging,client
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
+# Logfire - Python Logging Made Easy
+
+
+[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
+[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
+
+
+Collect logs directly from any Python code, including Django.
+
+[Logfire](https://logfire.ai) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.ai/). 
+
+### Features
+- Simple integration. Integrates with the Python `logging` library.
+- Support for structured logging and events.
+- Automatically captures useful context.
+- Performant, light weight, with a thoughtful design.
+
+### Supported language versions
+- Python 3.6.5 or newer
+- `pip` 20.0.2 or newer
+
+# Installation
+Install the Logfire Python client library using the `pip` command:
+
+```bash
+pip install logfire-python
+```
+
+*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
+
+---
+
+# Example project
+
+To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
+
+## Download and install the example project
+
+You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
+
+```bash
+pip install logfire-python
+```
+
+ ## Run the example project
+ 
+ To run the example application, simply run the following command:
+
+```bash
+python main.py <source-token>
+```
+
+*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
+
+
+If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
+
+```
+Output:
+All done! You can check your logs now.
+```
+
+This example project will create a total of 6 logs. Each corresponding to its respective method.
+
+## Explore how example project works
+ 
+Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
+ 
+---
+ 
+## Get in touch
+
+Have any questions? Please explore the Logfire [documentation](https://docs.ai/) or contact our [support](https://support@logfire.ai).
```

### Comparing `logfire-python-0.0.7/README.md` & `logfire-python-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
 [![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
 
 
 Collect logs directly from any Python code, including Django.
 
-[Logfire](https://logfire.sh) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.sh/). 
+[Logfire](https://logfire.ai) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.ai/). 
 
 ### Features
 - Simple integration. Integrates with the Python `logging` library.
 - Support for structured logging and events.
 - Automatically captures useful context.
 - Performant, light weight, with a thoughtful design.
 
@@ -66,8 +66,8 @@
  
 Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
  
 ---
  
 ## Get in touch
 
-Have any questions? Please explore the Logfire [documentation](https://docs.logfire.sh/) or contact our [support](https://support@logfire.sh).
+Have any questions? Please explore the Logfire [documentation](https://docs.ai/) or contact our [support](https://support@logfire.ai).
```

### Comparing `logfire-python-0.0.7/logfire/flusher.py` & `logfire-python-0.0.8/logfire/flusher.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/logfire/formatter.py` & `logfire-python-0.0.8/logfire/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/logfire/frame.py` & `logfire-python-0.0.8/logfire/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from os import path
 import __main__
 
 def create_frame(record, message, context, include_extra_attributes=False):
     r = record.__dict__
     frame = {}
-    # Python 3 only solution if we ever drop Python 2.7
+    # Python 3 only solution if we ever drop Python 2.7.
     # frame['dt'] = datetime.utcfromtimestamp(r['created']).replace(tzinfo=timezone.utc).isoformat()
     frame['dt'] = "{}+00:00".format(datetime.utcfromtimestamp(r['created']).isoformat())
     frame['level'] = level = _levelname(r['levelname'])
     frame['severity'] = int(r['levelno'] / 10)
     frame['message'] = message
     frame['context'] = ctx = {}
```

### Comparing `logfire-python-0.0.7/logfire/handler.py` & `logfire-python-0.0.8/logfire/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from __future__ import print_function, unicode_literals
-import logging
-import multiprocessing
-
-from .compat import queue
-from .helpers import DEFAULT_CONTEXT
-from .flusher import FlushWorker
-from .uploader import Uploader
-from .frame import create_frame
-
-DEFAULT_HOST = 'https://in.logfire.sh'
-DEFAULT_BUFFER_CAPACITY = 1000
-DEFAULT_FLUSH_INTERVAL = 1
-DEFAULT_RAISE_EXCEPTIONS = False
-DEFAULT_DROP_EXTRA_EVENTS = True
-DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
-
-
-class LogfireHandler(logging.Handler):
-    def __init__(self,
-                 source_token,
-                 host=DEFAULT_HOST,
-                 buffer_capacity=DEFAULT_BUFFER_CAPACITY,
-                 flush_interval=DEFAULT_FLUSH_INTERVAL,
-                 raise_exceptions=DEFAULT_RAISE_EXCEPTIONS,
-                 drop_extra_events=DEFAULT_DROP_EXTRA_EVENTS,
-                 include_extra_attributes=DEFAULT_INCLUDE_EXTRA_ATTRIBUTES,
-                 context=DEFAULT_CONTEXT,
-                 level=logging.NOTSET):
-        super(LogfireHandler, self).__init__(level=level)
-        self.source_token = source_token
-        self.host = host
-        self.context = context
-        self.pipe = multiprocessing.JoinableQueue(maxsize=buffer_capacity)
-        self.uploader = Uploader(self.source_token, self.host)
-        self.drop_extra_events = drop_extra_events
-        self.include_extra_attributes = include_extra_attributes
-        self.buffer_capacity = buffer_capacity
-        self.flush_interval = flush_interval
-        self.raise_exceptions = raise_exceptions
-        self.dropcount = 0
-        self.flush_thread = FlushWorker(
-            self.uploader,
-            self.pipe,
-            self.buffer_capacity,
-            self.flush_interval
-        )
-        if self._is_main_process():
-            self.flush_thread.start()
-
-    def _is_main_process(self):
-        return multiprocessing.current_process()._parent_pid == None
-
-    def emit(self, record):
-        try:
-            if self._is_main_process() and not self.flush_thread.is_alive():
-                self.flush_thread.start()
-            message = self.format(record)
-            frame = create_frame(record, message, self.context, include_extra_attributes=self.include_extra_attributes)
-            try:
-                self.pipe.put(frame, block=(not self.drop_extra_events))
-            except queue.Full:
-                # Only raised when not blocking, which means that extra events
-                # should be dropped.
-                self.dropcount += 1
-                pass
-        except Exception as e:
-            if self.raise_exceptions:
+from __future__ import print_function, unicode_literals
+import logging
+import multiprocessing
+
+from .compat import queue
+from .helpers import DEFAULT_CONTEXT
+from .flusher import FlushWorker
+from .uploader import Uploader
+from .frame import create_frame
+
+DEFAULT_HOST = 'https://in.logfire.ai'
+DEFAULT_BUFFER_CAPACITY = 1000
+DEFAULT_FLUSH_INTERVAL = 1
+DEFAULT_RAISE_EXCEPTIONS = False
+DEFAULT_DROP_EXTRA_EVENTS = True
+DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
+
+
+class LogfireHandler(logging.Handler):
+    def __init__(self,
+                 source_token,
+                 host=DEFAULT_HOST,
+                 buffer_capacity=DEFAULT_BUFFER_CAPACITY,
+                 flush_interval=DEFAULT_FLUSH_INTERVAL,
+                 raise_exceptions=DEFAULT_RAISE_EXCEPTIONS,
+                 drop_extra_events=DEFAULT_DROP_EXTRA_EVENTS,
+                 include_extra_attributes=DEFAULT_INCLUDE_EXTRA_ATTRIBUTES,
+                 context=DEFAULT_CONTEXT,
+                 level=logging.NOTSET):
+        super(LogfireHandler, self).__init__(level=level)
+        self.source_token = source_token
+        self.host = host
+        self.context = context
+        self.pipe = multiprocessing.JoinableQueue(maxsize=buffer_capacity)
+        self.uploader = Uploader(self.source_token, self.host)
+        self.drop_extra_events = drop_extra_events
+        self.include_extra_attributes = include_extra_attributes
+        self.buffer_capacity = buffer_capacity
+        self.flush_interval = flush_interval
+        self.raise_exceptions = raise_exceptions
+        self.dropcount = 0
+        self.flush_thread = FlushWorker(
+            self.uploader,
+            self.pipe,
+            self.buffer_capacity,
+            self.flush_interval
+        )
+        if self._is_main_process():
+            self.flush_thread.start()
+
+    def _is_main_process(self):
+        return multiprocessing.current_process()._parent_pid == None
+
+    def emit(self, record):
+        try:
+            if self._is_main_process() and not self.flush_thread.is_alive():
+                self.flush_thread.start()
+            message = self.format(record)
+            frame = create_frame(record, message, self.context, include_extra_attributes=self.include_extra_attributes)
+            try:
+                self.pipe.put(frame, block=(not self.drop_extra_events))
+            except queue.Full:
+                # Only raised when not blocking, which means that extra events
+                # should be dropped.
+                self.dropcount += 1
+                pass
+        except Exception as e:
+            if self.raise_exceptions:
                 raise e
```

### Comparing `logfire-python-0.0.7/logfire/helpers.py` & `logfire-python-0.0.8/logfire/helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/logfire/uploader.py` & `logfire-python-0.0.8/logfire/uploader.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/logfire_python.egg-info/PKG-INFO` & `logfire-python-0.0.8/logfire_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-Metadata-Version: 2.1
-Name: logfire-python
-Version: 0.0.7
-Summary: Logfire.sh client library
-Author-email: Logfire <support@logfire.sh>
-Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
-Keywords: api,logfire,logging,client
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-# Logfire - Python Logging Made Easy
-
-
-[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
-[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
-
-
-Collect logs directly from any Python code, including Django.
-
-[Logfire](https://logfire.sh) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.sh/). 
-
-### Features
-- Simple integration. Integrates with the Python `logging` library.
-- Support for structured logging and events.
-- Automatically captures useful context.
-- Performant, light weight, with a thoughtful design.
-
-### Supported language versions
-- Python 3.6.5 or newer
-- `pip` 20.0.2 or newer
-
-# Installation
-Install the Logfire Python client library using the `pip` command:
-
-```bash
-pip install logfire-python
-```
-
-*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
-
----
-
-# Example project
-
-To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
-
-## Download and install the example project
-
-You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
-
-```bash
-pip install logfire-python
-```
-
- ## Run the example project
- 
- To run the example application, simply run the following command:
-
-```bash
-python main.py <source-token>
-```
-
-*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
-
-
-If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
-
-```
-Output:
-All done! You can check your logs now.
-```
-
-This example project will create a total of 6 logs. Each corresponding to its respective method.
-
-## Explore how example project works
- 
-Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
- 
----
- 
-## Get in touch
-
-Have any questions? Please explore the Logfire [documentation](https://docs.logfire.sh/) or contact our [support](https://support@logfire.sh).
+Metadata-Version: 2.1
+Name: logfire-python
+Version: 0.0.8
+Summary: Logfire.ai client library
+Author-email: Logfire <support@logfire.ai>
+Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
+Keywords: api,logfire,logging,client
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
+# Logfire - Python Logging Made Easy
+
+
+[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
+[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
+
+
+Collect logs directly from any Python code, including Django.
+
+[Logfire](https://logfire.ai) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.ai/). 
+
+### Features
+- Simple integration. Integrates with the Python `logging` library.
+- Support for structured logging and events.
+- Automatically captures useful context.
+- Performant, light weight, with a thoughtful design.
+
+### Supported language versions
+- Python 3.6.5 or newer
+- `pip` 20.0.2 or newer
+
+# Installation
+Install the Logfire Python client library using the `pip` command:
+
+```bash
+pip install logfire-python
+```
+
+*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
+
+---
+
+# Example project
+
+To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
+
+## Download and install the example project
+
+You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
+
+```bash
+pip install logfire-python
+```
+
+ ## Run the example project
+ 
+ To run the example application, simply run the following command:
+
+```bash
+python main.py <source-token>
+```
+
+*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
+
+
+If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
+
+```
+Output:
+All done! You can check your logs now.
+```
+
+This example project will create a total of 6 logs. Each corresponding to its respective method.
+
+## Explore how example project works
+ 
+Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
+ 
+---
+ 
+## Get in touch
+
+Have any questions? Please explore the Logfire [documentation](https://docs.ai/) or contact our [support](https://support@logfire.ai).
```

### Comparing `logfire-python-0.0.7/logfire_python.egg-info/SOURCES.txt` & `logfire-python-0.0.8/logfire_python.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 logfire/compat.py
 logfire/flusher.py
 logfire/formatter.py
 logfire/frame.py
 logfire/handler.py
 logfire/helpers.py
 logfire/uploader.py
-logfire/__pycache__/__init__.cpython-311.pyc
-logfire/__pycache__/compat.cpython-311.pyc
-logfire/__pycache__/flusher.cpython-311.pyc
-logfire/__pycache__/formatter.cpython-311.pyc
-logfire/__pycache__/frame.cpython-311.pyc
-logfire/__pycache__/handler.cpython-311.pyc
-logfire/__pycache__/helpers.cpython-311.pyc
-logfire/__pycache__/uploader.cpython-311.pyc
 logfire_python.egg-info/PKG-INFO
 logfire_python.egg-info/SOURCES.txt
 logfire_python.egg-info/dependency_links.txt
 logfire_python.egg-info/requires.txt
 logfire_python.egg-info/top_level.txt
 tests/__init__.py
 tests/test_flusher.py
```

### Comparing `logfire-python-0.0.7/pyproject.toml` & `logfire-python-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "logfire-python"
-version = "0.0.7"
-description = "Logfire.sh client library"
-readme = "README.md"
-authors = [{ name = "Logfire", email = "support@logfire.sh" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: ISC License (ISCL)",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-]
-keywords = ["api", "logfire", "logging", "client"]
-dependencies = [
-    "requests",
-    "msgpack",
-]
-
-[project.optional-dependencies]
-dev = ["coverage>=3.7.1", "httpretty>=0.9.4", "nose>=1.3.7", "unittest2>=0.8.0", "mock>=1.0.1"]
-
-[project.urls]
-Homepage = "https://github.com/logfire-sh/logfire-python"
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "logfire-python"
+version = "0.0.8"
+description = "Logfire.ai client library"
+readme = "README.md"
+authors = [{ name = "Logfire", email = "support@logfire.ai" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: ISC License (ISCL)",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 2.7",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+keywords = ["api", "logfire", "logging", "client"]
+dependencies = [
+    "requests",
+    "msgpack",
+]
+
+[project.optional-dependencies]
+dev = ["coverage>=3.7.1", "httpretty>=0.9.4", "nose>=1.3.7", "unittest2>=0.8.0", "mock>=1.0.1"]
+
+[project.urls]
+Homepage = "https://github.com/logfire-sh/logfire-python"
```

### Comparing `logfire-python-0.0.7/tests/test_flusher.py` & `logfire-python-0.0.8/tests/test_flusher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-import mock
-import time
-import threading
-import unittest2
-
-from logfire.compat import queue
-from logfire.flusher import RETRY_SCHEDULE
-from logfire.flusher import FlushWorker
-from logfire.uploader import Uploader
-
-
-class TestFlushWorker(unittest2.TestCase):
-    host = 'https://in.logfire.sh'
-    source_token = 'dummy_source_token'
-    buffer_capacity = 5
-    flush_interval = 2
-
-    def _setup_worker(self, uploader=None):
-        pipe = queue.Queue(maxsize=self.buffer_capacity)
-        uploader = uploader or Uploader(self.source_token, self.host)
-        fw = FlushWorker(uploader, pipe, self.buffer_capacity, self.flush_interval)
-        return pipe, uploader, fw
-
-    def test_is_thread(self):
-        pipe, uploader, fw = self._setup_worker()
-        self.assertIsInstance(fw, threading.Thread)
-
-    def test_flushes_when_queue_is_full(self):
-        first_frame = list(range(self.buffer_capacity))
-        second_frame = list(range(self.buffer_capacity, self.buffer_capacity * 2))
-        self.calls = 0
-        self.flush_interval = 1000
-
-        def uploader(frame):
-            self.calls += 1
-            self.assertEqual(frame, first_frame)
-            return mock.MagicMock(status_code=202)
-
-        pipe, _, fw = self._setup_worker(uploader)
-
-        for log in first_frame:
-            pipe.put(log, block=False)
-
-        t1 = time.time()
-        fw.step()
-        t2 = time.time()
-        self.assertLess(t2 - t1, self.flush_interval)
-
-        self.assertEqual(self.calls, 1)
-
-    @mock.patch('logfire.flusher._calculate_time_remaining')
-    def test_flushes_after_interval(self, calculate_time_remaining):
-        self.buffer_capacity = 10
-        num_items = 2
-        first_frame = list(range(self.buffer_capacity))
-        self.assertLess(num_items, self.buffer_capacity)
-
-        self.upload_calls = 0
-        def uploader(frame):
-            self.upload_calls += 1
-            self.assertEqual(frame, first_frame[:num_items])
-            return mock.MagicMock(status_code=202)
-
-        self.timeout_calls = 0
-        def timeout(last_flush, interval):
-            self.timeout_calls += 1
-            # Until the last item has been retrieved from the pipe, the timeout
-            # length doesn't matter. After the last item has been retrieved,
-            # return a very small number so that the blocking get times out
-            if self.timeout_calls < num_items:
-                return 1000000
-            return 0
-        calculate_time_remaining.side_effect = timeout
-
-        pipe, _, fw = self._setup_worker(uploader)
-        for i in range(num_items):
-            pipe.put(first_frame[i], block=False)
-
-        fw.step()
-        self.assertEqual(self.upload_calls, 1)
-        self.assertEqual(self.timeout_calls, 2)
-
-    @mock.patch('logfire.flusher._calculate_time_remaining')
-    @mock.patch('logfire.flusher._initial_time_remaining')
-    def test_does_nothing_without_any_items(self, initial_time_remaining, calculate_time_remaining):
-        calculate_time_remaining.side_effect = lambda a,b: 0.0
-        initial_time_remaining.side_effect = lambda a: 0.0001
-
-        uploader = mock.MagicMock(side_effect=mock.MagicMock(status_code=202))
-        pipe, _, fw = self._setup_worker(uploader)
-
-        self.assertEqual(pipe.qsize(), 0)
-        fw.step()
-        self.assertFalse(uploader.called)
-
-    @mock.patch('logfire.flusher.time.sleep')
-    def test_retries_according_to_schedule(self, mock_sleep):
-        first_frame = list(range(self.buffer_capacity))
-
-        self.uploader_calls = 0
-        def uploader(frame):
-            self.uploader_calls += 1
-            self.assertEqual(frame, first_frame)
-            return mock.MagicMock(status_code=500)
-
-        self.sleep_calls = 0
-        def sleep(time):
-            self.assertEqual(time, RETRY_SCHEDULE[self.sleep_calls])
-            self.sleep_calls += 1
-        mock_sleep.side_effect = sleep
-
-        pipe, _, fw = self._setup_worker(uploader)
-
-        for log in first_frame:
-            pipe.put(log, block=False)
-
-        fw.step()
-        self.assertEqual(self.uploader_calls, len(RETRY_SCHEDULE) + 1)
-        self.assertEqual(self.sleep_calls, len(RETRY_SCHEDULE))
-
-    @mock.patch('logfire.flusher.sys.exit')
-    def test_shutdown_condition_empties_queue_and_calls_exit(self, mock_exit):
-        self.buffer_capacity = 10
-        num_items = 5
-        first_frame = list(range(self.buffer_capacity))
-        self.assertLess(num_items, self.buffer_capacity)
-
-        self.upload_calls = 0
-        def uploader(frame):
-            self.upload_calls += 1
-            self.assertEqual(frame, first_frame[:num_items])
-            return mock.MagicMock(status_code=202)
-
-        pipe, _, fw = self._setup_worker(uploader)
-        fw.parent_thread = mock.MagicMock(is_alive=lambda: False)
-
-        for i in range(num_items):
-            pipe.put(first_frame[i], block=False)
-
-        fw.step()
-        self.assertEqual(self.upload_calls, 1)
-        self.assertEqual(mock_exit.call_count, 1)
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+import mock
+import time
+import threading
+import unittest2
+
+from logfire.compat import queue
+from logfire.flusher import RETRY_SCHEDULE
+from logfire.flusher import FlushWorker
+from logfire.uploader import Uploader
+
+
+class TestFlushWorker(unittest2.TestCase):
+    host = 'https://in.logfire.ai'
+    source_token = 'dummy_source_token'
+    buffer_capacity = 5
+    flush_interval = 2
+
+    def _setup_worker(self, uploader=None):
+        pipe = queue.Queue(maxsize=self.buffer_capacity)
+        uploader = uploader or Uploader(self.source_token, self.host)
+        fw = FlushWorker(uploader, pipe, self.buffer_capacity, self.flush_interval)
+        return pipe, uploader, fw
+
+    def test_is_thread(self):
+        pipe, uploader, fw = self._setup_worker()
+        self.assertIsInstance(fw, threading.Thread)
+
+    def test_flushes_when_queue_is_full(self):
+        first_frame = list(range(self.buffer_capacity))
+        second_frame = list(range(self.buffer_capacity, self.buffer_capacity * 2))
+        self.calls = 0
+        self.flush_interval = 1000
+
+        def uploader(frame):
+            self.calls += 1
+            self.assertEqual(frame, first_frame)
+            return mock.MagicMock(status_code=202)
+
+        pipe, _, fw = self._setup_worker(uploader)
+
+        for log in first_frame:
+            pipe.put(log, block=False)
+
+        t1 = time.time()
+        fw.step()
+        t2 = time.time()
+        self.assertLess(t2 - t1, self.flush_interval)
+
+        self.assertEqual(self.calls, 1)
+
+    @mock.patch('logfire.flusher._calculate_time_remaining')
+    def test_flushes_after_interval(self, calculate_time_remaining):
+        self.buffer_capacity = 10
+        num_items = 2
+        first_frame = list(range(self.buffer_capacity))
+        self.assertLess(num_items, self.buffer_capacity)
+
+        self.upload_calls = 0
+        def uploader(frame):
+            self.upload_calls += 1
+            self.assertEqual(frame, first_frame[:num_items])
+            return mock.MagicMock(status_code=202)
+
+        self.timeout_calls = 0
+        def timeout(last_flush, interval):
+            self.timeout_calls += 1
+            # Until the last item has been retrieved from the pipe, the timeout
+            # length doesn't matter. After the last item has been retrieved,
+            # return a very small number so that the blocking get times out
+            if self.timeout_calls < num_items:
+                return 1000000
+            return 0
+        calculate_time_remaining.side_effect = timeout
+
+        pipe, _, fw = self._setup_worker(uploader)
+        for i in range(num_items):
+            pipe.put(first_frame[i], block=False)
+
+        fw.step()
+        self.assertEqual(self.upload_calls, 1)
+        self.assertEqual(self.timeout_calls, 2)
+
+    @mock.patch('logfire.flusher._calculate_time_remaining')
+    @mock.patch('logfire.flusher._initial_time_remaining')
+    def test_does_nothing_without_any_items(self, initial_time_remaining, calculate_time_remaining):
+        calculate_time_remaining.side_effect = lambda a,b: 0.0
+        initial_time_remaining.side_effect = lambda a: 0.0001
+
+        uploader = mock.MagicMock(side_effect=mock.MagicMock(status_code=202))
+        pipe, _, fw = self._setup_worker(uploader)
+
+        self.assertEqual(pipe.qsize(), 0)
+        fw.step()
+        self.assertFalse(uploader.called)
+
+    @mock.patch('logfire.flusher.time.sleep')
+    def test_retries_according_to_schedule(self, mock_sleep):
+        first_frame = list(range(self.buffer_capacity))
+
+        self.uploader_calls = 0
+        def uploader(frame):
+            self.uploader_calls += 1
+            self.assertEqual(frame, first_frame)
+            return mock.MagicMock(status_code=500)
+
+        self.sleep_calls = 0
+        def sleep(time):
+            self.assertEqual(time, RETRY_SCHEDULE[self.sleep_calls])
+            self.sleep_calls += 1
+        mock_sleep.side_effect = sleep
+
+        pipe, _, fw = self._setup_worker(uploader)
+
+        for log in first_frame:
+            pipe.put(log, block=False)
+
+        fw.step()
+        self.assertEqual(self.uploader_calls, len(RETRY_SCHEDULE) + 1)
+        self.assertEqual(self.sleep_calls, len(RETRY_SCHEDULE))
+
+    @mock.patch('logfire.flusher.sys.exit')
+    def test_shutdown_condition_empties_queue_and_calls_exit(self, mock_exit):
+        self.buffer_capacity = 10
+        num_items = 5
+        first_frame = list(range(self.buffer_capacity))
+        self.assertLess(num_items, self.buffer_capacity)
+
+        self.upload_calls = 0
+        def uploader(frame):
+            self.upload_calls += 1
+            self.assertEqual(frame, first_frame[:num_items])
+            return mock.MagicMock(status_code=202)
+
+        pipe, _, fw = self._setup_worker(uploader)
+        fw.parent_thread = mock.MagicMock(is_alive=lambda: False)
+
+        for i in range(num_items):
+            pipe.put(first_frame[i], block=False)
+
+        fw.step()
+        self.assertEqual(self.upload_calls, 1)
+        self.assertEqual(mock_exit.call_count, 1)
```

### Comparing `logfire-python-0.0.7/tests/test_formatter.py` & `logfire-python-0.0.8/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/tests/test_frame.py` & `logfire-python-0.0.8/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/tests/test_handler.py` & `logfire-python-0.0.8/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/tests/test_helpers.py` & `logfire-python-0.0.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.7/tests/test_uploader.py` & `logfire-python-0.0.8/tests/test_uploader.py`

 * *Files identical despite different names*

