# Comparing `tmp/trainyard-0.0.1a0.tar.gz` & `tmp/trainyard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainyard-0.0.1a0.tar", last modified: Thu Jul 27 23:51:41 2023, max compression
+gzip compressed data, was "trainyard-0.0.2.tar", last modified: Thu Jul 27 23:54:59 2023, max compression
```

## Comparing `trainyard-0.0.1a0.tar` & `trainyard-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/tests/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/runhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/engine_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine_v2/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine_v2/runhouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/tasks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/trainer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/workflow/prefect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.465172 trainyard-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 23:54:46.000000 trainyard-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 23:54:59.465172 trainyard-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 23:54:46.000000 trainyard-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 23:54:46.000000 trainyard-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:54:59.465172 trainyard-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 23:54:46.000000 trainyard-0.0.2/tests/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/runhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/engine_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine_v2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine_v2/runhouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.465172 trainyard-0.0.2/trainyard/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/trainer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.465172 trainyard-0.0.2/trainyard/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/workflow/prefect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/top_level.txt
```

### Comparing `trainyard-0.0.1a0/LICENSE` & `trainyard-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/tests/test_cluster.py` & `trainyard-0.0.2/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/__init__.py` & `trainyard-0.0.2/trainyard/__init__.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine/__init__.py` & `trainyard-0.0.2/trainyard/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine/cluster.py` & `trainyard-0.0.2/trainyard/engine/cluster.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine/local.py` & `trainyard-0.0.2/trainyard/engine/local.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine/runhouse.py` & `trainyard-0.0.2/trainyard/engine/runhouse.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine/utils.py` & `trainyard-0.0.2/trainyard/engine/utils.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine_v2/engine.py` & `trainyard-0.0.2/trainyard/engine_v2/engine.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/engine_v2/runhouse.py` & `trainyard-0.0.2/trainyard/engine_v2/runhouse.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/tasks/tasks.py` & `trainyard-0.0.2/trainyard/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/track.py` & `trainyard-0.0.2/trainyard/track.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/trainer/base.py` & `trainyard-0.0.2/trainyard/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/workflow/prefect.py` & `trainyard-0.0.2/trainyard/workflow/prefect.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard/workflow/workflow.py` & `trainyard-0.0.2/trainyard/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1a0/trainyard.egg-info/SOURCES.txt` & `trainyard-0.0.2/trainyard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

