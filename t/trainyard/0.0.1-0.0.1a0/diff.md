# Comparing `tmp/trainyard-0.0.1.tar.gz` & `tmp/trainyard-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainyard-0.0.1.tar", last modified: Tue Jul 11 20:04:43 2023, max compression
+gzip compressed data, was "trainyard-0.0.1a0.tar", last modified: Thu Jul 27 23:51:41 2023, max compression
```

## Comparing `trainyard-0.0.1.tar` & `trainyard-0.0.1a0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 20:04:32.000000 trainyard-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 20:04:43.833976 trainyard-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 20:04:32.000000 trainyard-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 20:04:32.000000 trainyard-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:04:43.833976 trainyard-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 20:04:32.000000 trainyard-0.0.1/tests/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/engine/runhouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/tasks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/trainer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/workflow/prefect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 20:04:32.000000 trainyard-0.0.1/trainyard/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:04:43.833976 trainyard-0.0.1/trainyard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 20:04:43.000000 trainyard-0.0.1/trainyard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/tests/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/runhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/engine_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine_v2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/engine_v2/runhouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/trainer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/workflow/prefect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 23:51:28.000000 trainyard-0.0.1a0/trainyard/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:41.286255 trainyard-0.0.1a0/trainyard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:51:41.000000 trainyard-0.0.1a0/trainyard.egg-info/top_level.txt
```

### Comparing `trainyard-0.0.1/LICENSE` & `trainyard-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1/tests/test_cluster.py` & `trainyard-0.0.1a0/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1/trainyard/engine/local.py` & `trainyard-0.0.1a0/trainyard/engine/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,25 +9,25 @@
         self.object_store: Dict[str, Any] = {}
 
     def run(
         self,
         fn: Callable[[Any], Any],
         name: Optional[str],
         *args,
+        packages: Optional[List[str]] = None,
         env_requirements: Optional[Union[List[str], str]] = None,
         resources: Optional[Dict[str, Any]] = None,
         config: Dict[str, Any] = {},
         **kwargs,
     ) -> Tuple[str, Any]:
         """
         Runs a remote function with args & kwargs. The cluster object is also passed into the function
 
         Args:
             fn (Callable[[Any], Any]): callable function
-            function_config (Dict[str, Any]): dictionary config for creating the remote function
 
         Returns:
             Any: name
             Any: function return object(s)
         """
         self.object_store[name] = fn(*args, **kwargs)
         return name, self.object_store[name]
@@ -43,15 +43,15 @@
         Returns:
             str: name of object
         """
         self.object_store[key] = obj
 
     def get(self, key: str, *args, **kwargs) -> Any:
         """
-        Get the result for a given key from the cluster’s local dictionary object store.
+        Get the result for a given key from the cluster's local dictionary object store.
 
         Args:
             key (str): key of the object to get
 
         Returns:
             Any: object retrieved from object store
         """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trainyard-0.0.1/trainyard/engine/runhouse.py` & `trainyard-0.0.1a0/trainyard/engine/runhouse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,58 @@
+from __future__ import annotations
+
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import runhouse as rh
 
-from trainyard.engine.cluster import Cluster
+from trainyard.engine.cluster import Cluster, RemoteObject
+
+
+def create_runhouse_cluster(name: str, instance_type: str, **kwargs):
+    if rh.exists(name, "cluster"):
+        return rh.cluster(name)
+    cluster = rh.cluster(name=name, instance_type=instance_type, **kwargs)
+    cluster.save()
+    return cluster
+
+
+# runhouse needs function to be exposed
+def _run_remote(*args, runnable_fn=None, **kwargs):
+    _args = []
+    for arg in args:
+        _arg = arg
+        if isinstance(_arg, RemoteObject):
+            _arg = _arg.get_result()
+        _args.append(_arg)
+
+    _kwargs = {}
+    for kw in kwargs:
+        _kwargs[kw] = kwargs[kw]
+        if isinstance(_kwargs[kw], RemoteObject):
+            _kwarg = _kwargs[kw].get_result()
+            kwargs[kw] = _kwarg
+    return runnable_fn(*_args, **_kwargs)
 
 
 class RunhouseCluster(Cluster):
-    def __init__(
-        self, name: str = None, instance_type: Optional[str] = None, *args, **kwargs
-    ):
+    def __init__(self, name: str, instance_type: str, **kwargs):
         """
         Creates a runhouse cluster with args. For a full list: https://runhouse-docs.readthedocs-hosted.com/en/latest/_modules/runhouse/rns/hardware/cluster_factory.html#cluster
