# Comparing `tmp/vsure-2.6.2.tar.gz` & `tmp/vsure-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsure-2.6.2.tar", last modified: Mon Jun 26 08:15:38 2023, max compression
+gzip compressed data, was "vsure-2.6.3.tar", last modified: Fri Jul 28 07:00:41 2023, max compression
```

## Comparing `vsure-2.6.2.tar` & `vsure-2.6.3.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/
--rw-rw-r--   0 per       (1000) per       (1000)     1082 2020-06-25 19:31:35.000000 vsure-2.6.2/LICENSE
--rw-rw-r--   0 per       (1000) per       (1000)       16 2020-10-28 18:46:19.000000 vsure-2.6.2/MANIFEST.in
--rw-rw-r--   0 per       (1000) per       (1000)      739 2023-06-26 08:15:38.866215 vsure-2.6.2/PKG-INFO
--rw-rw-r--   0 per       (1000) per       (1000)     7436 2023-06-26 08:14:50.000000 vsure-2.6.2/README.md
--rw-rw-r--   0 per       (1000) per       (1000)       38 2023-06-26 08:15:38.866215 vsure-2.6.2/setup.cfg
--rw-rw-r--   0 per       (1000) per       (1000)     1095 2023-06-26 08:14:50.000000 vsure-2.6.2/setup.py
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/test/
--rw-rw-r--   0 per       (1000) per       (1000)     1672 2022-09-10 14:24:33.000000 vsure-2.6.2/test/test_base_url_func.py
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/verisure/
--rw-rw-r--   0 per       (1000) per       (1000)      480 2023-06-26 08:14:45.000000 vsure-2.6.2/verisure/__init__.py
--rw-rw-r--   0 per       (1000) per       (1000)     4639 2023-06-26 08:14:45.000000 vsure-2.6.2/verisure/__main__.py
--rw-rw-r--   0 per       (1000) per       (1000)    34464 2023-06-26 08:14:50.000000 vsure-2.6.2/verisure/session.py
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/vsure.egg-info/
--rw-r--r--   0 per       (1000) per       (1000)      739 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/PKG-INFO
--rw-r--r--   0 per       (1000) per       (1000)      327 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/SOURCES.txt
--rw-r--r--   0 per       (1000) per       (1000)        1 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/dependency_links.txt
--rw-r--r--   0 per       (1000) per       (1000)       67 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/entry_points.txt
--rw-r--r--   0 per       (1000) per       (1000)       32 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/requires.txt
--rw-r--r--   0 per       (1000) per       (1000)        9 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/top_level.txt
--rw-r--r--   0 per       (1000) per       (1000)        1 2020-06-25 19:36:24.000000 vsure-2.6.2/vsure.egg-info/zip-safe
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-07-28 07:00:41.123849 vsure-2.6.3/
+-rw-rw-r--   0 per       (1000) per       (1000)     1082 2023-07-25 20:15:47.000000 vsure-2.6.3/LICENSE
+-rw-rw-r--   0 per       (1000) per       (1000)       16 2023-07-25 20:15:47.000000 vsure-2.6.3/MANIFEST.in
+-rw-rw-r--   0 per       (1000) per       (1000)      720 2023-07-28 07:00:41.123849 vsure-2.6.3/PKG-INFO
+-rw-rw-r--   0 per       (1000) per       (1000)     7472 2023-07-28 07:00:28.000000 vsure-2.6.3/README.md
+-rw-rw-r--   0 per       (1000) per       (1000)       38 2023-07-28 07:00:41.123849 vsure-2.6.3/setup.cfg
+-rw-rw-r--   0 per       (1000) per       (1000)     1095 2023-07-28 07:00:28.000000 vsure-2.6.3/setup.py
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-07-28 07:00:41.123849 vsure-2.6.3/verisure/
+-rw-rw-r--   0 per       (1000) per       (1000)      480 2023-07-25 20:15:47.000000 vsure-2.6.3/verisure/__init__.py
+-rw-rw-r--   0 per       (1000) per       (1000)     4639 2023-07-25 20:15:47.000000 vsure-2.6.3/verisure/__main__.py
+-rw-rw-r--   0 per       (1000) per       (1000)    34653 2023-07-28 07:00:28.000000 vsure-2.6.3/verisure/session.py
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-07-28 07:00:41.123849 vsure-2.6.3/vsure.egg-info/
+-rw-rw-r--   0 per       (1000) per       (1000)      720 2023-07-28 07:00:41.000000 vsure-2.6.3/vsure.egg-info/PKG-INFO
+-rw-rw-r--   0 per       (1000) per       (1000)      300 2023-07-28 07:00:41.000000 vsure-2.6.3/vsure.egg-info/SOURCES.txt
+-rw-rw-r--   0 per       (1000) per       (1000)        1 2023-07-28 07:00:41.000000 vsure-2.6.3/vsure.egg-info/dependency_links.txt
+-rw-rw-r--   0 per       (1000) per       (1000)       48 2023-07-28 07:00:41.000000 vsure-2.6.3/vsure.egg-info/entry_points.txt
+-rw-rw-r--   0 per       (1000) per       (1000)       32 2023-07-28 07:00:41.000000 vsure-2.6.3/vsure.egg-info/requires.txt
+-rw-rw-r--   0 per       (1000) per       (1000)        9 2023-07-28 07:00:41.000000 vsure-2.6.3/vsure.egg-info/top_level.txt
+-rw-rw-r--   0 per       (1000) per       (1000)        1 2023-07-25 20:29:54.000000 vsure-2.6.3/vsure.egg-info/zip-safe
```

### Comparing `vsure-2.6.2/LICENSE` & `vsure-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vsure-2.6.2/PKG-INFO` & `vsure-2.6.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: vsure
-Version: 2.6.2
+Version: 2.6.3
 Summary: Read and change status of verisure devices through mypages.
 Home-page: http://github.com/persandstrom/python-verisure
 Author: Per Sandstrom
 Author-email: per.j.sandstrom@gmail.com
 License: MIT
 Keywords: home automation verisure
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE
 
 A python3 module for reading and changing status of verisure devices through mypages.
