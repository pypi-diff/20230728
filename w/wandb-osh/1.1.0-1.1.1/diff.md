# Comparing `tmp/wandb_osh-1.1.0.tar.gz` & `tmp/wandb_osh-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb_osh-1.1.0.tar", last modified: Tue Jul  4 18:17:25 2023, max compression
+gzip compressed data, was "wandb_osh-1.1.1.tar", last modified: Fri Jul 28 19:20:44 2023, max compression
```

## Comparing `wandb_osh-1.1.0.tar` & `wandb_osh-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-04 18:17:25.518096 wandb_osh-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/wandb_osh/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/lightning_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/ray_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/syncer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/wandb_osh/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/util/hash_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/util/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/wandb_osh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_lightning_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_ray_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.107986 wandb_osh-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/src/wandb_osh/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/lightning_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/ray_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/src/wandb_osh/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/util/hash_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/util/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/src/wandb_osh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:20:43.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_lightning_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_ray_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_syncer.py
```

### Comparing `wandb_osh-1.1.0/LICENSE.txt` & `wandb_osh-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/PKG-INFO` & `wandb_osh-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wandb_osh
-Version: 1.1.0
+Version: 1.1.1
 Summary: Trigger wandb offline syncs from a compute node without internet
 Home-page: https://github.com/klieret/wandb-offline-sync-hook
 Author: Kilian Lieret
 Author-email: kilian.lieret@posteo.de
 Maintainer: Kilian Lieret
 Maintainer-email: kilian.lieret@posteo.de
 License: MIT
@@ -28,15 +28,15 @@
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
-[![Python 3.7‒3.11](https://img.shields.io/badge/python-3.7%E2%80%923.11-blue)](https://www.python.org)
+[![Python 3.8‒3.11](https://img.shields.io/badge/python-3.8%E2%80%923.11-blue)](https://www.python.org)
 [![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/klieret/wandb-offline-sync-hook/main.svg)](https://results.pre-commit.ci/latest/github/klieret/wandb-offline-sync-hook/main)
 [![.github/workflows/test.yaml](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml)
 [![link checker](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/check-links.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions)
 [![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://app.codecov.io/github/klieret/wandb-offline-sync-hook)
 [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `wandb_osh-1.1.0/README.md` & `wandb_osh-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
-[![Python 3.7‒3.11](https://img.shields.io/badge/python-3.7%E2%80%923.11-blue)](https://www.python.org)
+[![Python 3.8‒3.11](https://img.shields.io/badge/python-3.8%E2%80%923.11-blue)](https://www.python.org)
 [![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/klieret/wandb-offline-sync-hook/main.svg)](https://results.pre-commit.ci/latest/github/klieret/wandb-offline-sync-hook/main)
 [![.github/workflows/test.yaml](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml)
 [![link checker](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/check-links.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions)
 [![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://app.codecov.io/github/klieret/wandb-offline-sync-hook)
 [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `wandb_osh-1.1.0/setup.cfg` & `wandb_osh-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wandb_osh
-version = 1.1.0
+version = 1.1.1
 description = Trigger wandb offline syncs from a compute node without internet
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klieret/wandb-offline-sync-hook
 author = Kilian Lieret
 author_email = kilian.lieret@posteo.de
 maintainer = Kilian Lieret
```

### Comparing `wandb_osh-1.1.0/setup.py` & `wandb_osh-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/src/wandb_osh/cli.py` & `wandb_osh-1.1.1/src/wandb_osh/cli.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/src/wandb_osh/hooks.py` & `wandb_osh-1.1.1/src/wandb_osh/hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         """
         if logdir is None:
             # run.dir actually points to the `/files` subdirectory of the run,
             # but we need the directory above that.
             logdir = Path(wandb.run.dir).parent.resolve()
         trial_dir = Path(logdir).resolve()
         cmd_fname = hash_id(str(trial_dir)) + ".command"
+        # In case the communication dir was deleted since we initialized this class
+        self.communication_dir.mkdir(parents=True, exist_ok=True)
         command_file = self.communication_dir / cmd_fname
         if command_file.is_file():
             logger.warning(
                 "Syncing not active or too slow: Command %s file still exists",
                 command_file,
             )
         command_file.touch(exist_ok=True)
```

### Comparing `wandb_osh-1.1.0/src/wandb_osh/lightning_hooks.py` & `wandb_osh-1.1.1/src/wandb_osh/lightning_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/src/wandb_osh/ray_hooks.py` & `wandb_osh-1.1.1/src/wandb_osh/ray_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/src/wandb_osh/syncer.py` & `wandb_osh-1.1.1/src/wandb_osh/syncer.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/src/wandb_osh/util/log.py` & `wandb_osh-1.1.1/src/wandb_osh/util/log.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/src/wandb_osh.egg-info/PKG-INFO` & `wandb_osh-1.1.1/src/wandb_osh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wandb-osh
-Version: 1.1.0
+Version: 1.1.1
 Summary: Trigger wandb offline syncs from a compute node without internet
 Home-page: https://github.com/klieret/wandb-offline-sync-hook
 Author: Kilian Lieret
 Author-email: kilian.lieret@posteo.de
 Maintainer: Kilian Lieret
 Maintainer-email: kilian.lieret@posteo.de
 License: MIT
@@ -28,15 +28,15 @@
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
-[![Python 3.7‒3.11](https://img.shields.io/badge/python-3.7%E2%80%923.11-blue)](https://www.python.org)
+[![Python 3.8‒3.11](https://img.shields.io/badge/python-3.8%E2%80%923.11-blue)](https://www.python.org)
 [![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/klieret/wandb-offline-sync-hook/main.svg)](https://results.pre-commit.ci/latest/github/klieret/wandb-offline-sync-hook/main)
 [![.github/workflows/test.yaml](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml)
 [![link checker](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/check-links.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions)
 [![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://app.codecov.io/github/klieret/wandb-offline-sync-hook)
 [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `wandb_osh-1.1.0/src/wandb_osh.egg-info/SOURCES.txt` & `wandb_osh-1.1.1/src/wandb_osh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/tests/test_cli.py` & `wandb_osh-1.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/tests/test_ray_hooks.py` & `wandb_osh-1.1.1/tests/test_ray_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.0/tests/test_syncer.py` & `wandb_osh-1.1.1/tests/test_syncer.py`

 * *Files identical despite different names*

