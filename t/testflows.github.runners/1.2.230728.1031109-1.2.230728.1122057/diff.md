# Comparing `tmp/testflows.github.runners-1.2.230728.1031109.tar.gz` & `tmp/testflows.github.runners-1.2.230728.1122057.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230728.1031109.tar", last modified: Fri Jul 28 03:11:09 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230728.1122057.tar", last modified: Fri Jul 28 12:20:57 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230728.1031109.tar` & `testflows.github.runners-1.2.230728.1122057.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1031109/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1031109/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22613 2023-07-27 16:08:42.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    12697 2023-07-27 16:52:27.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8664 2023-07-28 03:09:56.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10817 2023-07-28 03:09:32.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1031109/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 03:11:09.783347 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 03:11:09.000000 testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.595384 testflows.github.runners-1.2.230728.1122057/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1122057/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 12:20:57.595384 testflows.github.runners-1.2.230728.1122057/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1122057/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 12:20:57.595384 testflows.github.runners-1.2.230728.1122057/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    12697 2023-07-27 16:52:27.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9722 2023-07-28 12:18:30.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11437 2023-07-28 12:18:30.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1122057/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 12:20:57.591383 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1035 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 12:20:57.000000 testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230728.1031109/LICENSE` & `testflows.github.runners-1.2.230728.1122057/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/PKG-INFO` & `testflows.github.runners-1.2.230728.1122057/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1031109
+Version: 1.2.230728.1122057
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1031109/README.rst` & `testflows.github.runners-1.2.230728.1122057/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/setup.py` & `testflows.github.runners-1.2.230728.1122057/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230728.1031109",
+    version="1.2.230728.1122057",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230728.1031109"
+__version__ = "1.2.230728.1122057"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,23 @@
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.scripts import Scripts, scripts
+from testflows.github.runners.logger import logger
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 
 check_args = args.check
 check_image = args.check_image
 
-logger = logging.getLogger("testflows.github.runners")
-
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
     powered off when job completes and then powered off servers are
     automatically deleted.
@@ -613,26 +612,28 @@
                     default_location=args.default_location,
                     worker_pool=worker_pool,
                     github_token=args.github_token,
                     github_repository=args.github_repository,
                     interval=args.scale_up_interval,
                     max_servers=args.max_runners,
                     max_server_ready_time=args.max_server_ready_time,
+                    debug=args.debug,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
                     terminate=terminate,
                     repo=repo,
                     client=client,
                     max_powered_off_time=args.max_powered_off_time,
                     max_idle_runner_time=args.max_idle_runner_time,
                     max_runner_registration_time=args.max_runner_registration_time,
                     interval=args.scale_down_interval,
+                    debug=args.debug,
                 )
 
             while True:
                 time.sleep(1)
 
                 if scale_up_service.done():
                     raise RuntimeError("scale-up service exited")