-
-        Args:
-            name (str): Name of the cluster
-            instance_type (Optional[str], optional): Instance type. This could be a resource (GPU:2) or a type (V100). Defaults to None.
         """
-        self.cluster = rh.OnDemandCluster(
-            name=name, instance_type=instance_type, *args, **kwargs
+        super().__init__(name, instance_type)
+        self.cluster = create_runhouse_cluster(
+            name=name, instance_type=instance_type, **kwargs
         )
 
+    def install_packages(self, packages: List[str]) -> None:
+        rh_packages = []
+        for package in packages:
+            rh_packages.append(package)
+        self.cluster.install_packages(rh_packages)
+
     def system(self, commands: List[str], *args, **kwargs):
         """
         Run bash commands on the cluster.
         For more details: https://runhouse-docs.readthedocs-hosted.com/en/latest/api/python/cluster.html
 
         Args:
             commands (List[str]): commands to run
@@ -31,84 +60,95 @@
         self.cluster.run(commands, *args, **kwargs)
 
     def run(
         self,
         fn: Callable[[Any], Any],
         *args,
         name: Optional[str] = None,
+        packages: Optional[List[str]] = None,
         env_requirements: Optional[Union[List[str], str]] = None,
         resources: Optional[Dict[str, Any]] = None,
-        config: Dict[str, Any] = {},
+        cluster_run_config: Dict[str, Any] = {},
         **kwargs,
     ) -> Tuple[str, Any]:
         """
         Wraps the function in a runhouse.function and automatically attaches it to the runhouse cluster.
         For a full list of Function parameters: https://runhouse-docs.readthedocs-hosted.com/en/latest/api/python/function.html#function-class
 
-
         Args:
             fn (Callable[[Any], Any]): Callable function
             name (str): name of the function
-            requirements (Optional[Union[List[str], str]], optional): requirements of the function. Defaults to None.
+            packages (Optional[List[str]]): Packages to install. Defaults to None
+            env_requirements (Optional[Union[List[str], str]], optional): Environment requirements of the function. Defaults to None.
             resources (Optional[Dict[str, Any]], optional): resources of the function. Optional number (int) of resources needed to run the Function on the Cluster. Keys must be num_cpus and num_gpus. Defaults to None.
-            config (Dict[str, Any], optional): Additional parameters, see https://runhouse-docs.readthedocs-hosted.com/en/latest/api/python/function.html#function-class. Defaults to {}.
+            cluster_run_config (Dict[str, Any], optional): Additional parameters, see https://runhouse-docs.readthedocs-hosted.com/en/latest/api/python/function.html#function-class. Defaults to {}.
 
         Returns:
             str: output name
             Any: function output
         """
+
         self.cluster.up_if_not()
+        if packages is not None:
+            self.install_packages(packages)
+
         remote_fn = rh.function(
-            fn=fn,
+            fn=_run_remote,
             name=name,
             system=self.cluster,
             env=env_requirements,
             resources=resources,
-            **config,
+            **cluster_run_config,
+        )
+        ref = remote_fn.run(*args, runnable_fn=fn, **kwargs)
+        return RemoteObject(
+            name=ref.name,
+            remote_output_ref=ref,
+            cluster=self,
+            cluster_name=self.name,
         )
-        ref = remote_fn.run(*args, **kwargs)
-        return ref.name, ref
 
     def put(self, key: str, obj: Any, *args, **kwargs) -> str:
         """
         https://runhouse-docs.readthedocs-hosted.com/en/latest/_modules/runhouse/rns/hardware/cluster.html#Cluster.put
 
         puts object in object store in cluster
 
         Args:
-            key (str): Put the given object on the cluster’s object store at the given key.
+            key (str): Put the given object on the cluster's object store at the given key.
             obj (Any): _description_
 
         Returns:
             str: _description_
         """
         self.cluster.put(key, obj, *args, **kwargs)
         return key
 
     def get(self, key: str, *args, **kwargs) -> Any:
         """
         https://runhouse-docs.readthedocs-hosted.com/en/latest/_modules/runhouse/rns/hardware/cluster.html#Cluster.get
 
-        Get the result for a given key from the cluster’s object store.
+        Get the result for a given key from the cluster's object store.
 
         Args:
             key (str): key to retrieve from runhouse object store
 
         Returns:
             Any: object in the object store
         """
         return self.cluster.get(key, *args, **kwargs)
 
-    def start(self) -> str:
+    def start(self) -> RunhouseCluster:
         self.cluster.up_if_not()
