# Comparing `tmp/webhaak-0.5.3.tar.gz` & `tmp/webhaak-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhaak-0.5.3.tar", last modified: Fri Jul 28 11:27:00 2023, max compression
+gzip compressed data, was "webhaak-0.5.4.tar", last modified: Fri Jul 28 11:47:09 2023, max compression
```

## Comparing `webhaak-0.5.3.tar` & `webhaak-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:27:00.001183 webhaak-0.5.3/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    11357 2021-10-12 17:55:24.000000 webhaak-0.5.3/LICENSE
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-07-28 11:27:00.001183 webhaak-0.5.3/PKG-INFO
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-07-03 15:05:41.000000 webhaak-0.5.3/README.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1327 2023-07-28 11:25:54.000000 webhaak-0.5.3/pyproject.toml
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-07-28 11:27:00.001183 webhaak-0.5.3/setup.cfg
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      189 2023-07-03 15:05:41.000000 webhaak-0.5.3/setup.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:26:59.997183 webhaak-0.5.3/src/
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:27:00.001183 webhaak-0.5.3/src/webhaak/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-03 15:05:41.000000 webhaak-0.5.3/src/webhaak/__init__.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    10158 2023-07-03 15:27:27.000000 webhaak-0.5.3/src/webhaak/incoming.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     9937 2023-07-03 19:59:32.000000 webhaak-0.5.3/src/webhaak/main.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    16684 2023-07-28 11:24:04.000000 webhaak-0.5.3/src/webhaak/tasks.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:27:00.001183 webhaak-0.5.3/src/webhaak.egg-info/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/PKG-INFO
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      343 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/SOURCES.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        1 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/dependency_links.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/entry_points.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      105 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/requires.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        8 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/top_level.txt
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:47:09.467773 webhaak-0.5.4/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    11357 2021-10-12 17:55:24.000000 webhaak-0.5.4/LICENSE
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-07-28 11:47:09.467773 webhaak-0.5.4/PKG-INFO
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-07-03 15:05:41.000000 webhaak-0.5.4/README.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1331 2023-07-28 11:46:00.000000 webhaak-0.5.4/pyproject.toml
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-07-28 11:47:09.467773 webhaak-0.5.4/setup.cfg
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      189 2023-07-03 15:05:41.000000 webhaak-0.5.4/setup.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:47:09.467773 webhaak-0.5.4/src/
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:47:09.467773 webhaak-0.5.4/src/webhaak/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-03 15:05:41.000000 webhaak-0.5.4/src/webhaak/__init__.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    10158 2023-07-03 15:27:27.000000 webhaak-0.5.4/src/webhaak/incoming.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     9937 2023-07-03 19:59:32.000000 webhaak-0.5.4/src/webhaak/main.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    16684 2023-07-28 11:24:04.000000 webhaak-0.5.4/src/webhaak/tasks.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:47:09.467773 webhaak-0.5.4/src/webhaak.egg-info/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-07-28 11:47:09.000000 webhaak-0.5.4/src/webhaak.egg-info/PKG-INFO
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      343 2023-07-28 11:47:09.000000 webhaak-0.5.4/src/webhaak.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        1 2023-07-28 11:47:09.000000 webhaak-0.5.4/src/webhaak.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       42 2023-07-28 11:47:09.000000 webhaak-0.5.4/src/webhaak.egg-info/entry_points.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      105 2023-07-28 11:47:09.000000 webhaak-0.5.4/src/webhaak.egg-info/requires.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        8 2023-07-28 11:47:09.000000 webhaak-0.5.4/src/webhaak.egg-info/top_level.txt
```

### Comparing `webhaak-0.5.3/LICENSE` & `webhaak-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.3/PKG-INFO` & `webhaak-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhaak
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple webhook service to update and deploy sites and do other maintenance and automatic tasks
 Author-email: Michiel Scholten <michiel@diginaut.net>
 License: Apache
 Project-URL: Homepage, https://github.com/aquatix/webhaak
 Project-URL: Bug Tracker, https://github.com/aquatix/webhaak/issues
 Keywords: webhook,api,automation,CI/CD
 Classifier: Framework :: FastAPI
```

### Comparing `webhaak-0.5.3/README.rst` & `webhaak-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.3/pyproject.toml` & `webhaak-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webhaak"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
     {name = "Michiel Scholten", email = "michiel@diginaut.net"},
 ]
 description= "Simple webhook service to update and deploy sites and do other maintenance and automatic tasks"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = ["webhook", "api", "automation", "CI/CD"]
@@ -26,15 +26,15 @@
     "strictyaml",
     "gitpython",
     "rq"
 ]
 # dynamic = ["version"]
 
 [project.scripts]
-my-script = "webhaak"
+my-script = "webhaak:app"
 
 [project.urls]
 "Homepage" = "https://github.com/aquatix/webhaak"
 "Bug Tracker" = "https://github.com/aquatix/webhaak/issues"
 
 [tool.ruff]
 exclude = [
```

### Comparing `webhaak-0.5.3/src/webhaak/incoming.py` & `webhaak-0.5.4/src/webhaak/incoming.py`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.3/src/webhaak/main.py` & `webhaak-0.5.4/src/webhaak/main.py`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.3/src/webhaak/tasks.py` & `webhaak-0.5.4/src/webhaak/tasks.py`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.3/src/webhaak.egg-info/PKG-INFO` & `webhaak-0.5.4/src/webhaak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhaak
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple webhook service to update and deploy sites and do other maintenance and automatic tasks
 Author-email: Michiel Scholten <michiel@diginaut.net>
 License: Apache
 Project-URL: Homepage, https://github.com/aquatix/webhaak
 Project-URL: Bug Tracker, https://github.com/aquatix/webhaak/issues
 Keywords: webhook,api,automation,CI/CD
 Classifier: Framework :: FastAPI
```

