# Comparing `tmp/oapi2mockserver-0.0.8.tar.gz` & `tmp/oapi2mockserver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oapi2mockserver-0.0.8.tar", last modified: Mon Sep  2 12:41:27 2019, max compression
+gzip compressed data, was "dist/oapi2mockserver-0.0.9.tar", last modified: Tue Sep  3 11:19:32 2019, max compression
```

## Comparing `oapi2mockserver-0.0.8.tar` & `oapi2mockserver-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 markus.baumann   (502) staff       (20)        0 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/
--rw-r--r--   0 markus.baumann   (502) staff       (20)      466 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/PKG-INFO
--rw-r--r--   0 markus.baumann   (502) staff       (20)        0 2019-08-26 14:36:09.000000 oapi2mockserver-0.0.8/README.md
-drwxr-xr-x   0 markus.baumann   (502) staff       (20)        0 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/
--rw-r--r--   0 markus.baumann   (502) staff       (20)        0 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/__init__.py
--rw-r--r--   0 markus.baumann   (502) staff       (20)     6979 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/converter.py
--rw-r--r--   0 markus.baumann   (502) staff       (20)     2279 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/expectation.py
--rw-r--r--   0 markus.baumann   (502) staff       (20)     1677 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/main.py
--rw-r--r--   0 markus.baumann   (502) staff       (20)     1259 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/open_api_schema.py
--rw-r--r--   0 markus.baumann   (502) staff       (20)     1502 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/requester.py
--rw-r--r--   0 markus.baumann   (502) staff       (20)      831 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver/scenario.py
-drwxr-xr-x   0 markus.baumann   (502) staff       (20)        0 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/
--rw-r--r--   0 markus.baumann   (502) staff       (20)      466 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/PKG-INFO
--rw-r--r--   0 markus.baumann   (502) staff       (20)      458 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/SOURCES.txt
--rw-r--r--   0 markus.baumann   (502) staff       (20)        1 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/dependency_links.txt
--rw-r--r--   0 markus.baumann   (502) staff       (20)       63 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/entry_points.txt
--rw-r--r--   0 markus.baumann   (502) staff       (20)       63 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/requires.txt
--rw-r--r--   0 markus.baumann   (502) staff       (20)       16 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/oapi2mockserver.egg-info/top_level.txt
--rw-r--r--   0 markus.baumann   (502) staff       (20)       38 2019-09-02 12:41:27.000000 oapi2mockserver-0.0.8/setup.cfg
--rw-r--r--   0 markus.baumann   (502) staff       (20)     1408 2019-09-02 12:39:29.000000 oapi2mockserver-0.0.8/setup.py
+drwxr-xr-x   0 markus.baumann   (502) staff       (20)        0 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/
+-rw-r--r--   0 markus.baumann   (502) staff       (20)      466 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/PKG-INFO
+-rw-r--r--   0 markus.baumann   (502) staff       (20)        0 2019-08-26 14:36:09.000000 oapi2mockserver-0.0.9/README.md
+drwxr-xr-x   0 markus.baumann   (502) staff       (20)        0 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver/
+-rw-r--r--   0 markus.baumann   (502) staff       (20)        0 2019-09-03 09:10:51.000000 oapi2mockserver-0.0.9/oapi2mockserver/__init__.py
+-rw-r--r--   0 markus.baumann   (502) staff       (20)     1633 2019-09-03 11:17:57.000000 oapi2mockserver-0.0.9/oapi2mockserver/cli_entrypoint.py
+-rw-r--r--   0 markus.baumann   (502) staff       (20)     6980 2019-09-03 11:17:57.000000 oapi2mockserver-0.0.9/oapi2mockserver/converter.py
+-rw-r--r--   0 markus.baumann   (502) staff       (20)     2279 2019-09-03 09:10:51.000000 oapi2mockserver-0.0.9/oapi2mockserver/expectation.py
+-rw-r--r--   0 markus.baumann   (502) staff       (20)     1259 2019-09-03 09:10:51.000000 oapi2mockserver-0.0.9/oapi2mockserver/open_api_schema.py
+-rw-r--r--   0 markus.baumann   (502) staff       (20)     1502 2019-09-02 12:41:31.000000 oapi2mockserver-0.0.9/oapi2mockserver/requester.py
+-rw-r--r--   0 markus.baumann   (502) staff       (20)      831 2019-09-03 10:23:35.000000 oapi2mockserver-0.0.9/oapi2mockserver/scenario.py
+drwxr-xr-x   0 markus.baumann   (502) staff       (20)        0 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/
+-rw-r--r--   0 markus.baumann   (502) staff       (20)      466 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/PKG-INFO
+-rw-r--r--   0 markus.baumann   (502) staff       (20)      468 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/SOURCES.txt
+-rw-r--r--   0 markus.baumann   (502) staff       (20)        1 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/dependency_links.txt
+-rw-r--r--   0 markus.baumann   (502) staff       (20)       73 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/entry_points.txt
+-rw-r--r--   0 markus.baumann   (502) staff       (20)       63 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/requires.txt
+-rw-r--r--   0 markus.baumann   (502) staff       (20)       16 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/oapi2mockserver.egg-info/top_level.txt
+-rw-r--r--   0 markus.baumann   (502) staff       (20)       38 2019-09-03 11:19:32.000000 oapi2mockserver-0.0.9/setup.cfg
+-rw-r--r--   0 markus.baumann   (502) staff       (20)     1405 2019-09-03 11:19:24.000000 oapi2mockserver-0.0.9/setup.py
```

### Comparing `oapi2mockserver-0.0.8/oapi2mockserver/converter.py` & `oapi2mockserver-0.0.9/oapi2mockserver/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
-from . import expectation
 
