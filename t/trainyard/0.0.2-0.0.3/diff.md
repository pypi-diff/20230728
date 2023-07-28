# Comparing `tmp/trainyard-0.0.2.tar.gz` & `tmp/trainyard-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainyard-0.0.2.tar", last modified: Thu Jul 27 23:54:59 2023, max compression
+gzip compressed data, was "trainyard-0.0.3.tar", last modified: Fri Jul 28 06:10:03 2023, max compression
```

## Comparing `trainyard-0.0.2.tar` & `trainyard-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.465172 trainyard-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 23:54:46.000000 trainyard-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 23:54:59.465172 trainyard-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 23:54:46.000000 trainyard-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 23:54:46.000000 trainyard-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:54:59.465172 trainyard-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 23:54:46.000000 trainyard-0.0.2/tests/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/runhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/engine_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine_v2/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/engine_v2/runhouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/tasks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.465172 trainyard-0.0.2/trainyard/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/trainer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.465172 trainyard-0.0.2/trainyard/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/workflow/prefect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 23:54:46.000000 trainyard-0.0.2/trainyard/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:54:59.461172 trainyard-0.0.2/trainyard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:54:59.000000 trainyard-0.0.2/trainyard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 06:09:47.000000 trainyard-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 06:10:03.272024 trainyard-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 06:09:47.000000 trainyard-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-28 06:09:47.000000 trainyard-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 06:10:03.272024 trainyard-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.268024 trainyard-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-28 06:09:47.000000 trainyard-0.0.3/tests/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.268024 trainyard-0.0.3/trainyard/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/trainyard/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine/runhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/trainyard/engine_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine_v2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/engine_v2/runhouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/trainyard/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/trainyard/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/trainer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/trainyard/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/workflow/prefect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-28 06:09:47.000000 trainyard-0.0.3/trainyard/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:10:03.272024 trainyard-0.0.3/trainyard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 06:10:03.000000 trainyard-0.0.3/trainyard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-28 06:10:03.000000 trainyard-0.0.3/trainyard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:10:03.000000 trainyard-0.0.3/trainyard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 06:10:03.000000 trainyard-0.0.3/trainyard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 06:10:03.000000 trainyard-0.0.3/trainyard.egg-info/top_level.txt
```

### Comparing `trainyard-0.0.2/LICENSE` & `trainyard-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/tests/test_cluster.py` & `trainyard-0.0.3/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/__init__.py` & `trainyard-0.0.3/trainyard/__init__.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/engine/__init__.py` & `trainyard-0.0.3/trainyard/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/engine/cluster.py` & `trainyard-0.0.3/trainyard/engine/cluster.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/engine/local.py` & `trainyard-0.0.3/trainyard/engine/local.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/engine/runhouse.py` & `trainyard-0.0.3/trainyard/engine/runhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         """
         Creates a runhouse cluster with args. For a full list: https://runhouse-docs.readthedocs-hosted.com/en/latest/_modules/runhouse/rns/hardware/cluster_factory.html#cluster
         """
         super().__init__(name, instance_type)
         self.cluster = create_runhouse_cluster(
             name=name, instance_type=instance_type, **kwargs
         )
+        if not self.cluster.is_up():
+            self.start()
 
     def install_packages(self, packages: List[str]) -> None:
         rh_packages = []
         for package in packages:
             rh_packages.append(package)
         self.cluster.install_packages(rh_packages)
 
@@ -135,14 +137,15 @@
         Returns:
             Any: object in the object store
         """
         return self.cluster.get(key, *args, **kwargs)
 
     def start(self) -> RunhouseCluster:
         self.cluster.up_if_not()
+        self.cluster.install_packages(["trainyard"])
         return self
 
     def teardown(self) -> None:
         # replace this with `teardown_and_delete` when it works
         self.cluster.teardown()
         self.cluster.unname()
```

### Comparing `trainyard-0.0.2/trainyard/engine/utils.py` & `trainyard-0.0.3/trainyard/engine/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     name: Optional[str] = None,
     instance_type: Optional[str] = None,
     **kwargs,
 ):
     if name is None:
         name = "".join(random.choice(string.lowercase) for x in range(10))
         name = f"{backend}-cluster-{name}"
-    if instance_type is None:
-        return LocalCluster(name=name, **kwargs)
     cluster_class = CLUSTER_MAP.get(backend, RunhouseCluster)
     return cluster_class(name, instance_type, **kwargs)
 
 
 class ClusterSpec:
     def __init__(
         self, name: Optional[str] = None, instance_type: Optional[str] = None, **kwargs
```

### Comparing `trainyard-0.0.2/trainyard/engine_v2/engine.py` & `trainyard-0.0.3/trainyard/engine_v2/engine.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/engine_v2/runhouse.py` & `trainyard-0.0.3/trainyard/engine_v2/runhouse.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/tasks/tasks.py` & `trainyard-0.0.3/trainyard/tasks/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             return task
         task.options = task.options.merge(**kwargs)
         return task
 
     return dec
 
 
-def run_fn(_task, *args, **kwargs):
+def run_fn(*args, _task=None, **kwargs):
     return _task(*args, **kwargs)
 
 
 class Task(metaclass=abc.ABCMeta):
     options: TaskOptions = TaskOptions()
 
     def __init__(
```

### Comparing `trainyard-0.0.2/trainyard/track.py` & `trainyard-0.0.3/trainyard/track.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/trainer/base.py` & `trainyard-0.0.3/trainyard/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard/workflow/prefect.py` & `trainyard-0.0.3/trainyard/workflow/prefect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Any, Callable, Dict
 
-import prefect
-
 from trainyard.tasks.tasks import Task, TaskWrapper
 from trainyard.workflow.workflow import WorkflowBackend
 
+try:
+    import prefect
+except Exception:
+    pass
+
 
 class PrefectTaskWrapper(TaskWrapper):
     def wrap(self, f: Callable[[Any], Any], task: Task) -> Callable[[Any], Any]:
         return prefect.task(
             name=task.name, description=task.options.description, refresh_cache=True
         )(f)
 
@@ -16,11 +19,9 @@
 class PrefectWorkflowBackend(WorkflowBackend):
     def __init__(self, workflow_params: Dict[str, Any] = {}):
         self.workflow_params = workflow_params
 
     def setup_task_wrapper(self):
         return PrefectTaskWrapper()
 
-    def create_workflow(
-        self, name: str, workflow_function: Callable[[Any], Any]
-    ) -> prefect.Flow:
+    def create_workflow(self, name: str, workflow_function: Callable[[Any], Any]):
         return prefect.flow(name=name, **self.workflow_params)(workflow_function)
```

### Comparing `trainyard-0.0.2/trainyard/workflow/workflow.py` & `trainyard-0.0.3/trainyard/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.2/trainyard.egg-info/SOURCES.txt` & `trainyard-0.0.3/trainyard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