```

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scale_down.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import logging
 import threading
 
 from dataclasses import dataclass
 
 from .actions import Action
 from .scale_up import server_name_prefix, runner_name_prefix
+from .logger import logger
 
 from github.Repository import Repository
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from hcloud import Client
 from hcloud.servers.client import BoundServer
 
@@ -59,14 +60,15 @@
     terminate: threading.Event,
     repo: Repository,
     client: Client,
     max_powered_off_time: int,
     max_idle_runner_time: int,
     max_runner_registration_time: int,
     interval: int,
+    debug: bool = False,
 ):
     """Scale down service by deleting any powered off server,
     any server that has stale idle runner, or any server that failed to register its
     runner (zombie server).
     """
     powered_off_servers: dict[str, PoweredOffServer] = {}
     idle_runners: dict[str, IdleRunner] = {}
@@ -75,143 +77,162 @@
     while True:
         current_interval = time.time()
 
         if terminate.is_set():
             with Action("Terminating scale down service"):
                 break
 
-        with Action("Getting list of servers", level=logging.DEBUG):
-            servers: list[BoundServer] = client.servers.get_all()
-            servers = [
-                server
-                for server in servers
-                if server.name.startswith(server_name_prefix)
-            ]
-
-        with Action("Getting list of self-hosted runners", level=logging.DEBUG):
-            runners: list[SelfHostedActionsRunner] = repo.get_self_hosted_runners()
-
-        with Action("Looking for powered off or zombie servers", level=logging.DEBUG):
-            for server in servers:
-                if server.status == server.STATUS_OFF:
-                    if server.name not in powered_off_servers:
-                        with Action(f"Found new powered off server {server.name}"):
-                            powered_off_servers[server.name] = PoweredOffServer(
-                                time=time.time(),
-                                server=server,
-                                observed_interval=current_interval,
-                            )
-                    powered_off_servers[server.name].server = server
-                    powered_off_servers[
-                        server.name
-                    ].observed_interval = current_interval
-
-                elif server.status == server.STATUS_RUNNING:
-                    if server.name not in [runner.name for runner in runners]:
-                        if server.name not in zombie_servers:
-                            with Action(
-                                f"Found new potential zombie server {server.name}"
-                            ):
-                                zombie_servers[server.name] = ZombieServer(
+        try:
+            with Action("Getting list of servers", level=logging.DEBUG):
+                servers: list[BoundServer] = client.servers.get_all()
+                servers = [
+                    server
+                    for server in servers
+                    if server.name.startswith(server_name_prefix)
+                ]
+
+            with Action("Getting list of self-hosted runners", level=logging.DEBUG):
+                runners: list[SelfHostedActionsRunner] = repo.get_self_hosted_runners()
+
+            with Action(
+                "Looking for powered off or zombie servers", level=logging.DEBUG
+            ):
+                for server in servers:
+                    if server.status == server.STATUS_OFF:
+                        if server.name not in powered_off_servers:
+                            with Action(f"Found new powered off server {server.name}"):
+                                powered_off_servers[server.name] = PoweredOffServer(
                                     time=time.time(),
                                     server=server,
                                     observed_interval=current_interval,
                                 )
-                        zombie_servers[server.name].server = server
-                        zombie_servers[server.name].observed_interval = current_interval
-
-                    else:
-                        zombie_servers.pop(server.name, None)
+                        powered_off_servers[server.name].server = server
+                        powered_off_servers[
+                            server.name
+                        ].observed_interval = current_interval
+
+                    elif server.status == server.STATUS_RUNNING:
+                        if server.name not in [runner.name for runner in runners]:
+                            if server.name not in zombie_servers:
+                                with Action(
+                                    f"Found new potential zombie server {server.name}"
+                                ):
+                                    zombie_servers[server.name] = ZombieServer(
+                                        time=time.time(),
+                                        server=server,
+                                        observed_interval=current_interval,
+                                    )
+                            zombie_servers[server.name].server = server
+                            zombie_servers[
+                                server.name
+                            ].observed_interval = current_interval
+
+                        else:
+                            zombie_servers.pop(server.name, None)
+
+            with Action("Looking for idle runners", level=logging.DEBUG):
+                for runner in runners:
+                    if runner.status == "online" and not runner.busy:
+                        if (
+                            runner.name.startswith(runner_name_prefix)
+                            and runner.name not in idle_runners
+                        ):
+                            with Action(f"Found new idle runner {runner.name}"):
+                                idle_runners[runner.name] = IdleRunner(
+                                    time=time.time(),
+                                    runner=runner,
+                                    observed_interval=current_interval,
+                                )
+                        idle_runners[runner.name].runner = runner
+                        idle_runners[runner.name].observed_interval = current_interval
 
-        with Action("Looking for idle runners", level=logging.DEBUG):
-            for runner in runners:
-                if runner.status == "online" and not runner.busy:
-                    if (
-                        runner.name.startswith(runner_name_prefix)
-                        and runner.name not in idle_runners
-                    ):
-                        with Action(f"Found new idle runner {runner.name}"):
-                            idle_runners[runner.name] = IdleRunner(
-                                time=time.time(),
-                                runner=runner,
-                                observed_interval=current_interval,
-                            )
-                    idle_runners[runner.name].runner = runner
-                    idle_runners[runner.name].observed_interval = current_interval
-
-        with Action(
-            "Checking which powered off servers need to be deleted", level=logging.DEBUG
-        ):
-            for server_name in list(powered_off_servers.keys()):
-                powered_off_server = powered_off_servers[server_name]
-
-                if powered_off_server.observed_interval != current_interval:
-                    with Action(f"Forgetting about powered off server {server.name}"):
-                        powered_off_servers.pop(server_name)
+            with Action(
+                "Checking which powered off servers need to be deleted",
+                level=logging.DEBUG,
+            ):
+                for server_name in list(powered_off_servers.keys()):
+                    powered_off_server = powered_off_servers[server_name]
 
-                else:
-                    if time.time() - powered_off_server.time > max_powered_off_time:
+                    if powered_off_server.observed_interval != current_interval:
                         with Action(
-                            f"Deleting powered off server {server_name}",
-                            ignore_fail=True,
-                        ) as action:
-                            powered_off_server.server.delete()
+                            f"Forgetting about powered off server {server.name}"
+                        ):
                             powered_off_servers.pop(server_name)
 
-        with Action(
-            "Checking which zombie servers need to be deleted", level=logging.DEBUG
-        ):
-            for server_name in list(zombie_servers.keys()):
-                zombie_server = zombie_servers[server_name]
-
-                if zombie_server.observed_interval != current_interval:
-                    with Action(f"Forgetting about zombie server {server.name}"):
-                        zombie_servers.pop(server_name)
+                    else:
+                        if time.time() - powered_off_server.time > max_powered_off_time:
+                            with Action(
+                                f"Deleting powered off server {server_name}",
+                                ignore_fail=True,
+                            ) as action:
+                                powered_off_server.server.delete()
+                                powered_off_servers.pop(server_name)
+
+            with Action(
+                "Checking which zombie servers need to be deleted", level=logging.DEBUG
+            ):
+                for server_name in list(zombie_servers.keys()):
+                    zombie_server = zombie_servers[server_name]
 
-                else:
-                    if time.time() - zombie_server.time > max_runner_registration_time:
-                        with Action(
-                            f"Deleting zombie server {server_name}",
-                            ignore_fail=True,
-                        ) as action:
-                            zombie_server.server.delete()
+                    if zombie_server.observed_interval != current_interval:
+                        with Action(f"Forgetting about zombie server {server.name}"):
                             zombie_servers.pop(server_name)
 
-        with Action(
-            "Checking which idle runners need to be removed and their servers deleted",
-            level=logging.DEBUG,
-        ):
-
-            for idle_runner_name in list(idle_runners.keys()):
-                idle_runner = idle_runners[idle_runner_name]
-
-                if idle_runner.observed_interval != current_interval:
-                    with Action(f"Forgetting about idle runner {idle_runner_name}"):
-                        idle_runners.pop(idle_runner_name)
-
-                else:
-                    if time.time() - idle_runner.time > max_idle_runner_time:
-                        runner_server = None
-
-                        with Action(
-                            f"Try to find server for the runner {idle_runner_name}",
-                            ignore_fail=True,
+                    else:
+                        if (
+                            time.time() - zombie_server.time
+                            > max_runner_registration_time
                         ):
-                            runner_server = client.servers.get_by_name(idle_runner_name)
-
-                        if runner_server is not None:
                             with Action(
-                                f"Deleting idle runner server {runner_server.name}",
+                                f"Deleting zombie server {server_name}",
                                 ignore_fail=True,
-                            ):
-                                runner_server.delete()
-                                runner_server = None
+                            ) as action:
+                                zombie_server.server.delete()
+                                zombie_servers.pop(server_name)
+
+            with Action(
+                "Checking which idle runners need to be removed and their servers deleted",
+                level=logging.DEBUG,
+            ):
+
+                for idle_runner_name in list(idle_runners.keys()):
+                    idle_runner = idle_runners[idle_runner_name]
+
+                    if idle_runner.observed_interval != current_interval:
+                        with Action(f"Forgetting about idle runner {idle_runner_name}"):
+                            idle_runners.pop(idle_runner_name)
+
+                    else:
+                        if time.time() - idle_runner.time > max_idle_runner_time:
+                            runner_server = None
 
-                        if runner_server is None:
                             with Action(
-                                f"Removing self-hosted runner {idle_runner_name}",
+                                f"Try to find server for the runner {idle_runner_name}",
                                 ignore_fail=True,
                             ):
-                                repo.remove_self_hosted_runner(idle_runner.runner)
+                                runner_server = client.servers.get_by_name(
+                                    idle_runner_name
+                                )
+
+                            if runner_server is not None:
+                                with Action(
+                                    f"Deleting idle runner server {runner_server.name}",
+                                    ignore_fail=True,
+                                ):
+                                    runner_server.delete()
+                                    runner_server = None
+
+                            if runner_server is None:
+                                with Action(
+                                    f"Removing self-hosted runner {idle_runner_name}",
+                                    ignore_fail=True,
+                                ):
+                                    repo.remove_self_hosted_runner(idle_runner.runner)
+        except Exception as exc:
+            msg = f"❗ Error: {type(exc).__name__} {exc}"
+            if debug:
+                logger.exception(f"{msg}\n{exc}")
+            else:
+                logger.error(msg)
 
         with Action(f"Sleeping until next interval {interval}s", level=logging.DEBUG):
             time.sleep(interval)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scale_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import logging
 import threading
 
 from .actions import Action
 from .scripts import Scripts
 from .request import request
 from .args import image_type, check_image
+from .logger import logger
 
 from .server import wait_ssh, ssh, wait_ready
 
 from hcloud import Client, APIException
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.locations.domain import Location
@@ -205,98 +206,109 @@
     ssh_key: SSHKey,
     default_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
     max_server_ready_time: int,
+    debug: bool = False,
 ):
     """Scale up service."""
 
     with ThreadPoolExecutor(
         max_workers=worker_pool._max_workers, thread_name_prefix=f"setup-worker"
     ) as setup_worker_pool:
 
         while True:
             if terminate.is_set():
                 with Action("Terminating scale up service"):
                     break
 
-            with Action("Getting workflow runs", level=logging.DEBUG):
-                workflow_runs = repo.get_workflow_runs(branch="main", status="queued")
+            try:
+                with Action("Getting workflow runs", level=logging.DEBUG):
+                    workflow_runs = repo.get_workflow_runs(
+                        branch="main", status="queued"
+                    )
+
+                futures: list[Future] = []
+
+                with Action("Looking for jobs", level=logging.DEBUG) as action:
+                    for run in workflow_runs:
+                        for job in run.jobs():
+                            with Action("Getting list of servers", level=logging.DEBUG):
+                                servers: list[BoundServer] = client.servers.get_all()
+                                servers = [
+                                    server
+                                    for server in servers
+                                    if server.name.startswith(server_name_prefix)
+                                ]
+
+                            server_name = f"{server_name_prefix}{job.run_id}-{job.id}"
+
+                            if job.status != "completed":
+                                if server_name in [server.name for server in servers]:
+                                    with Action(
+                                        f"Server already exists for {job.status} {job}",
+                                        level=logging.DEBUG,
+                                    ):
+                                        continue
 
-            futures: list[Future] = []
-
-            with Action("Looking for jobs", level=logging.DEBUG) as action:
-                for run in workflow_runs:
-                    for job in run.jobs():
-                        with Action("Getting list of servers", level=logging.DEBUG):
-                            servers: list[BoundServer] = client.servers.get_all()
-                            servers = [
-                                server
-                                for server in servers
-                                if server.name.startswith(server_name_prefix)
-                            ]
-
-                        server_name = f"{server_name_prefix}{job.run_id}-{job.id}"
-
-                        if job.status != "completed":
-                            if server_name in [server.name for server in servers]:
                                 with Action(
-                                    f"Server already exists for {job.status} {job}",
-                                    level=logging.DEBUG,
+                                    f"Found job for which server was not created {job}"
                                 ):
-                                    continue
-
-                            with Action(
-                                f"Found job for which server was not created {job}"
-                            ):
-                                server_type = get_server_type(
-                                    job=job, default=default_type
-                                )
-                                server_location = get_server_location(
-                                    job=job, default=default_location
-                                )
-                                server_image = get_server_image(
-                                    client=client, job=job, default=default_image
-                                )
-                                startup_script = get_startup_script(
-                                    server_type=server_type, scripts=scripts
-                                )
-
-                                if max_servers is not None:
-                                    if len(servers) >= max_servers:
-                                        with Action(
-                                            f"Maximum number of servers {max_servers} has been reached"
-                                        ):
-                                            break
-
-                                futures.append(
-                                    worker_pool.submit(
-                                        create_server,
-                                        setup_worker_pool=setup_worker_pool,
-                                        client=client,
-                                        job=job,
-                                        name=server_name,
-                                        server_type=server_type,
-                                        server_location=server_location,
-                                        server_image=server_image,
-                                        setup_script=scripts.setup,
-                                        startup_script=startup_script,
-                                        github_token=github_token,
-                                        github_repository=github_repository,
-                                        ssh_key=ssh_key,
-                                        timeout=max_server_ready_time,
+                                    server_type = get_server_type(
+                                        job=job, default=default_type
+                                    )
+                                    server_location = get_server_location(
+                                        job=job, default=default_location
+                                    )
+                                    server_image = get_server_image(
+                                        client=client, job=job, default=default_image
+                                    )
+                                    startup_script = get_startup_script(
+                                        server_type=server_type, scripts=scripts
                                     )
-                                )
-                    else:
-                        continue
-                    break
 
-            for future in futures:
-                with Action("Waiting to finish creating servers", ignore_fail=True):
-                    future.result()
+                                    if max_servers is not None:
+                                        if len(servers) >= max_servers:
+                                            with Action(
+                                                f"Maximum number of servers {max_servers} has been reached"
+                                            ):
+                                                break
+
+                                    futures.append(
+                                        worker_pool.submit(
+                                            create_server,
+                                            setup_worker_pool=setup_worker_pool,
+                                            client=client,
+                                            job=job,
+                                            name=server_name,
+                                            server_type=server_type,
+                                            server_location=server_location,
+                                            server_image=server_image,
+                                            setup_script=scripts.setup,
+                                            startup_script=startup_script,
+                                            github_token=github_token,
+                                            github_repository=github_repository,
+                                            ssh_key=ssh_key,
+                                            timeout=max_server_ready_time,
+                                        )
+                                    )
+                        else:
+                            continue
+                        break
+
+                for future in futures:
+                    with Action("Waiting to finish creating servers", ignore_fail=True):
+                        future.result()
+
+            except Exception as exc:
+                msg = f"❗ Error: {type(exc).__name__} {exc}"
+                if debug:
+                    logger.exception(f"{msg}\n{exc}")
+                else:
+                    logger.error(msg)
 
             with Action(
                 f"Sleeping until next interval {interval}s", level=logging.DEBUG
             ):
                 time.sleep(interval)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230728.1122057/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1031109
+Version: 1.2.230728.1122057
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230728.1031109/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230728.1122057/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 testflows.github.runners.egg-info/not-zip-safe
 testflows.github.runners.egg-info/requires.txt
 testflows.github.runners.egg-info/top_level.txt
 testflows/github/runners/__init__.py
 testflows/github/runners/actions.py
 testflows/github/runners/args.py
 testflows/github/runners/cloud.py
+testflows/github/runners/logger.py
 testflows/github/runners/request.py
 testflows/github/runners/scale_down.py
 testflows/github/runners/scale_up.py
 testflows/github/runners/server.py
 testflows/github/runners/service.py
 testflows/github/runners/shell.py
 testflows/github/runners/bin/github-runners
```

