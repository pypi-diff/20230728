# Comparing `tmp/pybsky-0.0.17.tar.gz` & `tmp/pybsky-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybsky-0.0.17.tar", last modified: Fri Jul 28 11:58:35 2023, max compression
+gzip compressed data, was "pybsky-0.0.2.tar", last modified: Sun Jul 23 19:40:03 2023, max compression
```

## Comparing `pybsky-0.0.17.tar` & `pybsky-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:58:35.294625 pybsky-0.0.17/
--rw-rw-rw-   0        0        0     1100 2023-07-23 19:53:13.000000 pybsky-0.0.17/LICENSE
--rw-rw-rw-   0        0        0     1310 2023-07-28 11:58:35.293624 pybsky-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-07-28 11:37:14.000000 pybsky-0.0.17/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 11:58:35.284617 pybsky-0.0.17/pybsky/
--rw-rw-rw-   0        0        0       67 2023-07-27 23:24:08.000000 pybsky-0.0.17/pybsky/__init__.py
--rw-rw-rw-   0        0        0     3390 2023-07-28 08:27:29.000000 pybsky-0.0.17/pybsky/client.py
-drwxrwxrwx   0        0        0        0 2023-07-28 11:58:35.292625 pybsky-0.0.17/pybsky.egg-info/
--rw-rw-rw-   0        0        0     1310 2023-07-28 11:58:35.000000 pybsky-0.0.17/pybsky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-28 11:58:35.000000 pybsky-0.0.17/pybsky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:58:35.000000 pybsky-0.0.17/pybsky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 11:58:35.000000 pybsky-0.0.17/pybsky.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 11:58:35.000000 pybsky-0.0.17/pybsky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1384 2023-07-28 11:58:26.000000 pybsky-0.0.17/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 11:58:35.294625 pybsky-0.0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.421621 pybsky-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-07-23 19:26:05.000000 pybsky-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1183 2023-07-23 19:40:03.420621 pybsky-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-07-23 19:38:22.000000 pybsky-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.399622 pybsky-0.0.2/pybsky/
+-rw-rw-rw-   0        0        0       68 2023-07-23 18:34:27.000000 pybsky-0.0.2/pybsky/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 18:18:34.000000 pybsky-0.0.2/pybsky/client.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.416622 pybsky-0.0.2/pybsky/core/
+-rw-rw-rw-   0        0        0      122 2023-07-23 18:34:23.000000 pybsky-0.0.2/pybsky/core/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-07-21 12:03:54.000000 pybsky-0.0.2/pybsky/core/configs.py
+-rw-rw-rw-   0        0        0      266 2023-07-21 11:59:59.000000 pybsky-0.0.2/pybsky/core/exceptions.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 19:13:17.000000 pybsky-0.0.2/pybsky/core/log.py
+-rw-rw-rw-   0        0        0     5947 2023-07-23 18:36:54.000000 pybsky-0.0.2/pybsky/core/user_agents.py
+-rw-rw-rw-   0        0        0     1038 2023-07-23 18:38:10.000000 pybsky-0.0.2/pybsky/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.419622 pybsky-0.0.2/pybsky/mixins/
+-rw-rw-rw-   0        0        0       60 2023-07-23 18:34:35.000000 pybsky-0.0.2/pybsky/mixins/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 19:51:23.000000 pybsky-0.0.2/pybsky/mixins/base.py
+-rw-rw-rw-   0        0        0      878 2023-07-23 18:18:45.000000 pybsky-0.0.2/pybsky/mixins/feed.py
+-rw-rw-rw-   0        0        0     1399 2023-07-23 18:18:50.000000 pybsky-0.0.2/pybsky/mixins/login.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.411622 pybsky-0.0.2/pybsky.egg-info/
+-rw-rw-rw-   0        0        0     1183 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1031 2023-07-23 19:39:45.000000 pybsky-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-23 19:40:03.421621 pybsky-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-23 19:20:21.000000 pybsky-0.0.2/setup.py
```

### Comparing `pybsky-0.0.17/LICENSE` & `pybsky-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybsky-0.0.17/PKG-INFO` & `pybsky-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 Metadata-Version: 2.1
 Name: pybsky
-Version: 0.0.17
+Version: 0.0.2
 Summary: Python Client for bsky social media