-        return self.cluster.address
+        return self
 
     def teardown(self) -> None:
-        if getattr(self.cluster, "teardown_and_delete", None) is not None:
-            self.cluster.teardown_and_delete()
+        # replace this with `teardown_and_delete` when it works
+        self.cluster.teardown()
+        self.cluster.unname()
 
     def save_blob(self, name: str, data: Any, *args, **kwargs) -> str:
         """
         Saves a blob of data into a datastore. For full configuration: https://runhouse-docs.readthedocs-hosted.com/en/latest/api/python/blob.html#blob-factory-method
 
         Args:
             name (str): name of the blob to save
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trainyard-0.0.1/trainyard/tasks/tasks.py` & `trainyard-0.0.1a0/trainyard/tasks/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,13 @@
 from __future__ import annotations
 
 import abc
-from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Type, Union
 
-from trainyard.engine import Cluster, LocalCluster
-
-
-@dataclass
-class RemoteObject:
-    name: str
-    remote_output_ref: Optional[Any] = None  # reference to remote output
-    cluster: Optional[Cluster] = None
-
-    def get_result(self) -> Any:
-        if self.cluster is None and self.remote_output_ref is None:
-            raise ValueError("Remote output or cluster must be specified!")
-        if self.remote_output_ref is not None:
-            return self.remote_output_ref
-        return self.cluster.get(self.name)
-
-
-# because runhouse needs module level function to be exposed
-def _run_task(*args, _task=None, **kwargs):
-    return _task(*args, **kwargs)
+from trainyard.engine import Cluster, ClusterSpec, RemoteObject
 
 
 class TaskWrapper:
     def wrap(self, f: Callable[[Any], Any], task: Task) -> Callable[[Any], Any]:
         return f
 
 
@@ -39,118 +19,172 @@
         GLOBAL_TASK_WRAPPER.task_wrapper = task_wrapper
 
     @staticmethod
     def get_task_wrapper():
         return GLOBAL_TASK_WRAPPER.task_wrapper
 
 
-class Task(metaclass=abc.ABCMeta):
+class TaskOptions:
+    """
+    Args:
+        name (str): name of the task
+        packages (Optional[List[str]]): Packages to install for the task. Defaults to None
+        env_requirements (Optional[Union[List[str], str]], optional): List of requirements to install on the remote cluster, or path to the requirements.txt file.  Defaults to None.
+        resources (Optional[Dict[str, Any]], optional): Optional number (int) of resources needed to run the Function on the Cluster. Keys must be num_cpus and num_gpus.. Defaults to None.
+        cluster (ClusterSpec, optional): cluster specification to run on. Defaults to ClusterSpec().
+        cluster_run_config (Dict[str, Any], optional): additional config for building the remote function. Defaults to {}.
+        description (str): Description for the task.
+    """
+
     def __init__(
         self,
-        name: str,
+        packages: Optional[List[str]] = None,
         env_requirements: Optional[Union[List[str], str]] = None,
         resources: Optional[Dict[str, Any]] = None,
-        config: Dict[str, Any] = {},
-        cluster: Cluster = LocalCluster(),
+        cluster: ClusterSpec = ClusterSpec(),
+        cluster_run_config: Dict[str, Any] = {},
         description: str = "",
     ):
+        self.packages = packages
+        self.env_requirements = env_requirements
+        self.resources = resources
+        self.cluster = cluster
+        self.cluster_run_config = cluster_run_config
+        self.description = description
+
+    def merge(self, **kwargs) -> TaskOptions:
+        return self.__class__(**{**self.to_dict(), **kwargs})
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            "packages": self.packages,
+            "env_requirements": self.env_requirements,
+            "resources": self.resources,
+            "cluster": self.cluster,
+            "cluster_run_config": self.cluster_run_config,
+            "description": self.description,
+        }
+
+
+def task_options(options: Optional[TaskOptions] = None, **kwargs) -> Type[Task]:
+    def dec(task):
+        if options is not None:
+            task.options = task.options.merge({**options.to_dict(), **kwargs})
+            return task
+        task.options = task.options.merge(**kwargs)
+        return task
+
+    return dec
+
+
+def run_fn(_task, *args, **kwargs):
+    return _task(*args, **kwargs)
+
+
+class Task(metaclass=abc.ABCMeta):
+    options: TaskOptions = TaskOptions()
+
+    def __init__(
+        self,
+        name: str,
+    ):
         """
         Base Task object. This is the main runnable function for workflows to run
 
         Args:
             name (str): name of the task
