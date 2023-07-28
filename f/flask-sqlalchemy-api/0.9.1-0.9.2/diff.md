# Comparing `tmp/flask-sqlalchemy-api-0.9.1.tar.gz` & `tmp/flask-sqlalchemy-api-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-sqlalchemy-api-0.9.1.tar", last modified: Sat Jul  8 17:28:46 2023, max compression
+gzip compressed data, was "flask-sqlalchemy-api-0.9.2.tar", last modified: Fri Jul 28 14:46:33 2023, max compression
```

## Comparing `flask-sqlalchemy-api-0.9.1.tar` & `flask-sqlalchemy-api-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:28:46.541948 flask-sqlalchemy-api-0.9.1/
--rw-r--r--   0 abc        (911) abc        (911)       39 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.1/AUTHORS.txt
--rw-r--r--   0 abc        (911) abc        (911)      162 2023-07-08 16:40:28.000000 flask-sqlalchemy-api-0.9.1/CHANGES.md
--rw-r--r--   0 abc        (911) abc        (911)      450 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.1/CLASSIFIERS.txt
--rw-r--r--   0 abc        (911) abc        (911)      177 2023-07-08 17:25:46.000000 flask-sqlalchemy-api-0.9.1/MANIFEST.in
--rw-r--r--   0 abc        (911) abc        (911)     4684 2023-07-08 17:28:46.537948 flask-sqlalchemy-api-0.9.1/PKG-INFO
--rw-r--r--   0 abc        (911) abc        (911)     3625 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.1/README.md
--rw-r--r--   0 abc        (911) abc        (911)       23 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.1/REQUIREMENTS.txt
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:28:46.537948 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api/
--rw-r--r--   0 abc        (911) abc        (911)       37 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api/__init__.py
--rw-r--r--   0 abc        (911) abc        (911)     7456 2023-07-08 17:28:16.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api/main.py
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:28:46.537948 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/
--rw-r--r--   0 abc        (911) abc        (911)     4684 2023-07-08 17:28:46.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/PKG-INFO
--rw-r--r--   0 abc        (911) abc        (911)      410 2023-07-08 17:28:46.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/SOURCES.txt
--rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-08 17:28:46.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/dependency_links.txt
--rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-08 17:28:46.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/not-zip-safe
--rw-r--r--   0 abc        (911) abc        (911)       24 2023-07-08 17:28:46.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/requires.txt
--rw-r--r--   0 abc        (911) abc        (911)       21 2023-07-08 17:28:46.000000 flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/top_level.txt
--rw-r--r--   0 abc        (911) abc        (911)       38 2023-07-08 17:28:46.541948 flask-sqlalchemy-api-0.9.1/setup.cfg
--rw-r--r--   0 abc        (911) abc        (911)     1360 2023-07-08 17:27:51.000000 flask-sqlalchemy-api-0.9.1/setup.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/
+-rw-r--r--   0 abc        (911) abc        (911)       39 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.2/AUTHORS.txt
+-rw-r--r--   0 abc        (911) abc        (911)      224 2023-07-08 17:52:28.000000 flask-sqlalchemy-api-0.9.2/CHANGES.md
+-rw-r--r--   0 abc        (911) abc        (911)      450 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.2/CLASSIFIERS.txt
+-rw-r--r--   0 abc        (911) abc        (911)      177 2023-07-08 17:25:46.000000 flask-sqlalchemy-api-0.9.2/MANIFEST.in
+-rw-r--r--   0 abc        (911) abc        (911)     4823 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/PKG-INFO
+-rw-r--r--   0 abc        (911) abc        (911)     3662 2023-07-28 14:39:20.000000 flask-sqlalchemy-api-0.9.2/README.md
+-rw-r--r--   0 abc        (911) abc        (911)       23 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.2/REQUIREMENTS.txt
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/
+-rw-r--r--   0 abc        (911) abc        (911)       46 2023-07-26 15:36:37.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/__init__.py
+-rw-r--r--   0 abc        (911) abc        (911)    12581 2023-07-28 14:35:32.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/main.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/
+-rw-r--r--   0 abc        (911) abc        (911)     4823 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/PKG-INFO
+-rw-r--r--   0 abc        (911) abc        (911)      410 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/not-zip-safe
+-rw-r--r--   0 abc        (911) abc        (911)       24 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/requires.txt
+-rw-r--r--   0 abc        (911) abc        (911)       21 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/top_level.txt
+-rw-r--r--   0 abc        (911) abc        (911)       38 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/setup.cfg
+-rw-r--r--   0 abc        (911) abc        (911)     1411 2023-07-28 14:46:26.000000 flask-sqlalchemy-api-0.9.2/setup.py
```

### Comparing `flask-sqlalchemy-api-0.9.1/PKG-INFO` & `flask-sqlalchemy-api-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-api
-Version: 0.9.1
+Version: 0.9.2
 Summary: flask-sqlalchemy-api extension for flask application
 Home-page: https://github.com/fraoustin/flask-sqlalchemy-api.git
 Author: Frédéric Aoustin
 Author-email: fraoustin@gmail.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python
