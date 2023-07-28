# Comparing `tmp/testflows.github.runners-1.2.230728.1163554.tar.gz` & `tmp/testflows.github.runners-1.2.230728.1180544.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230728.1163554.tar", last modified: Fri Jul 28 16:35:54 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230728.1180544.tar", last modified: Fri Jul 28 18:05:44 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230728.1163554.tar` & `testflows.github.runners-1.2.230728.1180544.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1163554/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1163554/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     9760 2023-07-28 16:35:01.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11437 2023-07-28 12:18:30.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.397243 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1163554/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 16:35:54.393243 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 16:35:54.000000 testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1180544/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1180544/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.494841 testflows.github.runners-1.2.230728.1180544/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.494841 testflows.github.runners-1.2.230728.1180544/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9760 2023-07-28 16:35:01.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13021 2023-07-28 17:58:32.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1180544/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 18:05:44.498842 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 18:05:44.000000 testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230728.1163554/LICENSE` & `testflows.github.runners-1.2.230728.1180544/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/PKG-INFO` & `testflows.github.runners-1.2.230728.1180544/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1163554
+Version: 1.2.230728.1180544
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1163554/README.rst` & `testflows.github.runners-1.2.230728.1180544/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/setup.py` & `testflows.github.runners-1.2.230728.1180544/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230728.1163554",
+    version="1.2.230728.1180544",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230728.1163554"
+__version__ = "1.2.230728.1180544"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/config.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/logger.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scale_up.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from hcloud.server_types.domain import ServerType
 from hcloud.locations.domain import Location
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 
 from github.Repository import Repository
 from github.WorkflowJob import WorkflowJob
+from github.WorkflowRun import WorkflowRun
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
 server_name_prefix = "github-runner-"
 runner_name_prefix = server_name_prefix
 
 
@@ -85,14 +86,15 @@
         )
 
 
 def create_server(
     setup_worker_pool: ThreadPoolExecutor,
     client: Client,
     job: WorkflowJob,
+    labels: list[str],
     name: str,
     server_type: ServerType,
     server_location: Location,
     server_image: Image,
     setup_script: str,
     startup_script: str,
     github_token: str,
@@ -118,15 +120,15 @@
     setup_worker_pool.submit(
         server_setup,
         server=response.server,
         setup_script=setup_script,
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
-        runner_labels=",".join(job.raw_data["labels"]),
+        runner_labels=",".join(labels),
         timeout=timeout,
     )
 
 
 def get_server_type(job: WorkflowJob, default: ServerType, label_prefix="type-"):
     """Get server type for the specified job."""
     server_type = None
@@ -221,23 +223,23 @@
         while True:
             if terminate.is_set():
                 with Action("Terminating scale up service"):
                     break
 
             try:
                 with Action("Getting workflow runs", level=logging.DEBUG):
-                    workflow_runs = repo.get_workflow_runs(
-                        branch="main", status="queued"
-                    )
+                    workflow_runs = repo.get_workflow_runs(status="queued")
 
                 futures: list[Future] = []
 
                 with Action("Looking for jobs", level=logging.DEBUG) as action:
                     for run in workflow_runs:
                         for job in run.jobs():
+                            labels = job.raw_data["labels"]
+
                             with Action("Getting list of servers", level=logging.DEBUG):
                                 servers: list[BoundServer] = client.servers.get_all()
                                 servers = [
                                     server
                                     for server in servers
                                     if server.name.startswith(server_name_prefix)
                                 ]
@@ -248,14 +250,41 @@
                                 if server_name in [server.name for server in servers]:
                                     with Action(
                                         f"Server already exists for {job.status} {job}",
                                         level=logging.DEBUG,
                                     ):
                                         continue
 
+                                if job.status == "in_progress":
+                                    victim_job = None
+
+                                    with Action(
+                                        f"Finding a job from which {job} stole the runner"
+                                    ):
+                                        victim_runner_name = job.raw_data["runner_name"]
+                                        (
+                                            victim_run_id,
+                                            victim_job_id,
+                                        ) = victim_runner_name.rsplit("-", 2)[-2:]
+                                        victim_run: WorkflowRun = repo.get_workflow_run(
+                                            victim_run_id
+                                        )
+
+                                        for victim_run_job in victim_run.jobs():
+                                            if victim_run_job.id == victim_job_id:
+                                                victim_job = victim_run_job
+                                                break
+
+                                        if victim_job is None:
+                                            raise ValueError(
+                                                f"victim job {victim_run_id}-{victim_job_id} was not found"
+                                            )
+
+                                        labels = victim_job.raw_data["labels"]
+
                                 with Action(
                                     f"Found job for which server was not created {job}"
                                 ):
                                     server_type = get_server_type(
                                         job=job, default=default_type
                                     )
                                     server_location = get_server_location(
@@ -277,14 +306,15 @@
 
                                     futures.append(
                                         worker_pool.submit(
                                             create_server,
                                             setup_worker_pool=setup_worker_pool,
                                             client=client,
                                             job=job,
+                                            labels=labels,
                                             name=server_name,
                                             server_type=server_type,
                                             server_location=server_location,
                                             server_image=server_image,
                                             setup_script=scripts.setup,
                                             startup_script=startup_script,
                                             github_token=github_token,
```

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230728.1180544/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1163554
+Version: 1.2.230728.1180544
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1163554/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230728.1180544/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

