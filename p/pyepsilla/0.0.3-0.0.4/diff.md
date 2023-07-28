# Comparing `tmp/pyepsilla-0.0.3.tar.gz` & `tmp/pyepsilla-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.3.tar", last modified: Thu Jul 27 17:13:44 2023, max compression
+gzip compressed data, was "pyepsilla-0.0.4.tar", last modified: Fri Jul 28 05:30:35 2023, max compression
```

## Comparing `pyepsilla-0.0.3.tar` & `pyepsilla-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.140181 pyepsilla-0.0.3/
--rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.3/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.3/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-27 17:13:44.140076 pyepsilla-0.0.3/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      357 2023-07-24 17:07:13.000000 pyepsilla-0.0.3/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.138213 pyepsilla-0.0.3/pyepsilla/
--rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.3/pyepsilla/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     1422 2023-07-27 17:08:27.000000 pyepsilla-0.0.3/pyepsilla/simple_example.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.139725 pyepsilla-0.0.3/pyepsilla/vectordb/
--rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.3/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     3902 2023-07-27 17:06:13.000000 pyepsilla-0.0.3/pyepsilla/vectordb/client.py
--rw-r--r--   0 eric       (501) staff       (20)      410 2023-07-27 17:05:39.000000 pyepsilla-0.0.3/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.139154 pyepsilla-0.0.3/pyepsilla.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-27 17:13:44.140215 pyepsilla-0.0.3/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-27 17:11:49.000000 pyepsilla-0.0.3/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.687439 pyepsilla-0.0.4/
+-rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.4/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.4/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 05:30:35.687307 pyepsilla-0.0.4/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.4/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.684699 pyepsilla-0.0.4/pyepsilla/
+-rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.4/pyepsilla/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     1701 2023-07-28 05:28:46.000000 pyepsilla-0.0.4/pyepsilla/simple_example.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.686608 pyepsilla-0.0.4/pyepsilla/vectordb/
+-rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.4/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     3885 2023-07-28 04:54:14.000000 pyepsilla-0.0.4/pyepsilla/vectordb/client.py
+-rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.4/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 05:30:35.685835 pyepsilla-0.0.4/pyepsilla.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 05:30:35.000000 pyepsilla-0.0.4/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 05:30:35.687765 pyepsilla-0.0.4/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 05:30:13.000000 pyepsilla-0.0.4/setup.py
```

### Comparing `pyepsilla-0.0.3/LICENSE` & `pyepsilla-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.3/pyepsilla/simple_example.py` & `pyepsilla-0.0.4/pyepsilla/simple_example.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
+#
+# 1.
+# 2.
+# pip3 install --upgrade pyepsilla
+
+from pyepsilla import vectordb
+
 
 ## 1.Connect to Epsilla VectorDB
-c = Client(host='127.0.0.1', port='8888', database='default')
+c = vectordb.Client(host='127.0.0.1', port='8888', database='default')
 
 ##
-status, body = c.welcome()
-status, body = c.state()
+status_code, response = c.welcome()
+status_code, response = c.state()
 
 ## Load DB with path
-c.load(dbname="myDB", path="/tmp/epsilla")
+status_code, response= c.load_db(db_name="myDB", db_path="/tmp/epsilla")
 
 ## Set DB to current DB
-c.use(dbname="myDB")
+c.use_db(db_name="myDB")
 
 ## Unload DB
 # c.unload(dbname="myDB")
 
 ## Create a table with schema in current DB
 id_field = {"name": "ID", "dataType": "INT", "primaryKey": True}
 doc_field = {"name": "Doc", "dataType": "STRING"}
 vec_field = {"name": "Embedding", "dataType": "VECTOR_FLOAT", "dimensions": 4}
 
 fields = [id_field, doc_field, vec_field]
-c.create_table(tablename="MyTable", fields=fields)
+status_code, response = c.create_table(table_name="MyTable", table_fields=fields)
 
 ## Insert new vector records into table
 Ids = [ i for i in range(5)]
 Docs = ["Berlin", "London", "Moscow", "San Francisco", "Shanghai"]
 Embedding =[[0.05, 0.61, 0.76, 0.74],
        [0.19, 0.81, 0.75, 0.11],
        [0.36, 0.55, 0.47, 0.94],
        [0.18, 0.01, 0.85, 0.80],
        [0.24, 0.18, 0.22, 0.44]
       ]
 
 records_data = [ {"ID": i, "Doc": Docs[i], "Embedding": Embedding[i]} for i in Ids]