+Author: softrebel, ovan
 Author-email: Mohammadreza softrebel <sh.mohammad66@yahoo.com>, Mahdi Ovan <mahdi.ovan@yahoo.com>
 Project-URL: Homepage, https://github.com/softrebel/pybsky
 Project-URL: Bug Tracker, https://github.com/softrebel/pybsky/issues
+Keywords: python,pybsky,bsky
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pybsky
 
 <div align='center'>
-
-![./a](./assets/cover.png)
+    <img src="./assets/cover.png" height="150" width="500" alt="pybsky-logo" >
 
 </div>
 
-# Requirements
-Python 3.10+
-
-Pybsky stands on the shoulder of:
-- requests package
-
-# Installation
-<div class="termy">
-  
-```console
- $ pip install pybsky
-
----> 100%
-```
-</div>
 
-## Feature List:
+## TODO List:
 
 - [x] Create Client
 - [x] Add Login logic
-- [x] Get Profile logic
-- [x] Get Follwer/Following logic
-- [x] Follow/Unfollow
-- [x] Get likes
-- [x] Get post, thread via replies
-- [x] Get Author Feed/Timeline
-- [x] Create post (text and image)
+- [ ] Get Profile logic
+- [ ] Get Follwer/Following logic
+- [ ] Follow/Unfollow
+- [ ] Get Likers
+- [ ] Get Commenters
+- [ ] Get Feed/Timeline
+- [ ] Post skeets
 
 ## License
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 
 - This project is licensed under the terms of the **[MIT license](LICENSE)**
```

### Comparing `pybsky-0.0.17/pybsky.egg-info/PKG-INFO` & `pybsky-0.0.2/pybsky.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 Metadata-Version: 2.1
 Name: pybsky
-Version: 0.0.17
+Version: 0.0.2
 Summary: Python Client for bsky social media
+Author: softrebel, ovan
 Author-email: Mohammadreza softrebel <sh.mohammad66@yahoo.com>, Mahdi Ovan <mahdi.ovan@yahoo.com>
 Project-URL: Homepage, https://github.com/softrebel/pybsky
 Project-URL: Bug Tracker, https://github.com/softrebel/pybsky/issues
+Keywords: python,pybsky,bsky
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pybsky
 
 <div align='center'>
-
-![./a](./assets/cover.png)
+    <img src="./assets/cover.png" height="150" width="500" alt="pybsky-logo" >
 
 </div>
 
-# Requirements
-Python 3.10+
-
-Pybsky stands on the shoulder of:
-- requests package
-
-# Installation
-<div class="termy">
-  
-```console
- $ pip install pybsky
-
----> 100%
-```
-</div>
 
-## Feature List:
+## TODO List:
 
 - [x] Create Client
 - [x] Add Login logic
-- [x] Get Profile logic
-- [x] Get Follwer/Following logic
-- [x] Follow/Unfollow
-- [x] Get likes
-- [x] Get post, thread via replies
-- [x] Get Author Feed/Timeline
-- [x] Create post (text and image)
+- [ ] Get Profile logic
+- [ ] Get Follwer/Following logic
+- [ ] Follow/Unfollow
+- [ ] Get Likers
+- [ ] Get Commenters
+- [ ] Get Feed/Timeline
+- [ ] Post skeets
 
 ## License
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 
 - This project is licensed under the terms of the **[MIT license](LICENSE)**
```

### Comparing `pybsky-0.0.17/pyproject.toml` & `pybsky-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 [project]
 name = "pybsky"
-version = "0.0.17"
+version = "0.0.2"
 authors = [
   { name="Mohammadreza softrebel", email="sh.mohammad66@yahoo.com" },
     { name="Mahdi Ovan", email="mahdi.ovan@yahoo.com" },
 ]
 description ='Python Client for bsky social media'
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "requests==2.31.0",
-]
 
 [project.urls]
 "Homepage" = "https://github.com/softrebel/pybsky"
 "Bug Tracker" = "https://github.com/softrebel/pybsky/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
@@ -34,13 +31,7 @@
 
 # Avoid trying to fix flake8-bugbear (`B`) violations.
 unfixable = ["B"]
 
 # Ignore `E402` (import violations) in all `__init__.py` files`.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402","F403","F401"]
-
-[tool.setuptools.packages.find]
-where = ["."]  # list of folders that contain the packages (["."] by default)
-include = ["pybsky"]  # package names should match these glob patterns (["*"] by default)
-exclude = []  # exclude packages matching these glob patterns (empty by default)
-namespaces = true
```

