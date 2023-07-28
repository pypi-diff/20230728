# Comparing `tmp/pyepsilla-0.0.7.tar.gz` & `tmp/pyepsilla-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.7.tar", last modified: Fri Jul 28 07:28:26 2023, max compression
+gzip compressed data, was "pyepsilla-0.0.8.tar", last modified: Fri Jul 28 13:00:22 2023, max compression
```

## Comparing `pyepsilla-0.0.7.tar` & `pyepsilla-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.486561 pyepsilla-0.0.7/
--rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.7/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.7/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:28:26.486338 pyepsilla-0.0.7/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.7/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.484431 pyepsilla-0.0.7/pyepsilla/
--rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.7/pyepsilla/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     1797 2023-07-28 07:24:52.000000 pyepsilla-0.0.7/pyepsilla/simple_example.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.485844 pyepsilla-0.0.7/pyepsilla/vectordb/
--rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.7/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     4334 2023-07-28 07:27:52.000000 pyepsilla-0.0.7/pyepsilla/vectordb/client.py
--rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.7/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 07:28:26.485245 pyepsilla-0.0.7/pyepsilla.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 07:28:26.000000 pyepsilla-0.0.7/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 07:28:26.486625 pyepsilla-0.0.7/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 07:28:01.000000 pyepsilla-0.0.7/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.246764 pyepsilla-0.0.8/
+-rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.8/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.8/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 13:00:22.246646 pyepsilla-0.0.8/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.8/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.244779 pyepsilla-0.0.8/pyepsilla/
+-rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.8/pyepsilla/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2416 2023-07-28 12:58:48.000000 pyepsilla-0.0.8/pyepsilla/simple_example.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.246235 pyepsilla-0.0.8/pyepsilla/vectordb/
+-rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.8/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     4360 2023-07-28 12:59:15.000000 pyepsilla-0.0.8/pyepsilla/vectordb/client.py
+-rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.8/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.245577 pyepsilla-0.0.8/pyepsilla.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 13:00:22.246803 pyepsilla-0.0.8/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 12:59:24.000000 pyepsilla-0.0.8/setup.py
```

### Comparing `pyepsilla-0.0.7/LICENSE` & `pyepsilla-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.7/README.md` & `pyepsilla-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.7/pyepsilla/simple_example.py` & `pyepsilla-0.0.8/pyepsilla/simple_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,75 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 # Try this simple example
-# 1. docker run -d -p 8888:8888 epsilla/vectordb
+# 1. docker run --pull=always -d -p 8888:8888 epsilla/vectordb
 # 2. pip3 install --upgrade pyepsilla
 # 3. python3 simple_example.py
 
 from pyepsilla import vectordb
-
+import random, string, time
 
 ## 1.Connect to Epsilla VectorDB
 c = vectordb.Client(host='127.0.0.1', port='8888', db_name='default')
+# c = vectordb.Client(host='3.209.6.179', port='8888', db_name='default')
 
 ##
 status_code, response = c.welcome()
 status_code, response = c.state()
 
 ## Load DB with path
 status_code, response= c.load_db(db_name="myDB", db_path="/tmp/epsilla")
 
 ## Set DB to current DB
 c.use_db(db_name="myDB")
 
 ## Unload DB
-# c.unload(dbname="myDB")
+# c.unload(db_name="myDB")
 
 ## Create a table with schema in current DB
+
+### define records number and vector dimension
+records_num = 3000
+dimensions = 8
+
 id_field = {"name": "ID", "dataType": "INT", "primaryKey": True}
 doc_field = {"name": "Doc", "dataType": "STRING"}
-vec_field = {"name": "Embedding", "dataType": "VECTOR_FLOAT", "dimensions": 4}
+vec_field = {"name": "Embedding", "dataType": "VECTOR_FLOAT", "dimensions": dimensions}
 
 fields = [id_field, doc_field, vec_field]
 status_code, response = c.create_table(table_name="MyTable", table_fields=fields)
 
 ## Insert new vector records into table
