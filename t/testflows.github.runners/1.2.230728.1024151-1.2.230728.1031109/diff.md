# Comparing `tmp/testflows.github.runners-1.2.230728.1024151.tar.gz` & `tmp/testflows.github.runners-1.2.230728.1031109.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230728.1024151.tar", last modified: Fri Jul 28 02:41:51 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230728.1031109.tar", last modified: Fri Jul 28 03:11:09 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230728.1024151.tar` & `testflows.github.runners-1.2.230728.1031109.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1024151/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1024151/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22613 2023-07-27 16:08:42.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    12697 2023-07-27 16:52:27.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8668 2023-07-28 01:58:18.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10825 2023-07-28 02:40:02.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1024151/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 02:41:51.291957 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 02:41:51.000000 testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1031109/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1031109/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22613 2023-07-27 16:08:42.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    12697 2023-07-27 16:52:27.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8664 2023-07-28 03:09:56.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10817 2023-07-28 03:09:32.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230728.1024151/LICENSE` & `testflows.github.runners-1.2.230728.1031109/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/PKG-INFO` & `testflows.github.runners-1.2.230728.1031109/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1024151
+Version: 1.2.230728.1031109
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1024151/README.rst` & `testflows.github.runners-1.2.230728.1031109/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/setup.py` & `testflows.github.runners-1.2.230728.1031109/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230728.1024151",
+    version="1.2.230728.1031109",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230728.1024151"
+__version__ = "1.2.230728.1031109"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_down.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import time
 import logging
 import threading
 
 from dataclasses import dataclass
 
 from .actions import Action
-from .scale_up import runner_server_prefix, runner_name_prefix
+from .scale_up import server_name_prefix, runner_name_prefix
 
 from github.Repository import Repository
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from hcloud import Client
 from hcloud.servers.client import BoundServer
 
@@ -80,15 +80,15 @@
                 break
 
         with Action("Getting list of servers", level=logging.DEBUG):
             servers: list[BoundServer] = client.servers.get_all()
             servers = [
                 server
                 for server in servers
-                if server.name.startswith(runner_server_prefix)
+                if server.name.startswith(server_name_prefix)
             ]
 
         with Action("Getting list of self-hosted runners", level=logging.DEBUG):
             runners: list[SelfHostedActionsRunner] = repo.get_self_hosted_runners()
 
         with Action("Looking for powered off or zombie servers", level=logging.DEBUG):
             for server in servers:
```

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_up.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 from hcloud.images.domain import Image
 
 from github.Repository import Repository
 from github.WorkflowJob import WorkflowJob
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
-runner_server_prefix = "github-runner-"
-runner_name_prefix = runner_server_prefix
+server_name_prefix = "github-runner-"
+runner_name_prefix = server_name_prefix
 
 
 def server_setup(
     server: BoundServer,
     setup_script: str,
     startup_script: str,
     github_token: str,
@@ -230,18 +230,18 @@
                 for run in workflow_runs:
                     for job in run.jobs():
                         with Action("Getting list of servers", level=logging.DEBUG):
                             servers: list[BoundServer] = client.servers.get_all()
                             servers = [
                                 server
                                 for server in servers
-                                if server.name.startswith(runner_server_prefix)
+                                if server.name.startswith(server_name_prefix)
                             ]
 
-                        server_name = f"{runner_server_prefix}{job.run_id}-{job.id}"
+                        server_name = f"{server_name_prefix}{job.run_id}-{job.id}"
 
                         if job.status != "completed":
                             if server_name in [server.name for server in servers]:
                                 with Action(
                                     f"Server already exists for {job.status} {job}",
                                     level=logging.DEBUG,
                                 ):
```

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1024151
+Version: 1.2.230728.1031109
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1024151/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

