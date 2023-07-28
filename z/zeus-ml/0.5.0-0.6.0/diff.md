# Comparing `tmp/zeus-ml-0.5.0.tar.gz` & `tmp/zeus-ml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus-ml-0.5.0.tar", last modified: Wed Jul 12 03:12:38 2023, max compression
+gzip compressed data, was "zeus-ml-0.6.0.tar", last modified: Fri Jul 28 20:53:57 2023, max compression
```

## Comparing `zeus-ml-0.5.0.tar` & `zeus-ml-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.948215 zeus-ml-0.5.0/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/optimizer/power_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/policy/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/mab.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/run/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49008 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/run/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/run/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/util/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/lr_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/zeus_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/optimizer/power_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49008 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/run/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/run/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/lr_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/top_level.txt
```

### Comparing `zeus-ml-0.5.0/LICENSE` & `zeus-ml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.5.0/PKG-INFO` & `zeus-ml-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.5.0
+Version: 0.6.0
 Summary: A framework for deep learning energy measurement and optimization.
 Home-page: https://github.com/SymbioticLab/Zeus
 Author: Jae-Won Chung
 Author-email: jwnchung@umich.edu
 License: Apache-2.0
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,sustainability,mlsys
@@ -25,32 +25,32 @@
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="docs/assets/img/logo_light.svg">
   <img alt="Zeus logo" width="55%" src="docs/assets/img/logo_dark.svg">
 </picture>