@@ -14,48 +14,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
+Description-Content-Type: text/markdown
 License-File: AUTHORS.txt
 
 # flask-sqlachemy-api
 
 generate API Rest from Model Class
 
 
 ## Installation
 
 
-::
-
     pip install flask-sqlachemy-api
         
 Or
 
-::
-
     git clone https://github.com/fraoustin/flask-sqlachemy-api.git
     cd flask-sqlachemy-api
     python setup.py install
 
 You can load test by
 
-::
-
     flake8 --ignore E501,E226,E128,F401
     python -m unittest discover -s tests
 
 
 ## Usage
 
-::
-
     import os, logging
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from flask_sqlalchemy_api import ApiRest, error_api
 
     app = Flask(__name__)
 
@@ -97,59 +90,79 @@
 - PATCH http://127.0.0.1:5000/api/v1/todo/<id>
 
 
 flask-sqlachemy-api generate 6 Apis from Model Class
 
 - ALL: it's a get request for list of item with url http://domain/api_path/items. You can add parameter filter, orderby, offset, limit.
 
-> http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc  method GET
-> http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc&filter=id%3D  method GET
-> http://127.0.0.1:5000/api/v1/todos?offset=50&limit=50  method GET
+    http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc  method GET
+
+    http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc&filter=id%3D  method GET
+
+    http://127.0.0.1:5000/api/v1/todos?offset=50&limit=50  method GET
 
 - GET: it's get request for  a specific item with url http://domain/api_path/item/<id>
 
-> http://127.0.0.1:5000/api/v1/todo/1 method GET
+    http://127.0.0.1:5000/api/v1/todo/1 method GET
 
 - DELETE: it's delete request for a specific item url http://domain/api_path/item/<id>
 
-> http://127.0.0.1:5000/api/v1/todo/1  method DELETE
+    http://127.0.0.1:5000/api/v1/todo/1  method DELETE
 
 - POST: it's post request for add a item with url http://domain/api_path/item. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo  method POST
+    http://127.0.0.1:5000/api/v1/todo  method POST
 
 - PUT: it's put request for modify a specific item with url http://domain/api_path/item/<id>. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo/1  method PUT
+    http://127.0.0.1:5000/api/v1/todo/1  method PUT
 
 - PATCH: it's patch request for modify a specific item on specific column with url http://domain/api_path/item/<id>. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo/1  method PATCH
+    http://127.0.0.1:5000/api/v1/todo/1  method PATCH
 
 You can 
 
 - specific url (default /api/v1) on ApiRest
 - add decorator (login, ...) in sample/sample1.py
 - specific endpoint
 - specific serialize: transform item to json
 
+## Sample
+
+You can launch sample 0 and 1
+
+    python sample/sample0.py &
+    python sample/sample0_test.py
+
+You can launch sample3
+
+    python sample/sample3.py
+
+And you test API by swagger UI on http://127.0.0.1:5000/swagger
 
 ## TODO
 
