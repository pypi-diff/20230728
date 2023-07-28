# Comparing `tmp/pyepsilla-0.0.6.tar.gz` & `tmp/pyepsilla-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.6.tar", last modified: Fri Jul 28 07:25:31 2023, max compression
+gzip compressed data, was "pyepsilla-0.0.7.tar", last modified: Fri Jul 28 07:28:26 2023, max compression
```

## Comparing `pyepsilla-0.0.6.tar` & `pyepsilla-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:25:31.543681 pyepsilla-0.0.6/
--rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.6/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.6/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:25:31.543571 pyepsilla-0.0.6/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.6/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:25:31.542308 pyepsilla-0.0.6/pyepsilla/
--rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.6/pyepsilla/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     1797 2023-07-28 07:24:52.000000 pyepsilla-0.0.6/pyepsilla/simple_example.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:25:31.543188 pyepsilla-0.0.6/pyepsilla/vectordb/
--rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.6/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     4329 2023-07-28 07:23:32.000000 pyepsilla-0.0.6/pyepsilla/vectordb/client.py
--rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.6/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:25:31.542810 pyepsilla-0.0.6/pyepsilla.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:25:31.000000 pyepsilla-0.0.6/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 07:25:31.000000 pyepsilla-0.0.6/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 07:25:31.000000 pyepsilla-0.0.6/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 07:25:31.000000 pyepsilla-0.0.6/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 07:25:31.000000 pyepsilla-0.0.6/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 07:25:31.543724 pyepsilla-0.0.6/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 07:23:25.000000 pyepsilla-0.0.6/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.486561 pyepsilla-0.0.7/
+-rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.7/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.7/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:28:26.486338 pyepsilla-0.0.7/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.7/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.484431 pyepsilla-0.0.7/pyepsilla/
+-rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.7/pyepsilla/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     1797 2023-07-28 07:24:52.000000 pyepsilla-0.0.7/pyepsilla/simple_example.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.485844 pyepsilla-0.0.7/pyepsilla/vectordb/
+-rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.7/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     4334 2023-07-28 07:27:52.000000 pyepsilla-0.0.7/pyepsilla/vectordb/client.py
+-rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.7/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.485245 pyepsilla-0.0.7/pyepsilla.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 07:28:26.486625 pyepsilla-0.0.7/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 07:28:01.000000 pyepsilla-0.0.7/setup.py
```

### Comparing `pyepsilla-0.0.6/LICENSE` & `pyepsilla-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.6/README.md` & `pyepsilla-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.6/pyepsilla/simple_example.py` & `pyepsilla-0.0.7/pyepsilla/simple_example.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.6/pyepsilla/vectordb/client.py` & `pyepsilla-0.0.7/pyepsilla/vectordb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._timeout = 10
         self._header = {'Content-type': 'application/json'}
         self.__check__()
 
     def __check__(self):
         socket.setdefaulttimeout(self._timeout)
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        check_result = s.connect_ex((self._host, self._port))
+        check_result = s.connect_ex((self._host, int(self._port)))
         if check_result == 0:
             print("{}:{} can be arrived!".format(self._host, self._port))
         else:
             print("{}:{} cann't be arrived!".format(self._host, self._port))
         s.close()
 
     def welcome(self):
@@ -32,15 +32,15 @@
         body = res.text
         print("Return:", body)
         return status_code, body
 
     def state(self):
         req_url = "{}/state".format(self._baseurl)
         req_data= None
-        res = self._rs.get(url=req_url, data=json.dumps(req_data), headers=self._header)
+        res = requests.get(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
     def use_db(self, db_name):
         self._db = db_name
```

### Comparing `pyepsilla-0.0.6/pyepsilla/vectordb/field.py` & `pyepsilla-0.0.7/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.6/setup.py` & `pyepsilla-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.6',
+    version= '0.0.7',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
```