+
+        Options:
+            name (str): name of the task
+            packages (Optional[List[str]]): Packages to install for the task. Defaults to None
             env_requirements (Optional[Union[List[str], str]], optional): List of requirements to install on the remote cluster, or path to the requirements.txt file.  Defaults to None.
             resources (Optional[Dict[str, Any]], optional): Optional number (int) of resources needed to run the Function on the Cluster. Keys must be num_cpus and num_gpus.. Defaults to None.
-            config (Dict[str, Any], optional): additional config for building the remote function. Defaults to {}.
-            cluster (Cluster, optional): cluster to run on. Defaults to LocalCluster().
+            cluster (ClusterSpec, optional): cluster specification to run on. Defaults to ClusterSpec().
+            cluster_run_config (Dict[str, Any], optional): additional config for building the remote function. Defaults to {}.
             description (str): Description for the task.
         """
         self.name = name
-        self.env_requirements = env_requirements
-        self.resources = resources
-        self.config = config
-        self.cluster = cluster
-        self.description = description
-        self.dependencies = []
+        self.options = self.__class__.options
+
+    @property
+    def cluster(self) -> Union[ClusterSpec, Cluster]:
+        return self.options.cluster
+
+    @cluster.setter
+    def cluster(self, cluster: Union[ClusterSpec, Cluster]) -> None:
+        self.options.cluster = cluster
 
-    def add_dependency(self, dependency: Task) -> None:
-        self.dependencies.append(dependency)
+    def set_options(self, options: TaskOptions = TaskOptions(), **kwargs) -> None:
+        self.options = options.merge(**kwargs)
 
     def to(self, cluster: Cluster) -> Task:
         self.cluster = cluster
         return self
 
     @abc.abstractmethod
     def __call__(self, *args, **kwargs) -> Any:
         """
         Main function for task.
         """
 
-    def remote(self, *args, **kwargs) -> Any:
-        _args = []
-        for arg in args:
-            _arg = arg
-            if isinstance(arg, RemoteObject):
-                _arg = arg.get_result()
-            _args.append(_arg)
-
-        _kwargs = {}
-        for kw in kwargs:
-            _kwargs[kw] = kwargs[kw]
-            if isinstance(kwargs[kw], RemoteObject):
-                _kwargs[kw] = kwargs[kw].get_result()
+    def remote(
+        self, *args, cluster: Optional[Cluster] = None, **kwargs
+    ) -> RemoteObject:
+        if cluster is None:
+            if isinstance(self.cluster, ClusterSpec):
+                self.cluster = self.cluster.create_cluster()
+            cluster = self.cluster
 
-        name, ref = self.cluster.run(
-            _run_task,
+        remote_output = cluster.run(
+            run_fn,
             name=self.name,
-            env_requirements=self.env_requirements,
-            resources=self.resources,
-            config=self.config,
+            packages=self.options.packages,
+            env_requirements=self.options.env_requirements,
+            resources=self.options.resources,
+            cluster_run_config=self.options.cluster_run_config,
             _task=self,
-            *_args,
-            **_kwargs,
+            *args,
+            **kwargs,
         )
-        remote_output = RemoteObject(name, ref, self.cluster)
         return remote_output
 
-    def run(self, *args, **kwargs) -> Any:
+    def run(self, *args, cluster: Optional[Cluster] = None, **kwargs) -> RemoteObject:
         """
         Runs the function remotely on `self.cluster`
 
         Returns:
             RemoteObject: remote output dataclass containing reference to output
         """
+
         if GLOBAL_TASK_WRAPPER.get_task_wrapper() is None:
-            raise ValueError(
-                "No GLOBAL_TASK_WRAPPER defined! Tasks must be run within context of a workflow"
+            print(
+                "No GLOBAL_TASK_WRAPPER defined! Tasks should be run within context of a workflow"
+            )
+            self._wrapped_fn = self.remote
+        else:
+            self._wrapped_fn = GLOBAL_TASK_WRAPPER.get_task_wrapper().wrap(
+                self.remote, self
             )
-        self._wrapped_fn = GLOBAL_TASK_WRAPPER.get_task_wrapper().wrap(
-            self.remote, self
-        )
 
-        return self._wrapped_fn(*args, **kwargs)
+        return self._wrapped_fn(*args, cluster=cluster, **kwargs)
 
 
 class FunctionTask(Task):
     def __init__(
         self,
-        fn: Callable[[Any], Any],
         name: str,
-        env_requirements: Optional[Union[List[str], str]] = None,
-        resources: Optional[Dict[str, Any]] = None,
-        config: Dict[str, Any] = {},
-        cluster: Cluster = LocalCluster(),
+        fn: Callable[[Any], Any],
     ):
         """
         Function Task object. This wraps a fn into a task
 
         Args:
             fn (Callable[[Any], Any]): callable function to be run
         """
-        super().__init__(name, env_requirements, resources, config, cluster)
+        super().__init__(name)
         self.fn = fn
 
     def __call__(self, *args, **kwargs) -> Any:
         """
         Runs the fn with args & kwargs
 
         Returns:
@@ -158,55 +192,34 @@
         """
         return self.fn(*args, **kwargs)
 
 
 def task(
     fn: Callable[[Any], Any] = None,
     name: str = None,
-    env_requirements: Optional[Union[List[str], str]] = None,
-    resources: Optional[Dict[str, Any]] = None,
-    config: Dict[str, Any] = {},
-    cluster: Cluster = LocalCluster(),
+    options: Optional[TaskOptions] = None,
+    **kwargs,
 ):
     """
-    Task decorator, returns a Function Task object
+    Task decorator, returns a FunctiFunctionTaskon Task object
 
     Args:
         fn (Callable[[Any], Any]): callable function to be run
-        name (str): name of the function
-        env_requirements (Optional[Union[List[str], str]], optional): List of requirements to install on the remote cluster, or path to the requirements.txt file.  Defaults to None.
-        resources (Optional[Dict[str, Any]], optional): Optional number (int) of resources needed to run the Function on the Cluster. Keys must be num_cpus and num_gpus.. Defaults to None.
-        config (Dict[str, Any], optional): additional config for building the remote function. Defaults to {}.
-        cluster (Cluster, optional): cluster to run on. Defaults to LocalCluster().
+        name (str): name of the task
     """
 
     def decorator(fn):
         function_name = name
         if function_name is None:
             function_name = fn.__name__
-        return FunctionTask(
-            fn,
-            name=name,
-            env_requirements=env_requirements,
-            resources=resources,
-            config=config,
-            cluster=cluster,
-        )
+        task = FunctionTask(name=name, fn=fn)
+        return task
 
     if fn is None:
         return decorator
 
     function_name = name
     if function_name is None:
         function_name = fn.__name__
 
-    return FunctionTask(
-        fn,
-        name=function_name,
-        env_requirements=env_requirements,
-        resources=resources,
-        config=config,
-        cluster=cluster,
-    )
-
-
-TaskSpec = Union[Task, Callable[[Any], Any]]
+    task = FunctionTask(name=function_name, fn=fn)
+    return task
```

### Comparing `trainyard-0.0.1/trainyard/track.py` & `trainyard-0.0.1a0/trainyard/track.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1/trainyard/trainer/base.py` & `trainyard-0.0.1a0/trainyard/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1/trainyard/workflow/prefect.py` & `trainyard-0.0.1a0/trainyard/workflow/prefect.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from trainyard.tasks.tasks import Task, TaskWrapper
 from trainyard.workflow.workflow import WorkflowBackend
 
 
 class PrefectTaskWrapper(TaskWrapper):
     def wrap(self, f: Callable[[Any], Any], task: Task) -> Callable[[Any], Any]:
         return prefect.task(
-            name=task.name,
-            description=task.description,
-            # task_run_name="{name}-on-{date:%A}",
+            name=task.name, description=task.options.description, refresh_cache=True
         )(f)
 
 
 class PrefectWorkflowBackend(WorkflowBackend):
     def __init__(self, workflow_params: Dict[str, Any] = {}):
         self.workflow_params = workflow_params
```

### Comparing `trainyard-0.0.1/trainyard/workflow/workflow.py` & `trainyard-0.0.1a0/trainyard/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `trainyard-0.0.1/trainyard.egg-info/SOURCES.txt` & `trainyard-0.0.1a0/trainyard.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 trainyard.egg-info/dependency_links.txt
 trainyard.egg-info/requires.txt
 trainyard.egg-info/top_level.txt
 trainyard/engine/__init__.py
 trainyard/engine/cluster.py
 trainyard/engine/local.py
 trainyard/engine/runhouse.py
+trainyard/engine/utils.py
+trainyard/engine_v2/engine.py
+trainyard/engine_v2/runhouse.py
 trainyard/tasks/__init__.py
 trainyard/tasks/tasks.py
 trainyard/trainer/__init__.py
 trainyard/trainer/base.py
 trainyard/workflow/__init__.py
 trainyard/workflow/prefect.py
 trainyard/workflow/workflow.py
```