-- essayer avec une pk sur plusieurs champs
-- voir pour plusieurs mimetype
-- voir pour test avec html (swagger.json) https://github.com/getsling/flask-swagger
-- faire test avec des fk non respecté (voir comment en sqlachemy on les décrit)
-- faire un outil pour ouvrir les dbml et faire des query
 - voir pour faire des apis lié au fk ex /api/person/(int: id)/computers (https://flask-restless.readthedocs.io/en/stable/requestformat.html)
+- faire exemple flask-sqlalchemy-api + dbml-to-sqlalchemy
+- faire full application todo avec gestion user
 
 # Feature
 
 - generate documentation
 - TODO
 
+# V. 0.9.2
+
+- change README
+
+
+# V. 0.9.1
+
+- correction setup
+
 # V. 0.9.0
 
 - init repos
 - add api 'ALL', 'POST', 'GET', 'DELETE', 'PUT', 'PATCH'
 - manage decorator, serialize, error
```

### Comparing `flask-sqlalchemy-api-0.9.1/README.md` & `flask-sqlalchemy-api-0.9.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,30 @@
 
 generate API Rest from Model Class
 
 
 ## Installation
 
 
-::
-
     pip install flask-sqlachemy-api
         
 Or
 
-::
-
     git clone https://github.com/fraoustin/flask-sqlachemy-api.git
     cd flask-sqlachemy-api
     python setup.py install
 
 You can load test by
 
-::
-
     flake8 --ignore E501,E226,E128,F401
     python -m unittest discover -s tests
 
 
 ## Usage
 
-::
-
     import os, logging
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from flask_sqlalchemy_api import ApiRest, error_api
 
     app = Flask(__name__)
 
@@ -75,47 +67,58 @@
 - PATCH http://127.0.0.1:5000/api/v1/todo/<id>
 
 
 flask-sqlachemy-api generate 6 Apis from Model Class
 
 - ALL: it's a get request for list of item with url http://domain/api_path/items. You can add parameter filter, orderby, offset, limit.
 
-> http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc  method GET
-> http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc&filter=id%3D  method GET
-> http://127.0.0.1:5000/api/v1/todos?offset=50&limit=50  method GET
+    http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc  method GET
+
+    http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc&filter=id%3D  method GET
+
+    http://127.0.0.1:5000/api/v1/todos?offset=50&limit=50  method GET
 
 - GET: it's get request for  a specific item with url http://domain/api_path/item/<id>
 
-> http://127.0.0.1:5000/api/v1/todo/1 method GET
+    http://127.0.0.1:5000/api/v1/todo/1 method GET
 
 - DELETE: it's delete request for a specific item url http://domain/api_path/item/<id>
 
-> http://127.0.0.1:5000/api/v1/todo/1  method DELETE
+    http://127.0.0.1:5000/api/v1/todo/1  method DELETE
 
 - POST: it's post request for add a item with url http://domain/api_path/item. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo  method POST
+    http://127.0.0.1:5000/api/v1/todo  method POST
 
 - PUT: it's put request for modify a specific item with url http://domain/api_path/item/<id>. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo/1  method PUT
+    http://127.0.0.1:5000/api/v1/todo/1  method PUT
 
 - PATCH: it's patch request for modify a specific item on specific column with url http://domain/api_path/item/<id>. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo/1  method PATCH
+    http://127.0.0.1:5000/api/v1/todo/1  method PATCH
 
 You can 
 
 - specific url (default /api/v1) on ApiRest
 - add decorator (login, ...) in sample/sample1.py
 - specific endpoint
 - specific serialize: transform item to json
 
+## Sample
+
+You can launch sample 0 and 1
+
+    python sample/sample0.py &
+    python sample/sample0_test.py
+
+You can launch sample3
+
+    python sample/sample3.py
+
+And you test API by swagger UI on http://127.0.0.1:5000/swagger
 
 ## TODO
 
-- essayer avec une pk sur plusieurs champs
-- voir pour plusieurs mimetype
-- voir pour test avec html (swagger.json) https://github.com/getsling/flask-swagger
-- faire test avec des fk non respecté (voir comment en sqlachemy on les décrit)
-- faire un outil pour ouvrir les dbml et faire des query
-- voir pour faire des apis lié au fk ex /api/person/(int: id)/computers (https://flask-restless.readthedocs.io/en/stable/requestformat.html)
+- voir pour faire des apis lié au fk ex /api/person/(int: id)/computers (https://flask-restless.readthedocs.io/en/stable/requestformat.html)
+- faire exemple flask-sqlalchemy-api + dbml-to-sqlalchemy
+- faire full application todo avec gestion user
```

### Comparing `flask-sqlalchemy-api-0.9.1/flask_sqlalchemy_api.egg-info/PKG-INFO` & `flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-api
-Version: 0.9.1
+Version: 0.9.2
 Summary: flask-sqlalchemy-api extension for flask application
 Home-page: https://github.com/fraoustin/flask-sqlalchemy-api.git
 Author: Frédéric Aoustin
 Author-email: fraoustin@gmail.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python
@@ -14,48 +14,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
+Description-Content-Type: text/markdown
 License-File: AUTHORS.txt
 
 # flask-sqlachemy-api
 
 generate API Rest from Model Class
 
 
 ## Installation
 
 
-::
-
     pip install flask-sqlachemy-api
         
 Or
 
-::
-
     git clone https://github.com/fraoustin/flask-sqlachemy-api.git
     cd flask-sqlachemy-api
     python setup.py install
 
 You can load test by
 
-::
-
     flake8 --ignore E501,E226,E128,F401
     python -m unittest discover -s tests
 
 
 ## Usage
 
-::
-
     import os, logging
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from flask_sqlalchemy_api import ApiRest, error_api
 
     app = Flask(__name__)
 
@@ -97,59 +90,79 @@
 - PATCH http://127.0.0.1:5000/api/v1/todo/<id>
 
 
 flask-sqlachemy-api generate 6 Apis from Model Class
 
 - ALL: it's a get request for list of item with url http://domain/api_path/items. You can add parameter filter, orderby, offset, limit.
 
-> http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc  method GET
-> http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc&filter=id%3D  method GET
-> http://127.0.0.1:5000/api/v1/todos?offset=50&limit=50  method GET
+    http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc  method GET
+
+    http://127.0.0.1:5000/api/v1/todos?orderby=title%20desc&filter=id%3D  method GET
+
+    http://127.0.0.1:5000/api/v1/todos?offset=50&limit=50  method GET
 
 - GET: it's get request for  a specific item with url http://domain/api_path/item/<id>
 
-> http://127.0.0.1:5000/api/v1/todo/1 method GET
+    http://127.0.0.1:5000/api/v1/todo/1 method GET
 
 - DELETE: it's delete request for a specific item url http://domain/api_path/item/<id>
 
-> http://127.0.0.1:5000/api/v1/todo/1  method DELETE
+    http://127.0.0.1:5000/api/v1/todo/1  method DELETE
 
 - POST: it's post request for add a item with url http://domain/api_path/item. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo  method POST
+    http://127.0.0.1:5000/api/v1/todo  method POST
 
 - PUT: it's put request for modify a specific item with url http://domain/api_path/item/<id>. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo/1  method PUT
+    http://127.0.0.1:5000/api/v1/todo/1  method PUT
 
 - PATCH: it's patch request for modify a specific item on specific column with url http://domain/api_path/item/<id>. You add data on your request
 
-> http://127.0.0.1:5000/api/v1/todo/1  method PATCH
+    http://127.0.0.1:5000/api/v1/todo/1  method PATCH
 
 You can 
 
 - specific url (default /api/v1) on ApiRest
 - add decorator (login, ...) in sample/sample1.py
 - specific endpoint
 - specific serialize: transform item to json
 
+## Sample
+
+You can launch sample 0 and 1
+
+    python sample/sample0.py &
+    python sample/sample0_test.py
+
+You can launch sample3
+
+    python sample/sample3.py
+
+And you test API by swagger UI on http://127.0.0.1:5000/swagger
 
 ## TODO
 
-- essayer avec une pk sur plusieurs champs
-- voir pour plusieurs mimetype
-- voir pour test avec html (swagger.json) https://github.com/getsling/flask-swagger
-- faire test avec des fk non respecté (voir comment en sqlachemy on les décrit)
-- faire un outil pour ouvrir les dbml et faire des query
 - voir pour faire des apis lié au fk ex /api/person/(int: id)/computers (https://flask-restless.readthedocs.io/en/stable/requestformat.html)
+- faire exemple flask-sqlalchemy-api + dbml-to-sqlalchemy
+- faire full application todo avec gestion user
 
 # Feature
 
 - generate documentation
 - TODO
 
+# V. 0.9.2
+
+- change README
+
+
+# V. 0.9.1
+
+- correction setup
+
 # V. 0.9.0
 
 - init repos
 - add api 'ALL', 'POST', 'GET', 'DELETE', 'PUT', 'PATCH'
 - manage decorator, serialize, error
```

### Comparing `flask-sqlalchemy-api-0.9.1/setup.py` & `flask-sqlalchemy-api-0.9.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Setup for flask-sqlalchemy-api
 """
 
 import os
 from setuptools import setup, find_packages
 
-__version_info__ = (0, 9, 1)
+__version_info__ = (0, 9, 2)
 VERSION = '.'.join([str(val) for val in __version_info__])
 NAME = "flask-sqlalchemy-api"
 DESC = "flask-sqlalchemy-api extension for flask application"
 URLPKG = "https://github.com/fraoustin/flask-sqlalchemy-api.git"
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
@@ -35,14 +35,15 @@
     name=NAME,
     version=VERSION,
     packages=find_packages(),
     author=AUTHORS,
     author_email=AUTHORS_EMAIL,
     description=DESC,
     long_description=LONG_DESC,
+    long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=REQUIRED,
     url=URLPKG,
     classifiers=CLASSIFIED,
     entry_points={},
     zip_safe=False,
     platforms='any'
```

