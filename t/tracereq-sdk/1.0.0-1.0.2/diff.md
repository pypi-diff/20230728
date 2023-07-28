# Comparing `tmp/tracereq-sdk-1.0.0.tar.gz` & `tmp/tracereq-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracereq-sdk-1.0.0.tar", last modified: Sun Jul 23 17:30:32 2023, max compression
+gzip compressed data, was "tracereq-sdk-1.0.2.tar", last modified: Fri Jul 28 12:44:32 2023, max compression
```

## Comparing `tracereq-sdk-1.0.0.tar` & `tracereq-sdk-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-23 17:30:32.368769 tracereq-sdk-1.0.0/
--rw-r--r--   0 psachan2   (501) staff       (20)     1064 2023-07-23 16:57:47.000000 tracereq-sdk-1.0.0/LICENSE
--rw-r--r--   0 psachan2   (501) staff       (20)     2214 2023-07-23 17:30:32.368595 tracereq-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 psachan2   (501) staff       (20)      468 2023-07-23 16:39:53.000000 tracereq-sdk-1.0.0/README.md
--rw-r--r--   0 psachan2   (501) staff       (20)     1213 2023-07-23 17:27:27.000000 tracereq-sdk-1.0.0/pyproject.toml
--rw-r--r--   0 psachan2   (501) staff       (20)       38 2023-07-23 17:30:32.368807 tracereq-sdk-1.0.0/setup.cfg
-drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-23 17:30:32.365778 tracereq-sdk-1.0.0/tracereq/
--rw-r--r--   0 psachan2   (501) staff       (20)       54 2023-07-23 17:17:14.000000 tracereq-sdk-1.0.0/tracereq/__init__.py
--rw-r--r--   0 psachan2   (501) staff       (20)      358 2023-07-23 17:18:41.000000 tracereq-sdk-1.0.0/tracereq/api.py
--rw-r--r--   0 psachan2   (501) staff       (20)      787 2023-07-23 16:45:14.000000 tracereq-sdk-1.0.0/tracereq/client.py
--rw-r--r--   0 psachan2   (501) staff       (20)      211 2023-07-21 18:11:38.000000 tracereq-sdk-1.0.0/tracereq/constants.py
--rw-r--r--   0 psachan2   (501) staff       (20)     2167 2023-07-23 17:18:50.000000 tracereq-sdk-1.0.0/tracereq/customlib.py
--rw-r--r--   0 psachan2   (501) staff       (20)     1428 2023-07-21 18:11:38.000000 tracereq-sdk-1.0.0/tracereq/engine.py
-drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-23 17:30:32.366647 tracereq-sdk-1.0.0/tracereq/integrations/
--rw-r--r--   0 psachan2   (501) staff       (20)     1355 2023-07-23 17:20:20.000000 tracereq-sdk-1.0.0/tracereq/integrations/__init__.py
--rw-r--r--   0 psachan2   (501) staff       (20)     1428 2023-07-23 17:20:09.000000 tracereq-sdk-1.0.0/tracereq/integrations/flasklib.py
--rw-r--r--   0 psachan2   (501) staff       (20)     4636 2023-07-21 18:11:38.000000 tracereq-sdk-1.0.0/tracereq/tracing.py
--rw-r--r--   0 psachan2   (501) staff       (20)     1400 2023-07-23 16:33:47.000000 tracereq-sdk-1.0.0/tracereq/transport.py
-drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-23 17:30:32.368250 tracereq-sdk-1.0.0/tracereq_sdk.egg-info/
--rw-r--r--   0 psachan2   (501) staff       (20)     2214 2023-07-23 17:30:32.000000 tracereq-sdk-1.0.0/tracereq_sdk.egg-info/PKG-INFO
--rw-r--r--   0 psachan2   (501) staff       (20)      440 2023-07-23 17:30:32.000000 tracereq-sdk-1.0.0/tracereq_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 psachan2   (501) staff       (20)        1 2023-07-23 17:30:32.000000 tracereq-sdk-1.0.0/tracereq_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 psachan2   (501) staff       (20)       62 2023-07-23 17:30:32.000000 tracereq-sdk-1.0.0/tracereq_sdk.egg-info/requires.txt
--rw-r--r--   0 psachan2   (501) staff       (20)        9 2023-07-23 17:30:32.000000 tracereq-sdk-1.0.0/tracereq_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-28 12:44:32.170677 tracereq-sdk-1.0.2/
+-rw-r--r--   0 psachan2   (501) staff       (20)     1064 2023-07-23 17:43:36.000000 tracereq-sdk-1.0.2/LICENSE
+-rw-r--r--   0 psachan2   (501) staff       (20)     2345 2023-07-28 12:44:32.170474 tracereq-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 psachan2   (501) staff       (20)      599 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/README.md
+-rw-r--r--   0 psachan2   (501) staff       (20)     1167 2023-07-28 12:43:26.000000 tracereq-sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 psachan2   (501) staff       (20)       38 2023-07-28 12:44:32.170734 tracereq-sdk-1.0.2/setup.cfg
+drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-28 12:44:32.168260 tracereq-sdk-1.0.2/tracereq_sdk/
+-rw-r--r--   0 psachan2   (501) staff       (20)       81 2023-07-28 12:43:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/__init__.py
+-rw-r--r--   0 psachan2   (501) staff       (20)      363 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/api.py
+-rw-r--r--   0 psachan2   (501) staff       (20)      787 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/client.py
+-rw-r--r--   0 psachan2   (501) staff       (20)      211 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/constants.py
+-rw-r--r--   0 psachan2   (501) staff       (20)     2167 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/customlib.py
+-rw-r--r--   0 psachan2   (501) staff       (20)     1428 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/engine.py
+drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-28 12:44:32.170164 tracereq-sdk-1.0.2/tracereq_sdk/integrations/
+-rw-r--r--   0 psachan2   (501) staff       (20)     1359 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/integrations/__init__.py
+-rw-r--r--   0 psachan2   (501) staff       (20)     1436 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/integrations/flasklib.py
+-rw-r--r--   0 psachan2   (501) staff       (20)     4636 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/tracing.py
+-rw-r--r--   0 psachan2   (501) staff       (20)     1400 2023-07-28 12:41:26.000000 tracereq-sdk-1.0.2/tracereq_sdk/transport.py
+drwxr-xr-x   0 psachan2   (501) staff       (20)        0 2023-07-28 12:44:32.169521 tracereq-sdk-1.0.2/tracereq_sdk.egg-info/
+-rw-r--r--   0 psachan2   (501) staff       (20)     2345 2023-07-28 12:44:32.000000 tracereq-sdk-1.0.2/tracereq_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 psachan2   (501) staff       (20)      480 2023-07-28 12:44:32.000000 tracereq-sdk-1.0.2/tracereq_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 psachan2   (501) staff       (20)        1 2023-07-28 12:44:32.000000 tracereq-sdk-1.0.2/tracereq_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 psachan2   (501) staff       (20)       62 2023-07-28 12:44:32.000000 tracereq-sdk-1.0.2/tracereq_sdk.egg-info/requires.txt
+-rw-r--r--   0 psachan2   (501) staff       (20)       13 2023-07-28 12:44:32.000000 tracereq-sdk-1.0.2/tracereq_sdk.egg-info/top_level.txt
```

### Comparing `tracereq-sdk-1.0.0/LICENSE` & `tracereq-sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tracereq-sdk-1.0.0/PKG-INFO` & `tracereq-sdk-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracereq-sdk
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python client for TraceReq (https://tracereq.com)
 Author-email: Prateek Sachan <ps@prateeksachan.com>
 License: MIT License
         
         Copyright (c) 2023 TraceReq
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,31 +32,33 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TraceReq SDK for Python
 
+[![PyPi page link -- version](https://img.shields.io/pypi/v/tracereq-sdk.svg)](https://pypi.python.org/pypi/tracereq-sdk)
+
 This is the Python SDK for [TraceReq](http://tracereq.com/)
 
 ---
 
 ## Installation
 
 ```bash
 pip install --upgrade tracereq-sdk
 ```
 
 ## Usage with Flask
 
 ```python
-import tracereq
+import tracereq_sdk
 
 app = Flask(__name__)
-tracereq.init(api_key='xxx-xxx',
+tracereq_sdk.init(api_key='xxx-xxx',
     flask_app=app.wsgi_app
 )
 ```
 
 Adding the above any flask service will start tracing requests.
 No other additional code is required.
```

### Comparing `tracereq-sdk-1.0.0/pyproject.toml` & `tracereq-sdk-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tracereq-sdk"
-version = "1.0.0"
+version = "1.0.2"
 description = "Python client for TraceReq (https://tracereq.com)"
 readme = "README.md"
 authors = [
     { name = "Prateek Sachan", email = "ps@prateeksachan.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -27,29 +27,22 @@
 [project.optional-dependencies]
 dev = ["pip-tools"]
 
 [project.urls]
 Homepage = "https://github.com/tracereq/python-tracereq-sdk"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
+    'version = "{version}"',
 ]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
-]
-
+"tracereq_sdk/__init__.py" = ["{version}"]
```

### Comparing `tracereq-sdk-1.0.0/tracereq/client.py` & `tracereq-sdk-1.0.2/tracereq_sdk/client.py`

 * *Files identical despite different names*

### Comparing `tracereq-sdk-1.0.0/tracereq/customlib.py` & `tracereq-sdk-1.0.2/tracereq_sdk/customlib.py`

 * *Files identical despite different names*

### Comparing `tracereq-sdk-1.0.0/tracereq/engine.py` & `tracereq-sdk-1.0.2/tracereq_sdk/engine.py`

 * *Files identical despite different names*

### Comparing `tracereq-sdk-1.0.0/tracereq/integrations/__init__.py` & `tracereq-sdk-1.0.2/tracereq_sdk/integrations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from threading import Lock
 
 _installer_lock = Lock()
 _installed_integrations = {}
 
 
 def get_core_integrations():
-    from tracereq.customlib import CustomlibIntegration
+    from tracereq_sdk.customlib import CustomlibIntegration
     yield CustomlibIntegration()
 
 
 def get_custom_integrations(**kwargs):
     if kwargs.get('flask_app'):
         from .flasklib import FlasklibIntegration
         yield FlasklibIntegration(kwargs.get('flask_app'))
```

### Comparing `tracereq-sdk-1.0.0/tracereq/integrations/flasklib.py` & `tracereq-sdk-1.0.2/tracereq_sdk/integrations/flasklib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from flask import Flask, _request_ctx_stack
 from flask.signals import request_started, request_finished
 from . import Integration
-from tracereq.engine import Engine
-from tracereq.tracing import generate_trace_event, Trace, generalize_request
+from tracereq_sdk.engine import Engine
+from tracereq_sdk.tracing import generate_trace_event, Trace, generalize_request
 
 
 class FlasklibIntegration(Integration):
     integration_key = "flasklib"
 
     def install(self):
         request_started.connect(_request_started)
```

### Comparing `tracereq-sdk-1.0.0/tracereq/tracing.py` & `tracereq-sdk-1.0.2/tracereq_sdk/tracing.py`

 * *Files identical despite different names*

### Comparing `tracereq-sdk-1.0.0/tracereq/transport.py` & `tracereq-sdk-1.0.2/tracereq_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `tracereq-sdk-1.0.0/tracereq_sdk.egg-info/PKG-INFO` & `tracereq-sdk-1.0.2/tracereq_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracereq-sdk
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python client for TraceReq (https://tracereq.com)
 Author-email: Prateek Sachan <ps@prateeksachan.com>
 License: MIT License
         
         Copyright (c) 2023 TraceReq
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,31 +32,33 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TraceReq SDK for Python
 
+[![PyPi page link -- version](https://img.shields.io/pypi/v/tracereq-sdk.svg)](https://pypi.python.org/pypi/tracereq-sdk)
+
 This is the Python SDK for [TraceReq](http://tracereq.com/)
 
 ---
 
 ## Installation
 
 ```bash
 pip install --upgrade tracereq-sdk
 ```
 
 ## Usage with Flask
 
 ```python
-import tracereq
+import tracereq_sdk
 
 app = Flask(__name__)
-tracereq.init(api_key='xxx-xxx',
+tracereq_sdk.init(api_key='xxx-xxx',
     flask_app=app.wsgi_app
 )
 ```
 
 Adding the above any flask service will start tracing requests.
 No other additional code is required.
```

