# Comparing `tmp/cq23-2.6.0.tar.gz` & `tmp/cq23-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-2.6.0.tar", last modified: Fri Jul 28 01:33:19 2023, max compression
+gzip compressed data, was "cq23-2.6.1.tar", last modified: Fri Jul 28 04:40:10 2023, max compression
```

## Comparing `cq23-2.6.0.tar` & `cq23-2.6.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 01:33:19.389171 cq23-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 01:33:10.000000 cq23-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 01:33:10.000000 cq23-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 01:33:19.389171 cq23-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/build_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/build_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/build_image/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/build_image/docker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/client_logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/client_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/client_logs/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/web_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/web_server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/web_server/files/loading_screen.html
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/zip/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.042409 cq23-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 04:40:10.042409 cq23-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 04:40:00.000000 cq23-2.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 04:40:00.000000 cq23-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 04:40:10.042409 cq23-2.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.034409 cq23-2.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/client_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/client_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/client_logs/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.042409 cq23-2.6.1/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.042409 cq23-2.6.1/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/web_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.042409 cq23-2.6.1/src/cq23/web_server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/web_server/files/loading_screen.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.042409 cq23-2.6.1/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-28 04:40:00.000000 cq23-2.6.1/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:40:10.038409 cq23-2.6.1/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 04:40:10.000000 cq23-2.6.1/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 04:40:10.000000 cq23-2.6.1/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:40:10.000000 cq23-2.6.1/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 04:40:10.000000 cq23-2.6.1/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 04:40:10.000000 cq23-2.6.1/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 04:40:10.000000 cq23-2.6.1/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-2.6.0/PKG-INFO` & `cq23-2.6.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.6.0
+Version: 2.6.1
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.6.0/setup.cfg` & `cq23-2.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 2.6.0
+version = 2.6.1
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-2.6.0/src/cq23/admin/aws.py` & `cq23-2.6.1/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/admin/builder.py` & `cq23-2.6.1/src/cq23/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/admin/worker.py` & `cq23-2.6.1/src/cq23/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/build_image/command.py` & `cq23-2.6.1/src/cq23/build_image/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/build_image/docker_tools.py` & `cq23-2.6.1/src/cq23/build_image/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/check/command.py` & `cq23-2.6.1/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/cleanup/command.py` & `cq23-2.6.1/src/cq23/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/client_logs/command.py` & `cq23-2.6.1/src/cq23/client_logs/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/main/command.py` & `cq23-2.6.1/src/cq23/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/main/utils.py` & `cq23-2.6.1/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/new_client/command.py` & `cq23-2.6.1/src/cq23/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/replay/command.py` & `cq23-2.6.1/src/cq23/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/run_game/command.py` & `cq23-2.6.1/src/cq23/run_game/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,25 @@
         current_dir = os.getcwd()
         os.chdir(folder_path)
         subprocess.run(["git", "pull"])
         os.chdir(current_dir)
     print(folder_path + " cloned successfully.")
 
 
-def extract_arg_from_command_args(arg_name, args, default=None):
+def extract_arg_from_command_args(arg_name, args, default=None, lower=False):
     arg_value = list(filter(lambda x: str(x).startswith(arg_name + "="), args))
     if not arg_value:
         return default
     if len(arg_value) > 1:
         raise Exception(f"Multiple `{arg_name}` arguments provided.")
 
-    return arg_value[0][len(arg_name) + 1 :]  # noqa: E203
+    val = arg_value[0][len(arg_name) + 1 :]  # noqa: E203
+    if lower:
+        return str(val).lower()
+    return val
 
 
 def copy_container_logs(game_files_abs_path, gcs_folder_name):
     src_dir = os.path.join(os.path.join(gcs_folder_name, "src"), "container_logs")
     dst_dir = os.path.join(game_files_abs_path, "replay_files")
     for filename in os.listdir(src_dir):
         src_file = os.path.join(src_dir, filename)
@@ -86,14 +89,14 @@
     clone_or_pull_repository(gcs_repo, gcs_folder_name)
     print("KH73TU")
     docker_tools.pull_latest_game_server()
     run_gcs(
         gcs_folder_name,
         home_image,
         away_image,
-        extract_arg_from_command_args("map", args),
+        extract_arg_from_command_args("map", args, lower=True),
     )
     docker_tools.copy_replay_files(game_files_abs_path)
     copy_container_logs(game_files_abs_path, gcs_folder_name)
 
     # Go back to the same directory as we were (one up)
     os.chdir(os.path.dirname(os.getcwd()))
```

### Comparing `cq23-2.6.0/src/cq23/run_game/docker_tools.py` & `cq23-2.6.1/src/cq23/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/run_game/gcs.py` & `cq23-2.6.1/src/cq23/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/web_server/files/loading_screen.html` & `cq23-2.6.1/src/cq23/web_server/files/loading_screen.html`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/web_server/flask_api.py` & `cq23-2.6.1/src/cq23/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23/zip/command.py` & `cq23-2.6.1/src/cq23/zip/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.6.0/src/cq23.egg-info/PKG-INFO` & `cq23-2.6.1/src/cq23.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.6.0
+Version: 2.6.1
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.6.0/src/cq23.egg-info/SOURCES.txt` & `cq23-2.6.1/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