-
```

### Comparing `vsure-2.6.2/README.md` & `vsure-2.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This software is not affiliated with Verisure Holding AB and the developers take no
 legal responsibility for the functionality or security of your Verisure Alarms and
 devices.
 
 ## Version History
 
 ```txt
+2.6.3 Differentiate response errors
 2.6.2 Fix request wrapper
 2.6.1 Move to automation subdomain
 2.6.0 Add Get Firmware Version
 2.5.6 Fix docstring, cookie lasts 15 minutes
 2.5.5 Solved bug during response error except using CLI
 2.5.4 Add possibility to set giid to all queries, refactoring and resolve lint warnings
 2.5.3 Refactor login
```

### Comparing `vsure-2.6.2/setup.py` & `vsure-2.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Setup for python-verisure """
 
 from setuptools import setup
 
 setup(
     name='vsure',
-    version='2.6.2',
+    version='2.6.3',
     description='Read and change status of verisure devices through mypages.',
     long_description='A python3 module for reading and changing status of '
     + 'verisure devices through mypages.',
     url='http://github.com/persandstrom/python-verisure',
     author='Per Sandstrom',
     author_email='per.j.sandstrom@gmail.com',
     license='MIT',
```

### Comparing `vsure-2.6.2/verisure/__main__.py` & `vsure-2.6.3/verisure/__main__.py`

 * *Files identical despite different names*

### Comparing `vsure-2.6.2/verisure/session.py` & `vsure-2.6.3/verisure/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 Verisure session, using verisure app api
 '''
 
 import json
 import os
 import pickle
+
 import requests
 
 
 class Error(Exception):
     ''' Verisure session error '''
 
 
@@ -96,24 +97,27 @@
 
         def wrapper(url, *args, **kwargs):
             last_exception = Error("Unknown error")
             base_urls = self._base_urls.copy()
             for base_url in base_urls:
                 try:
                     response = function(base_url+url, *args, **kwargs)
+                    if response.status_code >= 500:
+                        last_exception = ResponseError(response.status_code, response.text)
+                        self._base_urls.reverse()
+                        continue
+                    if response.status_code >= 400:
+                        last_exception = LoginError(response.text)
+                        break
                     if response.status_code == 200:
-                        if "SYS_00004" in response.text:
-                            self._base_urls.reverse()
-                            continue
                         return response
-                    response.raise_for_status()
                 except requests.exceptions.RequestException as ex:
-                    last_exception = ex
+                    last_exception = RequestError(str(ex))
                 self._base_urls.reverse()
-            raise Error from last_exception
+            raise last_exception
         return wrapper
 
 
     def login(self):
         """ Login to verisure app api
         Login before calling any read or write commands
         Return installations
```

### Comparing `vsure-2.6.2/vsure.egg-info/PKG-INFO` & `vsure-2.6.3/vsure.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: vsure
-Version: 2.6.2
+Version: 2.6.3
 Summary: Read and change status of verisure devices through mypages.
 Home-page: http://github.com/persandstrom/python-verisure
 Author: Per Sandstrom
 Author-email: per.j.sandstrom@gmail.com
 License: MIT
 Keywords: home automation verisure
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE
 
 A python3 module for reading and changing status of verisure devices through mypages.
-
```

