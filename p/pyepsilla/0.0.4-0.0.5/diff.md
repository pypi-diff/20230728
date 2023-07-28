# Comparing `tmp/pyepsilla-0.0.4.tar.gz` & `tmp/pyepsilla-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.4.tar", last modified: Fri Jul 28 05:30:35 2023, max compression
+gzip compressed data, was "pyepsilla-0.0.5.tar", last modified: Fri Jul 28 07:21:10 2023, max compression
```

## Comparing `pyepsilla-0.0.4.tar` & `pyepsilla-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.687439 pyepsilla-0.0.4/
--rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.4/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.4/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 05:30:35.687307 pyepsilla-0.0.4/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.4/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.684699 pyepsilla-0.0.4/pyepsilla/
--rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.4/pyepsilla/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     1701 2023-07-28 05:28:46.000000 pyepsilla-0.0.4/pyepsilla/simple_example.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.686608 pyepsilla-0.0.4/pyepsilla/vectordb/
--rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.4/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     3885 2023-07-28 04:54:14.000000 pyepsilla-0.0.4/pyepsilla/vectordb/client.py
--rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.4/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.685835 pyepsilla-0.0.4/pyepsilla.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 05:30:35.687765 pyepsilla-0.0.4/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 05:30:13.000000 pyepsilla-0.0.4/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:21:10.928262 pyepsilla-0.0.5/
+-rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.5/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.5/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:21:10.928154 pyepsilla-0.0.5/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.5/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:21:10.926545 pyepsilla-0.0.5/pyepsilla/
+-rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.5/pyepsilla/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     1701 2023-07-28 05:28:46.000000 pyepsilla-0.0.5/pyepsilla/simple_example.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:21:10.927771 pyepsilla-0.0.5/pyepsilla/vectordb/
+-rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.5/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     4363 2023-07-28 07:19:32.000000 pyepsilla-0.0.5/pyepsilla/vectordb/client.py
+-rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.5/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:21:10.927262 pyepsilla-0.0.5/pyepsilla.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:21:10.000000 pyepsilla-0.0.5/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 07:21:10.000000 pyepsilla-0.0.5/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 07:21:10.000000 pyepsilla-0.0.5/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 07:21:10.000000 pyepsilla-0.0.5/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 07:21:10.000000 pyepsilla-0.0.5/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 07:21:10.928301 pyepsilla-0.0.5/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 07:20:04.000000 pyepsilla-0.0.5/setup.py
```

### Comparing `pyepsilla-0.0.4/LICENSE` & `pyepsilla-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.4/README.md` & `pyepsilla-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.4/pyepsilla/simple_example.py` & `pyepsilla-0.0.5/pyepsilla/simple_example.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.4/pyepsilla/vectordb/client.py` & `pyepsilla-0.0.5/pyepsilla/vectordb/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
-import json, requests
+import json, requests, socket
 
 class Client():
     def __init__(self, host='localhost', port='8888', db_name='default'):
         self._protocol = "http"
-        self._baseurl = "{}://{}:{}".format(self._protocol, host, port)
+        self._host = host
+        self._port = port
+        self._baseurl = "{}://{}:{}".format(self._protocol, self._host, self._port)
         self._db=db_name
-        self._timeout = 5
+        self._timeout = 10
         self._header = {'Content-type': 'application/json'}
         self._rs = requests.Session()
+        self.__check__()
 
     def __check__(self):
-
+        socket.setdefaulttimeout(self._timeout)
+        s = socket.socket(sock.AF_INET, sock.SOCK_STREAM)
+        check_result = s.connect_ex((self._host, self._port))
+        if check_result == 0:
+            print("{}:{} can be arrived!".format(self._host, self._port))
+        else:
+            print("{}:{} cann't be arrived!".format(self._host, self._port))
+        s.close()
 
     def welcome(self):
         req_url = "{}/".format(self._baseurl)
         req_data= None
         res = requests.get(url=req_url, data=json.dumps(req_data), headers=self._header, timeout=self._timeout)
         status_code = res.status_code
         body = res.text
```

### Comparing `pyepsilla-0.0.4/pyepsilla/vectordb/field.py` & `pyepsilla-0.0.5/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.4/setup.py` & `pyepsilla-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.4',
+    version= '0.0.5',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
```