-Ids = [ i for i in range(5)]
-Docs = ["Berlin", "London", "Moscow", "San Francisco", "Shanghai"]
-Embedding =[[0.05, 0.61, 0.76, 0.74],
-       [0.19, 0.81, 0.75, 0.11],
-       [0.36, 0.55, 0.47, 0.94],
-       [0.18, 0.01, 0.85, 0.80],
-       [0.24, 0.18, 0.22, 0.44]
-      ]
+# Ids = [ i for i in range(5)]
+# Docs = ["Berlin", "London", "Moscow", "San Francisco", "Shanghai"]
+# Embedding =[[0.05, 0.61, 0.76, 0.74],
+#        [0.19, 0.81, 0.75, 0.11],
+#        [0.36, 0.55, 0.47, 0.94],
+#        [0.18, 0.01, 0.85, 0.80],
+#        [0.24, 0.18, 0.22, 0.44]
+#       ]
+
+## Insert new vector records
+letters = list(string.ascii_lowercase+string.ascii_uppercase+string.digits)
+Docs = [''.join(random.choices(letters, k=6)) for _ in range(records_num)]
+Embedding = [[random.random() for _ in range(dimensions)] for _ in range(records_num)]
 
-records_data = [ {"ID": i, "Doc": Docs[i], "Embedding": Embedding[i]} for i in Ids]
+records_data = [ {"ID": i, "Doc": Docs[i], "Embedding": Embedding[i]} for i in range(records_num)]
 status_code, response = c.insert(table_name="MyTable", records=records_data)
 
-## query vector
-queryField = "Embedding"
-queryVector = [0.35, 0.55, 0.47, 0.94]
-response = ["Doc"]
+# time.sleep(5)
+## Query Vectors
+query_field = "Embedding"
+query_vector = Embedding[-1]
+print(Docs[-1], query_vector)
+response_fields = ["Doc"]
 limit = 2
-status_code, response = c.query(table_name="MyTable", query_field=queryField, query_vector=queryVector, response_fields=response, limit=limit)
+status_code, response = c.query(table_name="MyTable", query_field=query_field, query_vector=query_vector, response_fields=response_fields, limit=limit)
+print("status_code", status_code, "response", response)
 
-## drop table
-status_code, response = c.drop_table("MyTable")
+## Drop table
+#status_code, response = c.drop_table("MyTable")
 
-## drop db
-status_code, response = c.drop_db("myDB")
+## Drop db
+#status_code, response = c.drop_db("myDB")
```

### Comparing `pyepsilla-0.0.7/pyepsilla/vectordb/client.py` & `pyepsilla-0.0.8/pyepsilla/vectordb/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,25 @@
         self._protocol = "http"
         self._host = host
         self._port = port
         self._baseurl = "{}://{}:{}".format(self._protocol, self._host, self._port)
         self._db=db_name
         self._timeout = 10
         self._header = {'Content-type': 'application/json'}
-        self.__check__()
+        self.check_networking()
 
-    def __check__(self):
+    def check_networking(self):
         socket.setdefaulttimeout(self._timeout)
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         check_result = s.connect_ex((self._host, int(self._port)))
+        s.close()
         if check_result == 0:
-            print("{}:{} can be arrived!".format(self._host, self._port))
+            print("[INFO] {}:{} can be arrived!".format(self._host, self._port))
         else:
-            print("{}:{} cann't be arrived!".format(self._host, self._port))
-        s.close()
+            raise Exception("[ERROR] {}:{} cann't be arrived!".format(self._host, self._port))
 
     def welcome(self):
         req_url = "{}/".format(self._baseurl)
         req_data= None
         res = requests.get(url=req_url, data=json.dumps(req_data), headers=self._header, timeout=self._timeout)
         status_code = res.status_code
         body = res.text
@@ -40,15 +40,14 @@
         status_code = res.status_code
         body = res.json()
         print("Return:", body)
         return status_code, body
 
     def use_db(self, db_name):
         self._db = db_name
-        pass
 
     def load_db(self, db_name, db_path):
         req_url = "{}/api/load".format(self._baseurl)
         req_data= {"name": db_name, "path": db_path}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
```

### Comparing `pyepsilla-0.0.7/pyepsilla/vectordb/field.py` & `pyepsilla-0.0.8/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.7/setup.py` & `pyepsilla-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.7',
+    version= '0.0.8',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
```