-c.insert(tablename="MyTable", records=records_data)
+status_code, response = c.insert(table_name="MyTable", records=records_data)
 
 ## query vector
 queryField = "Embedding"
 queryVector = [0.35, 0.55, 0.47, 0.94]
 response = ["Doc"]
 limit = 2
-c.query(tablename="MyTable", queryField=queryField, queryVector=queryVector, response=response, limit=limit)
+status_code, response = c.query(table_name="MyTable", query_field=queryField, query_vector=queryVector, response_fields=response, limit=limit)
 
 ## drop table
-c.drop_table("MyTable")
+status_code, response = c.drop_table("MyTable")
 
 ## drop db
-c.drop_db("myDB")
+status_code, response = c.drop_db("myDB")
```

### Comparing `pyepsilla-0.0.3/pyepsilla/vectordb/client.py` & `pyepsilla-0.0.4/pyepsilla/vectordb/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 import json, requests
 
-class Table():
-    def __init__(self):
-        pass
-
-class DB():
-    def __init__(self):
-        pass
-
 class Client():
-    def __init__(self, host='localhost', port='8888', database='default'):
+    def __init__(self, host='localhost', port='8888', db_name='default'):
         self._protocol = "http"
         self._baseurl = "{}://{}:{}".format(self._protocol, host, port)
-        self._db=database
+        self._db=db_name
         self._timeout = 5
         self._header = {'Content-type': 'application/json'}
         self._rs = requests.Session()
 
+    def __check__(self):
+
+
     def welcome(self):
         req_url = "{}/".format(self._baseurl)
         req_data= None
         res = requests.get(url=req_url, data=json.dumps(req_data), headers=self._header, timeout=self._timeout)
         status_code = res.status_code
         body = res.text
         print("Return:", body)
@@ -34,74 +29,74 @@
         req_data= None
         res = self._rs.get(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
-    def use(self, dbname):
-        self._db = dbname
+    def use_db(self, db_name):
+        self._db = db_name
         pass
 
-    def load(self, dbname, path):
+    def load_db(self, db_name, db_path):
         req_url = "{}/api/load".format(self._baseurl)
-        req_data= {"path": path, "name": dbname}
+        req_data= {"name": db_name, "path": db_path}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
-    def unload(self, dbname):
-        req_url = "{}/api/{}/unload".format(self._baseurl, dbname)
+    def unload_db(self, db_name):
+        req_url = "{}/api/{}/unload".format(self._baseurl, db_name)
         res = requests.post(url=req_url, data=None, headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
-    def create_table(self, tablename="MyTable", fields=[]):
+    def create_table(self, table_name="MyTable", table_fields=[]):
         req_url = "{}/api/{}/schema/tables".format(self._baseurl, self._db)
-        req_data= {"name": tablename, "fields": fields}
+        req_data= {"name": table_name, "fields": table_fields}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
 
-    def insert(self, tablename="MyTable", records=[]):
+    def insert(self, table_name="MyTable", records=[]):
         req_url = "{}/api/{}/data/insert".format(self._baseurl, self._db)
-        req_data= {"table": tablename, "data": records}
+        req_data= {"table": table_name, "data": records}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
 
-    def query(self, tablename="MyTable", queryField=[], queryVector=[], response=[], limit=1):
+    def query(self, table_name="MyTable", query_field="", query_vector=[], response_fields=[], limit=1):
         req_url = "{}/api/{}/data/query".format(self._baseurl, self._db)
-        req_data= {"table": tablename, "queryField": queryField, "queryVector": queryVector, "response": response, "limit": limit}
+        req_data= {"table": table_name, "queryField": query_field, "queryVector": query_vector, "response": response_fields, "limit": limit}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
 
-    def drop_table(self, tablename="MyTable"):
-        req_url = "{}/api/{}/schema/tables/{}".format(self._baseurl, self._db, tablename)
+    def drop_table(self, table_name="MyTable"):
+        req_url = "{}/api/{}/schema/tables/{}".format(self._baseurl, self._db, table_name)
         req_data= None
         res = requests.delete(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
-    def drop_db(self, dbname):
-        req_url = "{}/api/{}/drop".format(self._baseurl, dbname)
+    def drop_db(self, db_name):
+        req_url = "{}/api/{}/drop".format(self._baseurl, db_name)
         res = requests.delete(url=req_url, data=None, headers=self._header)
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
```

### Comparing `pyepsilla-0.0.3/setup.py` & `pyepsilla-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.3',
+    version= '0.0.4',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
```

