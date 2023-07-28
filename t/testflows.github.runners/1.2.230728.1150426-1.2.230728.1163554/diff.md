# Comparing `tmp/testflows.github.runners-1.2.230728.1150426.tar.gz` & `tmp/testflows.github.runners-1.2.230728.1163554.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230728.1150426.tar", last modified: Fri Jul 28 15:04:27 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230728.1163554.tar", last modified: Fri Jul 28 16:35:54 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230728.1150426.tar` & `testflows.github.runners-1.2.230728.1163554.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1150426/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1150426/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 15:04:26.000000 testflows.github.runners-1.2.230728.1150426/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 15:04:26.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     9722 2023-07-28 12:18:30.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11437 2023-07-28 12:18:30.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1150426/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 15:04:27.048652 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 15:04:27.000000 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 15:04:27.000000 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 15:04:27.000000 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 15:04:27.000000 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 15:04:27.000000 testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1163554/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1163554/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9760 2023-07-28 16:35:01.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11437 2023-07-28 12:18:30.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230728.1150426/LICENSE` & `testflows.github.runners-1.2.230728.1163554/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/PKG-INFO` & `testflows.github.runners-1.2.230728.1163554/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1150426
+Version: 1.2.230728.1163554
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1150426/README.rst` & `testflows.github.runners-1.2.230728.1163554/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/setup.py` & `testflows.github.runners-1.2.230728.1163554/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230728.1150426",
+    version="1.2.230728.1163554",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230728.1150426"
+__version__ = "1.2.230728.1163554"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/config.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/logger.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_down.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,26 +128,26 @@
 
                         else:
                             zombie_servers.pop(server.name, None)
 
             with Action("Looking for idle runners", level=logging.DEBUG):
                 for runner in runners:
                     if runner.status == "online" and not runner.busy:
-                        if (
-                            runner.name.startswith(runner_name_prefix)
-                            and runner.name not in idle_runners
-                        ):
-                            with Action(f"Found new idle runner {runner.name}"):
-                                idle_runners[runner.name] = IdleRunner(
-                                    time=time.time(),
-                                    runner=runner,
-                                    observed_interval=current_interval,
-                                )
-                        idle_runners[runner.name].runner = runner
-                        idle_runners[runner.name].observed_interval = current_interval
+                        if runner.name.startswith(runner_name_prefix):
+                            if runner.name not in idle_runners:
+                                with Action(f"Found new idle runner {runner.name}"):
+                                    idle_runners[runner.name] = IdleRunner(
+                                        time=time.time(),
+                                        runner=runner,
+                                        observed_interval=current_interval,
+                                    )
+                            idle_runners[runner.name].runner = runner
+                            idle_runners[
+                                runner.name
+                            ].observed_interval = current_interval
 
             with Action(
                 "Checking which powered off servers need to be deleted",
                 level=logging.DEBUG,
             ):
                 for server_name in list(powered_off_servers.keys()):
                     powered_off_server = powered_off_servers[server_name]
```

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1150426
+Version: 1.2.230728.1163554
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1150426/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

