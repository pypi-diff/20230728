# Comparing `tmp/cq23-2.5.0.tar.gz` & `tmp/cq23-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-2.5.0.tar", last modified: Thu Jul 27 14:16:04 2023, max compression
+gzip compressed data, was "cq23-2.6.0.tar", last modified: Fri Jul 28 01:33:19 2023, max compression
```

## Comparing `cq23-2.5.0.tar` & `cq23-2.6.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 14:16:04.235471 cq23-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 14:15:56.000000 cq23-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 14:15:56.000000 cq23-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-27 14:16:04.235471 cq23-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23/build_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/build_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/build_image/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/build_image/docker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/client_logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/client_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/client_logs/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/web_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/web_server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/web_server/files/loading_screen.html
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/zip/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 01:33:19.389171 cq23-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 01:33:10.000000 cq23-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 01:33:10.000000 cq23-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 01:33:19.389171 cq23-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/client_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/client_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/client_logs/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/web_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/web_server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/web_server/files/loading_screen.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.389171 cq23-2.6.0/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-28 01:33:10.000000 cq23-2.6.0/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:33:19.385170 cq23-2.6.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 01:33:19.000000 cq23-2.6.0/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-2.5.0/PKG-INFO` & `cq23-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.5.0
+Version: 2.6.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.5.0/setup.cfg` & `cq23-2.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 2.5.0
+version = 2.6.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-2.5.0/src/cq23/admin/aws.py` & `cq23-2.6.0/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/admin/builder.py` & `cq23-2.6.0/src/cq23/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/admin/worker.py` & `cq23-2.6.0/src/cq23/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/build_image/command.py` & `cq23-2.6.0/src/cq23/build_image/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         )
         exit(1)
 
     if name[0] in ["-", "_"] or name[-1] in ["-", "_"]:
         print("Name can't end with - or _.")
         exit(1)
 
-    if name in ["local-dev-client"]:
+    if name in ["local-dev-client", "sample-bot-1"]:
         print("This is a reserved name. Choose another name.")
         exit(1)
 
     docker_tools.ensure_docker_client_exists()
     docker_tools.check_dockerfile_exists()
     docker_tools.build_and_tag_image("cq-" + name)
     print(
```

### Comparing `cq23-2.5.0/src/cq23/build_image/docker_tools.py` & `cq23-2.6.0/src/cq23/build_image/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/check/command.py` & `cq23-2.6.0/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/cleanup/command.py` & `cq23-2.6.0/src/cq23/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/client_logs/command.py` & `cq23-2.6.0/src/cq23/client_logs/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/main/command.py` & `cq23-2.6.0/src/cq23/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/main/utils.py` & `cq23-2.6.0/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/new_client/command.py` & `cq23-2.6.0/src/cq23/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/replay/command.py` & `cq23-2.6.0/src/cq23/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/run_game/command.py` & `cq23-2.6.0/src/cq23/run_game/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def clean_image_name(image_name):
     """
     If the image name is one of the reserved ones, add the remote name to it.
     """
     if not image_name:
         return image_name
 
-    if image_name in []:  # Add reserved names here when there are any
+    if image_name in ["sample-bot-1"]:  # Add reserved names here when there are any
         image_name = (
             docker_tools.ECR_REGISTRY
             + "/"
             + docker_tools.SUBMISSIONS_ECR_REPO
             + ":"
             + image_name
         )
```

### Comparing `cq23-2.5.0/src/cq23/run_game/docker_tools.py` & `cq23-2.6.0/src/cq23/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/run_game/gcs.py` & `cq23-2.6.0/src/cq23/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/web_server/files/loading_screen.html` & `cq23-2.6.0/src/cq23/web_server/files/loading_screen.html`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/web_server/flask_api.py` & `cq23-2.6.0/src/cq23/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23/zip/command.py` & `cq23-2.6.0/src/cq23/zip/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.5.0/src/cq23.egg-info/PKG-INFO` & `cq23-2.6.0/src/cq23.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.5.0
+Version: 2.6.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.5.0/src/cq23.egg-info/SOURCES.txt` & `cq23-2.6.0/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

