# Comparing `tmp/SparkleWeb-0.1.1.tar.gz` & `tmp/SparkleWeb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleWeb-0.1.1.tar", last modified: Fri Jul 28 21:19:07 2023, max compression
+gzip compressed data, was "SparkleWeb-1.0.0.tar", last modified: Fri Jul 28 21:51:37 2023, max compression
```

## Comparing `SparkleWeb-0.1.1.tar` & `SparkleWeb-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 21:19:07.485176 SparkleWeb-0.1.1/
--rw-rw-rw-   0        0        0      179 2023-07-28 21:19:07.484106 SparkleWeb-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 21:19:07.463830 SparkleWeb-0.1.1/SparkleWeb/
--rw-rw-rw-   0        0        0     3116 2023-07-28 21:16:48.000000 SparkleWeb-0.1.1/SparkleWeb/SparkleWeb.py
--rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-0.1.1/SparkleWeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 21:19:07.482105 SparkleWeb-0.1.1/SparkleWeb.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 21:19:07.485176 SparkleWeb-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      304 2023-07-28 21:19:03.000000 SparkleWeb-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:51:37.212862 SparkleWeb-1.0.0/
+-rw-rw-rw-   0        0        0      179 2023-07-28 21:51:37.211864 SparkleWeb-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 21:51:37.188692 SparkleWeb-1.0.0/SparkleWeb/
+-rw-rw-rw-   0        0        0     3105 2023-07-28 21:51:19.000000 SparkleWeb-1.0.0/SparkleWeb/SparkleWeb.py
+-rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-1.0.0/SparkleWeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:51:37.209862 SparkleWeb-1.0.0/SparkleWeb.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-28 21:51:37.000000 SparkleWeb-1.0.0/SparkleWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-28 21:51:37.000000 SparkleWeb-1.0.0/SparkleWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 21:51:37.000000 SparkleWeb-1.0.0/SparkleWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 21:51:37.000000 SparkleWeb-1.0.0/SparkleWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 21:51:37.000000 SparkleWeb-1.0.0/SparkleWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 21:51:37.212862 SparkleWeb-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-07-28 21:51:32.000000 SparkleWeb-1.0.0/setup.py
```

### Comparing `SparkleWeb-0.1.1/SparkleWeb/SparkleWeb.py` & `SparkleWeb-1.0.0/SparkleWeb/SparkleWeb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from flask import Flask, jsonify, render_template, request, render_template_string
+from flask import jsonify, render_template, request, render_template_string
 from flask_cors import CORS
 import json
 import requests
 
-class Server:
-    def __init__(self, base, cssDict={}, jsDict={}) -> None:
-        self.app = Flask(__name__)
+class Server():
+    def __init__(self, app, base, cssDict={}, jsDict={}) -> None:
+        self.app = app
         CORS(self.app)
         self.cssDict = cssDict
         self.jsDict = jsDict
         self.base = base.get("template")
         self.base_title = base.get("title")
         self.base_args = base.get("args")
         self.base_reload = base.get("reloadRequired")
         self.app.jinja_env.filters['load'] = self.load
         self.app.add_url_rule('/', 'index', self.index, methods=['GET'])
         self.app.add_url_rule('/', 'response', self.response, methods=['POST'])
         self.base_template = requests.post("https://sparkleweb.vercel.app/index").text
 
-    def run(self, debug=True, port=5300):
+    def run(self, debug=False, port=5300):
         self.app.run(debug=debug, port=port)
 
     def index(self):
         siteData = {
             "route": request.base_url,
             "cssDict": self.cssDict,
             "jsDict": self.jsDict
```

