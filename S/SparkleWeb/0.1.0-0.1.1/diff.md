# Comparing `tmp/SparkleWeb-0.1.0.tar.gz` & `tmp/SparkleWeb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleWeb-0.1.0.tar", last modified: Fri Jul 28 20:36:13 2023, max compression
+gzip compressed data, was "SparkleWeb-0.1.1.tar", last modified: Fri Jul 28 21:19:07 2023, max compression
```

## Comparing `SparkleWeb-0.1.0.tar` & `SparkleWeb-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 20:36:13.369369 SparkleWeb-0.1.0/
--rw-rw-rw-   0        0        0      179 2023-07-28 20:36:13.368365 SparkleWeb-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 20:36:13.348957 SparkleWeb-0.1.0/SparkleWeb/
--rw-rw-rw-   0        0        0     3119 2023-07-28 20:05:03.000000 SparkleWeb-0.1.0/SparkleWeb/SparkleWeb.py
--rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-0.1.0/SparkleWeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 20:36:13.367365 SparkleWeb-0.1.0/SparkleWeb.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-28 20:36:13.000000 SparkleWeb-0.1.0/SparkleWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-28 20:36:13.000000 SparkleWeb-0.1.0/SparkleWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:36:13.000000 SparkleWeb-0.1.0/SparkleWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 20:36:13.000000 SparkleWeb-0.1.0/SparkleWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-28 20:36:13.000000 SparkleWeb-0.1.0/SparkleWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 20:36:13.370383 SparkleWeb-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      304 2023-07-28 20:01:42.000000 SparkleWeb-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:19:07.485176 SparkleWeb-0.1.1/
+-rw-rw-rw-   0        0        0      179 2023-07-28 21:19:07.484106 SparkleWeb-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 21:19:07.463830 SparkleWeb-0.1.1/SparkleWeb/
+-rw-rw-rw-   0        0        0     3116 2023-07-28 21:16:48.000000 SparkleWeb-0.1.1/SparkleWeb/SparkleWeb.py
+-rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-0.1.1/SparkleWeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:19:07.482105 SparkleWeb-0.1.1/SparkleWeb.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 21:19:07.000000 SparkleWeb-0.1.1/SparkleWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 21:19:07.485176 SparkleWeb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-07-28 21:19:03.000000 SparkleWeb-0.1.1/setup.py
```

### Comparing `SparkleWeb-0.1.0/SparkleWeb/SparkleWeb.py` & `SparkleWeb-0.1.1/SparkleWeb/SparkleWeb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from flask import Flask, redirect, url_for, jsonify, render_template, request, render_template_string
+from flask import Flask, jsonify, render_template, request, render_template_string
 from flask_cors import CORS
 import json
 import requests
 
 class Server:
     def __init__(self, base, cssDict={}, jsDict={}) -> None:
         self.app = Flask(__name__)
@@ -12,15 +12,15 @@
         self.base = base.get("template")
         self.base_title = base.get("title")
         self.base_args = base.get("args")
         self.base_reload = base.get("reloadRequired")
         self.app.jinja_env.filters['load'] = self.load
         self.app.add_url_rule('/', 'index', self.index, methods=['GET'])
         self.app.add_url_rule('/', 'response', self.response, methods=['POST'])
-        self.base_template = requests.post("http://127.0.0.1:5100/index").text
+        self.base_template = requests.post("https://sparkleweb.vercel.app/index").text
 
     def run(self, debug=True, port=5300):
         self.app.run(debug=debug, port=port)
 
     def index(self):
         siteData = {
             "route": request.base_url,
@@ -62,8 +62,8 @@
         if requestType == "page":
             return 'loadPage({"request":"page", '+f'"template" : "{data["template"]}", "title" : "{data["title"]}", "args":{data["args"]},"reloadRequired" : {data["reload"]}'+'})'
 
         elif requestType == "section":
             return 'loadPage({"request":"section", '+f'"title" : "{data["title"]}", "template" : "{data["template"]}", "args":{data["args"]},"reloadRequired" : {data["reload"]}'+'}, body_id = '+f'"{data["target_id"]}")'
 
         else:
-            return 'loadPage({"request":"page", "template" : "error.html", "title" : "ERROR", "args":{"error": "Invalid Request Type :- request type must be page or section not ' + requestType + '"},"reloadRequired" : [] }, "mainServerBody", "http://127.0.0.1:5100/error")'
+            return 'loadPage({"request":"page", "template" : "error.html", "title" : "ERROR", "args":{"error": "Invalid Request Type :- request type must be page or section not ' + requestType + '"},"reloadRequired" : [] }, "mainServerBody", "https://sparkleweb.vercel.app/error")'
```