-<h1>A Framework for Deep Learning Energy Measurement and Optimization</h1>
+<h1>Deep Learning Energy Measurement and Optimization</h1>
 </div>
 
 [![NSDI23 paper](https://custom-icon-badges.herokuapp.com/badge/NSDI'23-paper-b31b1b.svg)](https://www.usenix.org/conference/nsdi23/presentation/you)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/611f69?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Homepage build](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml/badge.svg)](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/SymbioticLab/Zeus?logo=law)](/LICENSE)
 
 ---
-**Latest News** ⚡ 
+**Project News** ⚡ 
 
 - \[2023/07\] [`ZeusMonitor`](https://ml.energy/zeus/reference/monitor/#zeus.monitor.ZeusMonitor) was used to profile GPU time and energy consumption for the [ML.ENERGY leaderboard](https://ml.energy/leaderboard).
 - \[2023/03\] [Chase](https://symbioticlab.org/publications/files/chase:ccai23/chase-ccai23.pdf), an automatic carbon optimization framework for DNN training, will appear at ICLR'23 workshop.
 - \[2022/11\] [Carbon-Aware Zeus](https://taikai.network/gsf/hackathons/carbonhack22/projects/cl95qxjpa70555701uhg96r0ek6/idea) won the **second overall best solution award** at Carbon Hack 22.
 ---
 
-Zeus is a general framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
+Zeus is a framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
 
 ### Measuring GPU energy
 
 ```python
 from zeus.monitor import ZeusMonitor
 
 monitor = ZeusMonitor(gpu_indices=[0,1,2,3])
@@ -123,17 +123,17 @@
 ### Docker image
 
 We provide a Docker image fully equipped with all dependencies and environments.
 The only command you need is:
 
 ```sh
 docker run -it \
-    --gpus 1                    `# Mount one GPU` \
+    --gpus all                  `# Mount all GPUs` \
     --cap-add SYS_ADMIN         `# Needed to change the power limit of the GPU` \
-    --shm-size 64G              `# PyTorch DataLoader workers need enough shm` \
+    --ipc host                  `# PyTorch DataLoader workers need enough shm` \
     symbioticlab/zeus:latest \
     bash
 ```
 
 Refer to [Environment setup](https://ml.energy/zeus/getting_started/environment/) for details.
 
 ### Examples
```

### Comparing `zeus-ml-0.5.0/README.md` & `zeus-ml-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="docs/assets/img/logo_light.svg">
   <img alt="Zeus logo" width="55%" src="docs/assets/img/logo_dark.svg">
 </picture>
-<h1>A Framework for Deep Learning Energy Measurement and Optimization</h1>
+<h1>Deep Learning Energy Measurement and Optimization</h1>
 </div>
 
 [![NSDI23 paper](https://custom-icon-badges.herokuapp.com/badge/NSDI'23-paper-b31b1b.svg)](https://www.usenix.org/conference/nsdi23/presentation/you)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/611f69?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Homepage build](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml/badge.svg)](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/SymbioticLab/Zeus?logo=law)](/LICENSE)
 
 ---
-**Latest News** ⚡ 
+**Project News** ⚡ 
 
 - \[2023/07\] [`ZeusMonitor`](https://ml.energy/zeus/reference/monitor/#zeus.monitor.ZeusMonitor) was used to profile GPU time and energy consumption for the [ML.ENERGY leaderboard](https://ml.energy/leaderboard).
 - \[2023/03\] [Chase](https://symbioticlab.org/publications/files/chase:ccai23/chase-ccai23.pdf), an automatic carbon optimization framework for DNN training, will appear at ICLR'23 workshop.
 - \[2022/11\] [Carbon-Aware Zeus](https://taikai.network/gsf/hackathons/carbonhack22/projects/cl95qxjpa70555701uhg96r0ek6/idea) won the **second overall best solution award** at Carbon Hack 22.
 ---
 
-Zeus is a general framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
+Zeus is a framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
 
 ### Measuring GPU energy
 
 ```python
 from zeus.monitor import ZeusMonitor
 
 monitor = ZeusMonitor(gpu_indices=[0,1,2,3])
@@ -98,17 +98,17 @@
 ### Docker image
 
 We provide a Docker image fully equipped with all dependencies and environments.
 The only command you need is:
 
 ```sh
 docker run -it \
-    --gpus 1                    `# Mount one GPU` \
+    --gpus all                  `# Mount all GPUs` \
     --cap-add SYS_ADMIN         `# Needed to change the power limit of the GPU` \
-    --shm-size 64G              `# PyTorch DataLoader workers need enough shm` \
+    --ipc host                  `# PyTorch DataLoader workers need enough shm` \
     symbioticlab/zeus:latest \
     bash
 ```
 
 Refer to [Environment setup](https://ml.energy/zeus/getting_started/environment/) for details.
 
 ### Examples
```

### Comparing `zeus-ml-0.5.0/pyproject.toml` & `zeus-ml-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 ]
 ignore = [
   "PLW0603",  # Global statement
   "B019",     # Usage of functools.lru_cache
   "PLR0913",  # Too many function arguments
   "B905",     # zip strict argument
   "PLR0915",  # Too many statements
+  "PLR2004",  # Magic values
+  "SIM115",   # Context manager for opening files
+  "E501",     # Line too long
 ]
 line-length = 120
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
```

### Comparing `zeus-ml-0.5.0/setup.py` & `zeus-ml-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # 
 #     http://www.apache.org/licenses/LICENSE-2.0
 # 
@@ -19,15 +19,15 @@
     "test": ["pytest==7.3.2", "pytest-mock==3.10.0", "pytest-xdist==3.3.1"],
     "torch": ["torch==2.0.1"],
 }
 extras_require["dev"] = extras_require["lint"] + extras_require["test"] + extras_require["torch"]
 
 setup(
     name="zeus-ml",
-    version="0.5.0",
+    version="0.6.0",
     description="A framework for deep learning energy measurement and optimization.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SymbioticLab/Zeus",
     author="Jae-Won Chung",
     author_email="jwnchung@umich.edu",
     license="Apache-2.0",
@@ -44,12 +44,13 @@
         "Documentation": "https://ml.energy/zeus",
     },
     packages=find_packages("."),
     install_requires=[
         "numpy",
         "pandas",
         "scikit-learn",
-        "pynvml",
+        "nvidia-ml-py",
+        "pydantic",
     ],
     python_requires=">=3.8",
     extras_require=extras_require,
 )
```

### Comparing `zeus-ml-0.5.0/zeus/__init__.py` & `zeus-ml-0.6.0/zeus/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/analyze.py` & `zeus-ml-0.6.0/zeus/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/callback.py` & `zeus-ml-0.6.0/zeus/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/controller.py` & `zeus-ml-0.6.0/zeus/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/job.py` & `zeus-ml-0.6.0/zeus/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/monitor.py` & `zeus-ml-0.6.0/zeus/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -155,15 +155,15 @@
         # Initialize loggers.
         self.logger = get_logger(type(self).__name__)
         if log_file is None:
             self.log_file = None
         else:
             if dir := os.path.dirname(log_file):
                 os.makedirs(dir, exist_ok=True)
-            self.log_file = open(log_file, "w")  # ruff: noqa: SIM115
+            self.log_file = open(log_file, "w")
             self.logger.info("Writing measurement logs to %s.", log_file)
             self.log_file.write(
                 f"start_time,window_name,elapsed_time,{','.join(map(lambda i: f'gpu{i}_energy', self.gpu_indices))}\n",
             )
             self.log_file.flush()
 
         self.logger.info("Monitoring GPU %s.", self.gpu_indices)
```

### Comparing `zeus-ml-0.5.0/zeus/optimizer/__init__.py` & `zeus-ml-0.6.0/zeus/optimizer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/policy/__init__.py` & `zeus-ml-0.6.0/zeus/policy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/policy/interface.py` & `zeus-ml-0.6.0/zeus/policy/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/policy/mab.py` & `zeus-ml-0.6.0/zeus/policy/mab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/policy/optimizer.py` & `zeus-ml-0.6.0/zeus/policy/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/run/__init__.py` & `zeus-ml-0.6.0/zeus/run/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/run/dataloader.py` & `zeus-ml-0.6.0/zeus/run/dataloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/run/master.py` & `zeus-ml-0.6.0/zeus/run/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/simulate.py` & `zeus-ml-0.6.0/zeus/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/util/__init__.py` & `zeus-ml-0.6.0/zeus/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/util/check.py` & `zeus-ml-0.6.0/zeus/util/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/util/framework.py` & `zeus-ml-0.6.0/zeus/util/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/util/logging.py` & `zeus-ml-0.6.0/zeus/util/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,15 +20,15 @@
 
 
 class FileAndConsole:
     """Like tee, but for Python prints."""
 
     def __init__(self, filepath: Path) -> None:
         """Initialize the object."""
-        self.file = open(filepath, "w")  # ruff: noqa: SIM115
+        self.file = open(filepath, "w")
         self.stdout = sys.stdout
 
     def write(self, message):
         """Write message."""
         self.file.write(message)
         self.stdout.write(message)
         self.file.flush()
```

### Comparing `zeus-ml-0.5.0/zeus/util/lr_scaler.py` & `zeus-ml-0.6.0/zeus/util/lr_scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/util/metric.py` & `zeus-ml-0.6.0/zeus/util/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `zeus-ml-0.5.0/zeus/util/testing.py` & `zeus-ml-0.6.0/zeus/util/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Jae-Won Chung <jwnchung@umich.edu>
+# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -65,15 +65,15 @@
             ignore_sync_cuda: Whether to ignore `sync_cuda` calls. (Default: `False`)
             match_window_name: Whether to make sure window names match. (Default: `True`)
         """
         if log_file is None:
             raise ValueError("`log_file` cannot be `None` for `ReplayZeusMonitor`.")
 
         self.monitor_exec = monitor_exec
-        self.log_file = open(log_file)  # ruff: noqa: SIM115
+        self.log_file = open(log_file)
         self.ignore_sync_cuda = ignore_sync_cuda
         self.match_window_name = match_window_name
 
         # Infer GPU indices from the log file if not provided.
         header = self.log_file.readline()
         if gpu_indices is None:
             gpu_indices = [
```

### Comparing `zeus-ml-0.5.0/zeus_ml.egg-info/PKG-INFO` & `zeus-ml-0.6.0/zeus_ml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.5.0
+Version: 0.6.0
 Summary: A framework for deep learning energy measurement and optimization.
 Home-page: https://github.com/SymbioticLab/Zeus
 Author: Jae-Won Chung
 Author-email: jwnchung@umich.edu
 License: Apache-2.0
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,sustainability,mlsys
@@ -25,32 +25,32 @@
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="docs/assets/img/logo_light.svg">
   <img alt="Zeus logo" width="55%" src="docs/assets/img/logo_dark.svg">
 </picture>
-<h1>A Framework for Deep Learning Energy Measurement and Optimization</h1>
+<h1>Deep Learning Energy Measurement and Optimization</h1>
 </div>
 
 [![NSDI23 paper](https://custom-icon-badges.herokuapp.com/badge/NSDI'23-paper-b31b1b.svg)](https://www.usenix.org/conference/nsdi23/presentation/you)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/611f69?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Homepage build](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml/badge.svg)](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/SymbioticLab/Zeus?logo=law)](/LICENSE)
 
 ---
-**Latest News** ⚡ 
+**Project News** ⚡ 
 
 - \[2023/07\] [`ZeusMonitor`](https://ml.energy/zeus/reference/monitor/#zeus.monitor.ZeusMonitor) was used to profile GPU time and energy consumption for the [ML.ENERGY leaderboard](https://ml.energy/leaderboard).
 - \[2023/03\] [Chase](https://symbioticlab.org/publications/files/chase:ccai23/chase-ccai23.pdf), an automatic carbon optimization framework for DNN training, will appear at ICLR'23 workshop.
 - \[2022/11\] [Carbon-Aware Zeus](https://taikai.network/gsf/hackathons/carbonhack22/projects/cl95qxjpa70555701uhg96r0ek6/idea) won the **second overall best solution award** at Carbon Hack 22.
 ---
 
-Zeus is a general framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
+Zeus is a framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
 
 ### Measuring GPU energy
 
 ```python
 from zeus.monitor import ZeusMonitor
 
 monitor = ZeusMonitor(gpu_indices=[0,1,2,3])
@@ -123,17 +123,17 @@
 ### Docker image
 
 We provide a Docker image fully equipped with all dependencies and environments.
 The only command you need is:
 
 ```sh
 docker run -it \
-    --gpus 1                    `# Mount one GPU` \
+    --gpus all                  `# Mount all GPUs` \
     --cap-add SYS_ADMIN         `# Needed to change the power limit of the GPU` \
-    --shm-size 64G              `# PyTorch DataLoader workers need enough shm` \
+    --ipc host                  `# PyTorch DataLoader workers need enough shm` \
     symbioticlab/zeus:latest \
     bash
 ```
 
 Refer to [Environment setup](https://ml.energy/zeus/getting_started/environment/) for details.
 
 ### Examples
```

### Comparing `zeus-ml-0.5.0/zeus_ml.egg-info/SOURCES.txt` & `zeus-ml-0.6.0/zeus_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