-from open_api_schema import OpenAPISchema
-from scenario import Scenario
+from .expectation import Expectation
+from .open_api_schema import OpenAPISchema
+from .scenario import Scenario
 
 
 class Converter(object):
 
 	def __init__(self):
 		self.scenarios = ''
 		self.spec = {}
@@ -128,15 +128,15 @@
 	def create_expectation(self):
 		if self.currentPath is None or 'operation' not in self.currentOperation or 'statusCode' not in self.currentStatusCode:
 			return False
 
 		request_content_types = []
 		response_content_types = []
 
-		e = expectation.Expectation()
+		e = Expectation()
 		e.set_path(self.currentPath)
 		e.set_method(self.currentOperation['operation'])
 		e.set_status_code(self.currentStatusCode['statusCode'])
 
 		#if 'schema' in self.currentStatusCode:
 		#	e.set_request_schema(self.currentStatusCode['schema'])
```

### Comparing `oapi2mockserver-0.0.8/oapi2mockserver/expectation.py` & `oapi2mockserver-0.0.9/oapi2mockserver/expectation.py`

 * *Files identical despite different names*

### Comparing `oapi2mockserver-0.0.8/oapi2mockserver/main.py` & `oapi2mockserver-0.0.9/oapi2mockserver/cli_entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-#!/usr/bin/python
+#!/usr/bin/python3
 
 import argparse
-import sys
 import prance
-import json
 import os
-from . import expectation
+
 from . import requester
 from . import converter
 
 def parse_yaml(filepath):
 	exists = os.path.isfile(filepath)
 	if not exists:
 		print(filepath + ' does not exist')
@@ -65,12 +63,14 @@
 	parser_reset = subparsers.add_parser('reset')
 	parser_reset.set_defaults(func=reset)
 	parser_reset.add_argument('mockserver_uri')
 
 	args = parser.parse_args()
 	args.func(args)
 
+
 def main():
 	arguments()
 
+
 if __name__ == '__main__':
-	main()
+	main()
```

### Comparing `oapi2mockserver-0.0.8/oapi2mockserver/open_api_schema.py` & `oapi2mockserver-0.0.9/oapi2mockserver/open_api_schema.py`

 * *Files identical despite different names*

### Comparing `oapi2mockserver-0.0.8/oapi2mockserver/requester.py` & `oapi2mockserver-0.0.9/oapi2mockserver/requester.py`

 * *Files identical despite different names*

### Comparing `oapi2mockserver-0.0.8/oapi2mockserver/scenario.py` & `oapi2mockserver-0.0.9/oapi2mockserver/scenario.py`

 * *Files identical despite different names*

### Comparing `oapi2mockserver-0.0.8/setup.py` & `oapi2mockserver-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # load subpackages which are provided to other users for import statements
 with open("provides.txt", "r") as provide:
     provides = provide.read()
 
 setuptools.setup(
     name="oapi2mockserver",
-    version="0.0.8",
+    version="0.0.9",
     author="allmyhomes GmbH",
     author_email="opensource@allmyhomes.com",
     description="Provides the basic setup of an API mockserver.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -31,11 +31,11 @@
     install_requires=requirements,
     # package_data={'': ['<none_python_file_name>']},         # list all non python files
     # install_package_data=True,                              # installs non python files
     provides=[provides],                                      # usable by other users
 
     entry_points={
         "console_scripts": [                                  # create custom shell commands
-            "oapi2mockserver = oapi2mockserver.main:main"             
+            "oapi2mockserver = oapi2mockserver.cli_entrypoint:main"
         ]
     }
 )
```

