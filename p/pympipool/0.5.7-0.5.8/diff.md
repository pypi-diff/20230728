# Comparing `tmp/pympipool-0.5.7.tar.gz` & `tmp/pympipool-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.7.tar", last modified: Tue Jul 25 19:50:13 2023, max compression
+gzip compressed data, was "pympipool-0.5.8.tar", last modified: Thu Jul 27 23:36:19 2023, max compression
```

## Comparing `pympipool-0.5.7.tar` & `pympipool-0.5.8.tar`

### file list

```diff
@@ -1,44 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.560990 pympipool-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-25 19:50:08.000000 pympipool-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 19:50:08.000000 pympipool-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-25 19:50:13.560990 pympipool-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-25 19:50:08.000000 pympipool-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.560990 pympipool-0.5.7/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 19:50:13.560990 pympipool-0.5.7/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.552990 pympipool-0.5.7/pympipool/external_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.556990 pympipool-0.5.7/pympipool/parallel_executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/parallel_executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/parallel_executors/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/parallel_executors/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.556990 pympipool-0.5.7/pympipool/shared_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/shared_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/shared_functions/external_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/shared_functions/parallel_executors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.552990 pympipool-0.5.7/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 19:50:13.560990 pympipool-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 19:50:13.000000 pympipool-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.560990 pympipool-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-25 19:50:08.000000 pympipool-0.5.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.940517 pympipool-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-27 23:36:17.000000 pympipool-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 23:36:17.000000 pympipool-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-27 23:36:19.940517 pympipool-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-27 23:36:17.000000 pympipool-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.940517 pympipool-0.5.8/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 23:36:19.940517 pympipool-0.5.8/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/backend/mpiexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/interfaces/taskbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/interfaces/taskexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/backend/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/interfaces/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/shared/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/taskexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-27 23:36:19.940517 pympipool-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-27 23:36:19.000000 pympipool-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.940517 pympipool-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_parse_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-27 23:36:17.000000 pympipool-0.5.8/versioneer.py
```

### Comparing `pympipool-0.5.7/LICENSE` & `pympipool-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/PKG-INFO` & `pympipool-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.7
+Version: 0.5.8
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.7/README.md` & `pympipool-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/pympipool/__init__.py` & `pympipool-0.5.8/pympipool/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from pympipool.external_interfaces.communication import (
+from pympipool.shared.communication import (
     SocketInterface,
     connect_to_socket_interface,
     send_result,
     close_connection,
     receive_instruction,
 )
-from pympipool.external_interfaces.executor import Executor, PoolExecutor
-from pympipool.external_interfaces.pool import Pool, MPISpawnPool
-from pympipool.external_interfaces.thread import RaisingThread
-from pympipool.shared_functions.external_interfaces import cancel_items_in_queue
+from pympipool.interfaces.taskbroker import HPCExecutor
+from pympipool.interfaces.taskexecutor import Executor
+from pympipool.legacy.interfaces.executor import PoolExecutor
+from pympipool.legacy.interfaces.pool import Pool, MPISpawnPool
+from pympipool.shared.thread import RaisingThread
+from pympipool.shared.taskexecutor import cancel_items_in_queue
 
 from ._version import get_versions
 
 __version__ = get_versions()["version"]
 del get_versions
```

### Comparing `pympipool-0.5.7/pympipool/external_interfaces/communication.py` & `pympipool-0.5.8/pympipool/shared/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/pympipool/external_interfaces/executor.py` & `pympipool-0.5.8/pympipool/shared/taskexecutor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,194 +1,173 @@
-from abc import ABC
-from concurrent.futures import Executor as FutureExecutor, Future
-from queue import Queue
-
-from pympipool.external_interfaces.thread import RaisingThread
-from pympipool.shared_functions.external_interfaces import (
-    execute_parallel_tasks,
-    execute_serial_tasks,
-    cloudpickle_register,
-    cancel_items_in_queue,
-)
-
-
-class ExecutorBase(FutureExecutor, ABC):
-    """
-    Base class for the Executor and PoolExecutor class defined below. The ExecutorBase class is not intended to be used
-    alone. Rather it implements the submit(), shutdown() and __len__() function shared between the derived classes.
-    """
-
-    def __init__(self):
-        self._future_queue = Queue()
-        self._process = None
-        cloudpickle_register(ind=3)
-
-    def submit(self, fn, *args, **kwargs):
-        """Submits a callable to be executed with the given arguments.
-
-        Schedules the callable to be executed as fn(*args, **kwargs) and returns
-        a Future instance representing the execution of the callable.
-
-        Returns:
-            A Future representing the given call.
-        """
-        f = Future()
-        self._future_queue.put({"fn": fn, "args": args, "kwargs": kwargs, "future": f})
-        return f
-
-    def shutdown(self, wait=True, *, cancel_futures=False):
-        """Clean-up the resources associated with the Executor.
-
-        It is safe to call this method several times. Otherwise, no other
-        methods can be called after this one.
-
-        Args:
-            wait: If True then shutdown will not return until all running
-                futures have finished executing and the resources used by the
-                parallel_executors have been reclaimed.
-            cancel_futures: If True then shutdown will cancel all pending
-                futures. Futures that are completed or running will not be
-                cancelled.
-        """
-        if cancel_futures:
-            cancel_items_in_queue(que=self._future_queue)
-        self._future_queue.put({"shutdown": True, "wait": wait})
-        self._process.join()
-
-    def __len__(self):
-        return self._future_queue.qsize()
-
-
-class Executor(ExecutorBase):
-    """
-    The pympipool.Executor behaves like the concurrent.futures.Executor but it uses mpi4py to execute parallel tasks.
-    In contrast to the mpi4py.futures.MPIPoolExecutor the pympipool.Executor can be executed in a serial python process
-    and does not require the python script to be executed with MPI. Still internally the pympipool.Executor uses the
-    mpi4py.futures.MPIPoolExecutor, consequently it is primarily an abstraction of its functionality to improve the
-    usability in particular when used in combination with Jupyter notebooks.
+import inspect
+import os
+import socket
+import queue
+
+import cloudpickle
+
+from pympipool.shared.communication import SocketInterface
+
+
+def cancel_items_in_queue(que):
+    """
+    Cancel items which are still waiting in the queue. If the executor is busy tasks remain in the queue, so the future
+    objects have to be cancelled when the executor shuts down.
 
     Args:
-        cores (int): defines the number of MPI ranks to use for each function call
-        oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only) - default False
-        enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
-        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
-        init_function (None): optional function to preset arguments for functions which are submitted later
-        cwd (str/None): current working directory where the parallel python task is executed
-        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
-        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
-
-    Simple example:
-        ```
-        import numpy as np
-        from pympipool import Executor
-
-        def calc(i, j, k):
-            from mpi4py import MPI
-            size = MPI.COMM_WORLD.Get_size()
-            rank = MPI.COMM_WORLD.Get_rank()
-            return np.array([i, j, k]), size, rank
-
-        def init_k():
-            return {"k": 3}
-
-        with Executor(cores=2, init_function=init_k) as p:
-            fs = p.submit(calc, 2, j=4)
-            print(fs.result())
-
-        >>> [(array([2, 4, 3]), 2, 0), (array([2, 4, 3]), 2, 1)]
-        ```
-    """
-
-    def __init__(
-        self,
-        cores,
-        oversubscribe=False,
-        enable_flux_backend=False,
-        enable_slurm_backend=False,
-        init_function=None,
-        cwd=None,
-        queue_adapter=None,
-        queue_adapter_kwargs=None,
-    ):
-        super().__init__()
-        self._process = RaisingThread(
-            target=execute_parallel_tasks,
-            kwargs={
-                "future_queue": self._future_queue,
-                "cores": cores,
-                "oversubscribe": oversubscribe,
-                "enable_flux_backend": enable_flux_backend,
-                "enable_slurm_backend": enable_slurm_backend,
-                "cwd": cwd,
-                "queue_adapter": queue_adapter,
-                "queue_adapter_kwargs": queue_adapter_kwargs,
-            },
-        )
-        self._process.start()
-        if init_function is not None:
-            self._future_queue.put(
-                {"init": True, "fn": init_function, "args": (), "kwargs": {}}
-            )
-
-
-class PoolExecutor(ExecutorBase):
-    """
-    To combine the functionality of the pympipool.Pool and the pympipool.Executor the pympipool.PoolExecutor again
-    connects to the mpi4py.futures.MPIPoolExecutor. Still in contrast to the pympipool.Pool it does not implement the
-    map() and starmap() functions but rather the submit() function based on the concurrent.futures.Executor interface.
-    In this case the load balancing happens internally and the maximum number of workers max_workers defines the maximum
-    number of parallel tasks. But only serial python tasks can be executed in contrast to the pympipool.Executor which
-    can also execute MPI parallel python tasks.
+        que (queue.Queue): Queue with task objects which should be executed
+    """
+    while True:
+        try:
+            item = que.get_nowait()
+            if isinstance(item, dict) and "future" in item.keys():
+                item["future"].cancel()
+                que.task_done()
+        except queue.Empty:
+            break
+
+
+def cloudpickle_register(ind=2):
+    """
+    Cloudpickle can either pickle by value or pickle by reference. The functions which are communicated have to
+    be pickled by value rather than by reference, so the module which calls the map function is pickled by value.
+    https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs
+    inspect can help to find the module which is calling pympipool
+    https://docs.python.org/3/library/inspect.html
+    to learn more about inspect another good read is:
+    http://pymotw.com/2/inspect/index.html#module-inspect
+    1 refers to 1 level higher than the map function
+
+    Args:
+        ind (int): index of the level at which pickle by value starts while for the rest pickle by reference is used
+    """
+    try:  # When executed in a jupyter notebook this can cause a ValueError - in this case we just ignore it.
+        cloudpickle.register_pickle_by_value(inspect.getmodule(inspect.stack()[ind][0]))
+    except ValueError:
+        pass
+
+
+def command_line_options(
+    hostname,
+    port_selected,
+    path,
+    cores,
+    gpus_per_task=0,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    enable_slurm_backend=False,
+    enable_multi_host=False,
+):
+    """
+    Translate the individual parameters to command line options.
 
     Args:
-        max_workers (int): defines the total number of MPI ranks to use
-        oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only) - default False
-        enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
+        hostname (str): name of the host where the SocketInterface instance runs the client process should conenct to.
+        port_selected (int): port the SocketInterface instance runs on.
+        path (str): path to the python script which should be executed as client process.
+        cores (int): defines the total number of MPI ranks to use
+        cores_per_task (int): number of MPI ranks per task - defaults to 1
+        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
+        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
-        cwd (str/None): current working directory where the parallel python task is executed
-        sleep_interval (float):
-        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
-        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
-
-    Simple example:
-        ```
-        from pympipool import PoolExecutor
-
-        def calc(i, j):
-            return i + j
-
-        with PoolExecutor(max_workers=2) as p:
-            fs1 = p.submit(calc, 1, 2)
-            fs2 = p.submit(calc, 3, 4)
-            fs3 = p.submit(calc, 5, 6)
-            fs4 = p.submit(calc, 7, 8)
-            print(fs1.result(), fs2.result(), fs3.result(), fs4.result()
-        ```
-    """
-
-    def __init__(
-        self,
-        max_workers=1,
-        oversubscribe=False,
-        enable_flux_backend=False,
-        enable_slurm_backend=False,
-        cwd=None,
-        sleep_interval=0.1,
-        queue_adapter=None,
-        queue_adapter_kwargs=None,
-    ):
-        super().__init__()
-        self._process = RaisingThread(
-            target=execute_serial_tasks,
-            kwargs={
-                "future_queue": self._future_queue,
-                "cores": max_workers,
-                "oversubscribe": oversubscribe,
-                "enable_flux_backend": enable_flux_backend,
-                "enable_slurm_backend": enable_slurm_backend,
-                "cwd": cwd,
-                "sleep_interval": sleep_interval,
-                "queue_adapter": queue_adapter,
-                "queue_adapter_kwargs": queue_adapter_kwargs,
-            },
-        )
-        self._process.start()
+        enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
+        enable_multi_host (bool): communicate the host to connect to - defaults to False
+
+    Returns:
+        list: list of strings to be executed on the command line
+    """
+    if enable_flux_backend:
+        command_lst = ["flux", "run"]
+    elif enable_slurm_backend:
+        command_lst = ["srun"]
+    else:
+        command_lst = ["mpiexec"]
+    if gpus_per_task > 0 and (enable_flux_backend or enable_slurm_backend):
+        command_lst += ["--gpus-per-task=" + str(gpus_per_task)]
+    elif gpus_per_task > 0:
+        raise ValueError("GPU binding is only supported for flux and SLURM backend.")
+    if oversubscribe:
+        command_lst += ["--oversubscribe"]
+    command_lst += ["-n", str(cores), "python", path]
+    if enable_flux_backend or enable_slurm_backend or enable_multi_host:
+        command_lst += [
+            "--host",
+            hostname,
+        ]
+    command_lst += [
+        "--zmqport",
+        str(port_selected),
+    ]
+    return command_lst
+
+
+def execute_parallel_tasks(
+    future_queue,
+    cores,
+    gpus_per_task=0,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    enable_slurm_backend=False,
+    cwd=None,
+    queue_adapter=None,
+    queue_adapter_kwargs=None,
+):
+    """
+    Execute a single tasks in parallel using the message passing interface (MPI).
+
+    Args:
+       future_queue (queue.Queue): task queue of dictionary objects which are submitted to the parallel process
+       cores (int): defines the total number of MPI ranks to use
+       gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
+       oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+       enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
+       enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+       cwd (str/None): current working directory where the parallel python task is executed
+       queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
+       queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
+    """
+    interface = SocketInterface(
+        queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+    )
+    interface.bootup(
+        command_lst=command_line_options(
+            hostname=socket.gethostname(),
+            port_selected=interface.bind_to_random_port(),
+            path=os.path.abspath(
+                os.path.join(__file__, "..", "..", "backend", "mpiexec.py")
+            ),
+            cores=cores,
+            gpus_per_task=gpus_per_task,
+            oversubscribe=oversubscribe,
+            enable_flux_backend=enable_flux_backend,
+            enable_slurm_backend=enable_slurm_backend,
+            enable_multi_host=queue_adapter is not None,
+        ),
+        cwd=cwd,
+        cores=cores,
+    )
+    _execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
+
+
+def _execute_parallel_tasks_loop(interface, future_queue):
+    while True:
+        task_dict = future_queue.get()
+        if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
+            interface.shutdown(wait=task_dict["wait"])
+            future_queue.task_done()
+            break
+        elif "fn" in task_dict.keys() and "future" in task_dict.keys():
+            f = task_dict.pop("future")
+            if f.set_running_or_notify_cancel():
+                try:
+                    f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+                except Exception as thread_exeception:
+                    interface.shutdown(wait=True)
+                    future_queue.task_done()
+                    f.set_exception(exception=thread_exeception)
+                    raise thread_exeception
+                else:
+                    future_queue.task_done()
+        elif "fn" in task_dict.keys() and "init" in task_dict.keys():
+            interface.send_dict(input_dict=task_dict)
+            future_queue.task_done()
```

### Comparing `pympipool-0.5.7/pympipool/external_interfaces/pool.py` & `pympipool-0.5.8/pympipool/legacy/interfaces/pool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from abc import ABC
 
-from pympipool.external_interfaces.communication import SocketInterface
-from pympipool.shared_functions.external_interfaces import (
-    get_parallel_subprocess_command,
-    cloudpickle_register,
-)
+from pympipool.shared.communication import SocketInterface
+from pympipool.shared.taskexecutor import cloudpickle_register
+from pympipool.legacy.shared.interface import get_parallel_subprocess_command
 
 
 class PoolBase(ABC):
     """
     Base class for the Pool and MPISpawnPool classes defined below. The PoolBase class is not intended to be used
     alone. Rather it implements the __enter__(), __exit__() and shutdown() function shared between the derived classes.
     """
@@ -37,14 +35,15 @@
     mpi4py.futures.MPIPoolExecutor the pympipool.Pool can be executed in a serial python process and does not require
     the python script to be executed with MPI. Still internally the pympipool.Pool uses the
     mpi4py.futures.MPIPoolExecutor, consequently it is primarily an abstraction of its functionality to improve the
     usability in particular when used in combination with Jupyter notebooks.
 
     Args:
         max_workers (int): defines the total number of MPI ranks to use
+        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
         oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only)
         enable_flux_backend (bool): use the flux-framework as backend
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
         cwd (str/None): current working directory where the parallel python task is executed
         queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
         queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
 
@@ -60,14 +59,15 @@
             print(p.map(func=calc, iterable=[1, 2, 3, 4]))
         ```
     """
 
     def __init__(
         self,
         max_workers=1,
+        gpus_per_task=0,
         oversubscribe=False,
         enable_flux_backend=False,
         enable_slurm_backend=False,
         cwd=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
@@ -75,14 +75,15 @@
             queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
         )
         self._interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=self._interface.bind_to_random_port(),
                 cores=max_workers,
                 cores_per_task=1,
+                gpus_per_task=gpus_per_task,
                 oversubscribe=oversubscribe,
                 enable_flux_backend=enable_flux_backend,
                 enable_slurm_backend=enable_slurm_backend,
                 enable_mpi4py_backend=True,
                 enable_multi_host=queue_adapter is not None,
             ),
             cwd=cwd,
@@ -145,14 +146,15 @@
     not require the python script to be executed with MPI. Still internally the pympipool.Pool uses the
     mpi4py.futures.MPIPoolExecutor, consequently it is primarily an abstraction of its functionality to improve the
     usability in particular when used in combination with Jupyter notebooks.
 
     Args:
         max_ranks (int): defines the total number of MPI ranks to use
         ranks_per_task (int): defines the number of MPI ranks per task
+        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
         oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only)
         cwd (str/None): current working directory where the parallel python task is executed
         queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
         queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
 
     Simple example:
         ```
@@ -166,27 +168,29 @@
         ```
     """
 
     def __init__(
         self,
         max_ranks=1,
         ranks_per_task=1,
+        gpus_per_task=0,
         oversubscribe=False,
         cwd=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
         super().__init__(
             queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
         )
         self._interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=self._interface.bind_to_random_port(),
                 cores=max_ranks,
                 cores_per_task=ranks_per_task,
+                gpus_per_task=gpus_per_task,
                 oversubscribe=oversubscribe,
                 enable_flux_backend=False,
                 enable_slurm_backend=False,
                 enable_mpi4py_backend=True,
                 enable_multi_host=queue_adapter is not None,
             ),
             cwd=cwd,
```

### Comparing `pympipool-0.5.7/pympipool/external_interfaces/thread.py` & `pympipool-0.5.8/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/pympipool/parallel_executors/mpiexec.py` & `pympipool-0.5.8/pympipool/backend/mpiexec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from os.path import abspath
 import pickle
 import sys
 
 import cloudpickle
 
-from pympipool.external_interfaces.communication import (
+from pympipool.shared.communication import (
     connect_to_socket_interface,
     send_result,
     close_connection,
     receive_instruction,
 )
-from pympipool.shared_functions.parallel_executors import call_funct, parse_arguments
+from pympipool.shared.backend import call_funct, parse_arguments
 
 
 def main():
     from mpi4py import MPI
 
     MPI.pickle.__init__(
         cloudpickle.dumps,
```

### Comparing `pympipool-0.5.7/pympipool/parallel_executors/mpipool.py` & `pympipool-0.5.8/pympipool/legacy/backend/mpipool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from os.path import abspath
 import pickle
 import sys
 
 import cloudpickle
 
-from pympipool.external_interfaces.communication import (
+from pympipool.shared.communication import (
     connect_to_socket_interface,
     send_result,
     close_connection,
     receive_instruction,
 )
-from pympipool.shared_functions.parallel_executors import (
-    parse_arguments,
-    parse_socket_communication,
-)
+from pympipool.legacy.shared.backend import parse_socket_communication, parse_arguments
 
 
 def main():
     from mpi4py import MPI
 
     MPI.pickle.__init__(
         cloudpickle.dumps,
```

### Comparing `pympipool-0.5.7/pympipool/shared_functions/external_interfaces.py` & `pympipool-0.5.8/pympipool/legacy/shared/interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,23 @@
-import inspect
 import os
+import queue
 import socket
 import time
-import queue
-
-import cloudpickle
-
-from pympipool.external_interfaces.communication import SocketInterface
-
-
-def cancel_items_in_queue(que):
-    while True:
-        try:
-            item = que.get_nowait()
-            if isinstance(item, dict) and "future" in item.keys():
-                item["future"].cancel()
-        except queue.Empty:
-            break
 
 
-def cloudpickle_register(ind=2):
-    # Cloudpickle can either pickle by value or pickle by reference. The functions which are communicated have to
-    # be pickled by value rather than by reference, so the module which calls the map function is pickled by value.
-    # https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs
-    # inspect can help to find the module which is calling pympipool
-    # https://docs.python.org/3/library/inspect.html
-    # to learn more about inspect another good read is:
-    # http://pymotw.com/2/inspect/index.html#module-inspect
-    # 1 refers to 1 level higher than the map function
-    try:  # When executed in a jupyter notebook this can cause a ValueError - in this case we just ignore it.
-        cloudpickle.register_pickle_by_value(inspect.getmodule(inspect.stack()[ind][0]))
-    except ValueError:
-        pass
+from pympipool.shared.communication import SocketInterface
 
 
 def command_line_options(
     hostname,
     port_selected,
     path,
     cores,
     cores_per_task=1,
+    gpus_per_task=0,
     oversubscribe=False,
     enable_flux_backend=False,
     enable_slurm_backend=False,
     enable_mpi4py_backend=True,
     enable_multi_host=False,
 ):
     """
@@ -51,14 +25,15 @@
 
     Args:
         hostname (str): name of the host where the SocketInterface instance runs the client process should conenct to.
         port_selected (int): port the SocketInterface instance runs on.
         path (str): path to the python script which should be executed as client process.
         cores (int): defines the total number of MPI ranks to use
         cores_per_task (int): number of MPI ranks per task - defaults to 1
+        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
         oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
         enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
         enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
         enable_multi_host (bool): communicate the host to connect to - defaults to False
 
     Returns:
@@ -66,14 +41,18 @@
     """
     if enable_flux_backend:
         command_lst = ["flux", "run"]
     elif enable_slurm_backend:
         command_lst = ["srun"]
     else:
         command_lst = ["mpiexec"]
+    if gpus_per_task > 0 and (enable_flux_backend or enable_slurm_backend):
+        command_lst += ["--gpus-per-task=" + str(gpus_per_task)]
+    elif gpus_per_task > 0:
+        raise ValueError("GPU binding is only supported for flux and SLURM backend.")
     if oversubscribe:
         command_lst += ["--oversubscribe"]
     if cores_per_task == 1 and enable_mpi4py_backend:
         command_lst += ["-n", str(cores), "python", "-m", "mpi4py.futures"]
     elif cores_per_task > 1 and enable_mpi4py_backend:
         # Running MPI parallel tasks within the map() requires mpi4py to use mpi spawn:
         # https://github.com/mpi4py/mpi4py/issues/324
@@ -96,74 +75,84 @@
             str(cores_per_task),
             "--cores-total",
             str(cores),
         ]
     return command_lst
 
 
-def execute_parallel_tasks(
-    future_queue,
+def get_parallel_subprocess_command(
+    port_selected,
     cores,
+    cores_per_task=1,
+    gpus_per_task=0,
     oversubscribe=False,
     enable_flux_backend=False,
     enable_slurm_backend=False,
-    cwd=None,
-    queue_adapter=None,
-    queue_adapter_kwargs=None,
+    enable_mpi4py_backend=True,
+    enable_multi_host=False,
 ):
     """
-    Execute a single tasks in parallel using the message passing interface (MPI).
+    Translate the individual parameters to command line options.
 
     Args:
-       future_queue (queue.Queue): task queue of dictionary objects which are submitted to the parallel process
-       cores (int): defines the total number of MPI ranks to use
-       oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
-       enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
-       enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
-       cwd (str/None): current working directory where the parallel python task is executed
-       queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
-       queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
+        port_selected (int): port the SocketInterface instance runs on.
+        cores (int): defines the total number of MPI ranks to use
+        cores_per_task (int): number of MPI ranks per task - defaults to 1
+        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
+        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
+        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+        enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
+        enable_multi_host (bool): communicate the host to connect to - defaults to False
+
+    Returns:
+        list: list of strings to be executed on the command line
     """
-    interface = SocketInterface(
-        queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
-    )
-    interface.bootup(
-        command_lst=get_parallel_subprocess_command(
-            port_selected=interface.bind_to_random_port(),
-            cores=cores,
-            cores_per_task=1,
-            oversubscribe=oversubscribe,
-            enable_flux_backend=enable_flux_backend,
-            enable_slurm_backend=enable_slurm_backend,
-            enable_mpi4py_backend=False,
-            enable_multi_host=queue_adapter is not None,
-        ),
-        cwd=cwd,
+    if enable_mpi4py_backend:
+        executable = os.path.abspath(
+            os.path.join(__file__, "..", "..", "backend", "mpipool.py")
+        )
+    else:
+        executable = os.path.abspath(
+            os.path.join(__file__, "..", "..", "..", "backend", "mpiexec.py")
+        )
+    return command_line_options(
+        hostname=socket.gethostname(),
+        port_selected=port_selected,
+        path=executable,
         cores=cores,
+        cores_per_task=cores_per_task,
+        gpus_per_task=gpus_per_task,
+        oversubscribe=oversubscribe,
+        enable_flux_backend=enable_flux_backend,
+        enable_slurm_backend=enable_slurm_backend,
+        enable_mpi4py_backend=enable_mpi4py_backend,
+        enable_multi_host=enable_multi_host,
     )
-    _execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
 
 
 def execute_serial_tasks(
     future_queue,
     cores,
+    gpus_per_task=0,
     oversubscribe=False,
     enable_flux_backend=False,
     enable_slurm_backend=False,
     cwd=None,
     sleep_interval=0.1,
     queue_adapter=None,
     queue_adapter_kwargs=None,
 ):
     """
     Execute a single tasks in serial.
 
     Args:
        future_queue (queue.Queue): task queue of dictionary objects which are submitted to the parallel process
        cores (int): defines the total number of MPI ranks to use
+       gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
        cwd (str/None): current working directory where the parallel python task is executed
        sleep_interval (float):
        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
@@ -172,14 +161,15 @@
     interface = SocketInterface(
         queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
     )
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
+            gpus_per_task=gpus_per_task,
             cores_per_task=1,
             oversubscribe=oversubscribe,
             enable_flux_backend=enable_flux_backend,
             enable_slurm_backend=enable_slurm_backend,
             enable_mpi4py_backend=True,
             enable_multi_host=queue_adapter is not None,
         ),
@@ -190,78 +180,14 @@
         interface=interface,
         future_queue=future_queue,
         future_dict=future_dict,
         sleep_interval=sleep_interval,
     )
 
 
-def get_parallel_subprocess_command(
-    port_selected,
-    cores,
-    cores_per_task=1,
-    oversubscribe=False,
-    enable_flux_backend=False,
-    enable_slurm_backend=False,
-    enable_mpi4py_backend=True,
-    enable_multi_host=False,
-):
-    """
-    Translate the individual parameters to command line options.
-
-    Args:
-        port_selected (int): port the SocketInterface instance runs on.
-        cores (int): defines the total number of MPI ranks to use
-        cores_per_task (int): number of MPI ranks per task - defaults to 1
-        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
-        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
-        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
-        enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
-        enable_multi_host (bool): communicate the host to connect to - defaults to False
-
-    Returns:
-        list: list of strings to be executed on the command line
-    """
-    if enable_mpi4py_backend:
-        executable = "mpipool.py"
-    else:
-        executable = "mpiexec.py"
-    return command_line_options(
-        hostname=socket.gethostname(),
-        port_selected=port_selected,
-        path=os.path.abspath(
-            os.path.join(__file__, "../../parallel_executors", executable)
-        ),
-        cores=cores,
-        cores_per_task=cores_per_task,
-        oversubscribe=oversubscribe,
-        enable_flux_backend=enable_flux_backend,
-        enable_slurm_backend=enable_slurm_backend,
-        enable_mpi4py_backend=enable_mpi4py_backend,
-        enable_multi_host=enable_multi_host,
-    )
-
-
-def _execute_parallel_tasks_loop(interface, future_queue):
-    while True:
-        task_dict = future_queue.get()
-        if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
-            interface.shutdown(wait=task_dict["wait"])
-            break
-        elif "fn" in task_dict.keys() and "future" in task_dict.keys():
-            f = task_dict.pop("future")
-            if f.set_running_or_notify_cancel():
-                try:
-                    f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
-                except Exception as thread_exeception:
-                    f.set_exception(exception=thread_exeception)
-                    raise thread_exeception
-        elif "fn" in task_dict.keys() and "init" in task_dict.keys():
-            interface.send_dict(input_dict=task_dict)
-
-
 def _execute_serial_tasks_loop(
     interface, future_queue, future_dict, sleep_interval=0.1
 ):
     while True:
         try:
             task_dict = future_queue.get_nowait()
         except queue.Empty:
@@ -269,19 +195,21 @@
         else:
             if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
                 done_dict = interface.shutdown(wait=task_dict["wait"])
                 if isinstance(done_dict, dict):
                     for k, v in done_dict.items():
                         if k in future_dict.keys() and not future_dict[k].cancelled():
                             future_dict.pop(k).set_result(v)
+                future_queue.task_done()
                 break
             elif "fn" in task_dict.keys() and "future" in task_dict.keys():
                 f = task_dict.pop("future")
                 future_hash = interface.send_and_receive_dict(input_dict=task_dict)
                 future_dict[future_hash] = f
+                future_queue.task_done()
         _update_future_dict(
             interface=interface, future_dict=future_dict, sleep_interval=sleep_interval
         )
 
 
 def _update_future_dict(interface, future_dict, sleep_interval=0.1):
     time.sleep(sleep_interval)
```

### Comparing `pympipool-0.5.7/pympipool/shared_functions/parallel_executors.py` & `pympipool-0.5.8/pympipool/legacy/shared/backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-import inspect
-
 from tqdm import tqdm
 
-
-def call_funct(input_dict, funct=None, memory=None):
-    if funct is None:
-
-        def funct(*args, **kwargs):
-            return args[0].__call__(*args[1:], **kwargs)
-
-    funct_args = inspect.getfullargspec(input_dict["fn"]).args
-    if memory is not None:
-        input_dict["kwargs"].update(
-            _update_dict_delta(
-                dict_input=memory,
-                dict_output=input_dict["kwargs"],
-                keys_possible_lst=funct_args,
-            )
-        )
-    return funct(input_dict["fn"], *input_dict["args"], **input_dict["kwargs"])
+from pympipool.shared.backend import call_funct, _update_default_dict_from_arguments
 
 
 def map_funct(executor, funct, lst, chunksize=1, cores_per_task=1, map_flag=True):
     if cores_per_task == 1:
         if map_flag:
             results = executor.map(funct, lst, chunksize=chunksize)
         else:
@@ -56,29 +38,24 @@
 
     Args:
         argument_lst (list): list of arguments as strings
 
     Returns:
         dict: dictionary with the parsed arguments and their corresponding values
     """
-    argument_dict = {
-        "total_cores": "--cores-total",
-        "zmqport": "--zmqport",
-        "cores_per_task": "--cores-per-task",
-        "host": "--host",
-    }
-    parse_dict = {"host": "localhost"}
-    parse_dict.update(
-        {
-            k: argument_lst[argument_lst.index(v) + 1]
-            for k, v in argument_dict.items()
-            if v in argument_lst
-        }
+    return _update_default_dict_from_arguments(
+        argument_lst=argument_lst,
+        argument_dict={
+            "total_cores": "--cores-total",
+            "zmqport": "--zmqport",
+            "cores_per_task": "--cores-per-task",
+            "host": "--host",
+        },
+        default_dict={"host": "localhost"},
     )
-    return parse_dict
 
 
 def parse_socket_communication(executor, input_dict, future_dict, cores_per_task=1):
     if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
         executor.shutdown(wait=input_dict["wait"])
         done_dict = _update_futures(future_dict=future_dict)
         # If close "shutdown" is communicated the process is shutdown.
@@ -123,22 +100,14 @@
         return {"result": done_dict}
     elif "cancel" in input_dict.keys():
         for k in input_dict["cancel"]:
             future_dict[k].cancel()
         return {"result": True}
 
 
-def _update_dict_delta(dict_input, dict_output, keys_possible_lst):
-    return {
-        k: v
-        for k, v in dict_input.items()
-        if k in keys_possible_lst and k not in dict_output.keys()
-    }
-
-
 def _update_futures(future_dict, hash_lst=None):
     if hash_lst is None:
         hash_lst = list(future_dict.keys())
     done_dict = {
         k: f.result()
         for k, f in {k: future_dict[k] for k in hash_lst}.items()
         if f.done()
```

### Comparing `pympipool-0.5.7/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.8/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.7
+Version: 0.5.8
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.7/setup.py` & `pympipool-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/tests/test_communicator_split.py` & `pympipool-0.5.8/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/tests/test_executor.py` & `pympipool-0.5.8/tests/test_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 from concurrent.futures import ThreadPoolExecutor
-from pympipool.shared_functions.parallel_executors import map_funct, parse_socket_communication, call_funct
+from pympipool.legacy.shared.backend import map_funct, parse_socket_communication
+from pympipool.shared.backend import call_funct
 
 
 def function_multi_args(a, b):
     return a + b
 
 
 class TestExecutor(unittest.TestCase):
```

### Comparing `pympipool-0.5.7/tests/test_future.py` & `pympipool-0.5.8/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/tests/test_interface.py` & `pympipool-0.5.8/tests/test_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+import os
+import socket
+
 import numpy as np
 import unittest
-from pympipool.external_interfaces.communication import SocketInterface
-from pympipool.shared_functions.external_interfaces import get_parallel_subprocess_command, cloudpickle_register
+from pympipool.shared.communication import SocketInterface
+from pympipool.shared.taskexecutor import command_line_options, cloudpickle_register
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
 class TestInterface(unittest.TestCase):
     def test_interface(self):
         cloudpickle_register(ind=1)
         task_dict = {"fn": calc, 'args': (), "kwargs": {"i": 2}}
         interface = SocketInterface(queue_adapter=None, queue_adapter_kwargs=None)
         interface.bootup(
-            command_lst=get_parallel_subprocess_command(
+            command_lst=command_line_options(
+                hostname=socket.gethostname(),
                 port_selected=interface.bind_to_random_port(),
+                path=os.path.abspath(os.path.join(__file__, "..", "..", "pympipool", "backend", "mpiexec.py")),
                 cores=1,
-                cores_per_task=1,
+                gpus_per_task=0,
                 oversubscribe=False,
                 enable_flux_backend=False,
-                enable_mpi4py_backend=False,
+                enable_slurm_backend=False,
+                enable_multi_host=False,
             )
         )
         self.assertEqual(interface.send_and_receive_dict(input_dict=task_dict), np.array(4))
         interface.shutdown(wait=True)
```

### Comparing `pympipool-0.5.7/tests/test_multitask.py` & `pympipool-0.5.8/tests/test_multitask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import unittest
 from queue import Queue
 from time import sleep
 from pympipool import PoolExecutor
-from pympipool.shared_functions.external_interfaces import execute_serial_tasks, cloudpickle_register
+from pympipool.legacy.shared.interface import execute_serial_tasks
+from pympipool.shared.taskexecutor import cloudpickle_register
 from concurrent.futures import Future
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
@@ -49,14 +50,15 @@
         execute_serial_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array(4))
+        q.join()
 
     def test_pool_cancel(self):
         with PoolExecutor(max_workers=2, sleep_interval=0) as p:
             fs1 = p.submit(sleep_one, i=2)
             fs2 = p.submit(sleep_one, i=2)
             fs3 = p.submit(sleep_one, i=2)
             fs4 = p.submit(sleep_one, i=2)
@@ -81,14 +83,15 @@
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertTrue(fs1.done())
         self.assertTrue(fs1.cancelled())
+        q.join()
 
     def test_waiting(self):
         exe = PoolExecutor(max_workers=2)
         f1 = exe.submit(wait_and_calc, 42)
         f2 = exe.submit(wait_and_calc, 84)
         f1.add_done_callback(call_back)
         f2.add_done_callback(call_back)
```

### Comparing `pympipool-0.5.7/tests/test_parse.py` & `pympipool-0.5.8/tests/test_parse_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
-from pympipool.parallel_executors.mpipool import parse_arguments
-from pympipool.shared_functions.external_interfaces import command_line_options
+from pympipool.legacy.shared.backend import parse_arguments
+from pympipool.legacy.shared.interface import command_line_options
 
 
 class TestParser(unittest.TestCase):
     def test_command_local(self):
         result_dict = {
             'host': 'localhost',
             'total_cores': '2',
```

### Comparing `pympipool-0.5.7/tests/test_pool.py` & `pympipool-0.5.8/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/tests/test_queue.py` & `pympipool-0.5.8/tests/test_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from concurrent.futures import Future, CancelledError
 from queue import Queue
-from pympipool.shared_functions.external_interfaces import cancel_items_in_queue
+from pympipool.shared.taskexecutor import cancel_items_in_queue
 
 
 class TestQueue(unittest.TestCase):
     def test_cancel_items_in_queue(self):
         q = Queue()
         fs1 = Future()
         fs2 = Future()
@@ -15,7 +15,8 @@
         self.assertEqual(q.qsize(), 0)
         self.assertTrue(fs1.done())
         with self.assertRaises(CancelledError):
             self.assertTrue(fs1.result())
         self.assertTrue(fs2.done())
         with self.assertRaises(CancelledError):
             self.assertTrue(fs2.result())
+        q.join()
```

### Comparing `pympipool-0.5.7/tests/test_task.py` & `pympipool-0.5.8/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.7/tests/test_worker.py` & `pympipool-0.5.8/tests/test_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import unittest
 from queue import Queue
 from time import sleep
 from concurrent.futures import CancelledError
 from pympipool import Executor
-from pympipool.shared_functions.external_interfaces import execute_parallel_tasks, cloudpickle_register
+from pympipool.shared.taskexecutor import execute_parallel_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
@@ -84,58 +84,60 @@
             output = p.map(mpi_funct, [1, 2, 3])
         self.assertEqual(list(output), [[(1, 2, 0), (1, 2, 1)], [(2, 2, 0), (2, 2, 1)], [(3, 2, 0), (3, 2, 1)]])
 
     def test_execute_task_failed_no_argument(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {}, "future": f})
-        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         with self.assertRaises(TypeError):
             execute_parallel_tasks(
                 future_queue=q,
                 cores=1,
                 oversubscribe=False,
                 enable_flux_backend=False
             )
+        q.join()
 
     def test_execute_task_failed_wrong_argument(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"j": 4}, "future": f})
-        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         with self.assertRaises(TypeError):
             execute_parallel_tasks(
                 future_queue=q,
                 cores=1,
                 oversubscribe=False,
                 enable_flux_backend=False
             )
+        q.join()
 
     def test_execute_task(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
         q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_parallel_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array(4))
+        q.join()
 
     def test_execute_task_parallel(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
         q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_parallel_tasks(
             future_queue=q,
             cores=2,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), [np.array(4), np.array(4)])
+        q.join()
```

### Comparing `pympipool-0.5.7/tests/test_worker_memory.py` & `pympipool-0.5.8/tests/test_worker_memory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import numpy as np
 from queue import Queue
 from pympipool import Executor
-from pympipool.shared_functions.parallel_executors import call_funct
-from pympipool.shared_functions.external_interfaces import execute_parallel_tasks, cloudpickle_register
+from pympipool.shared.backend import call_funct
+from pympipool.shared.taskexecutor import execute_parallel_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def get_global(memory=None):
     return memory
 
 
@@ -39,7 +39,8 @@
         execute_parallel_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array([5]))
+        q.join()
```

### Comparing `pympipool-0.5.7/tests/test_zmq.py` & `pympipool-0.5.8/tests/test_zmq.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import zmq
-from pympipool.external_interfaces.communication import (
+from pympipool.shared.communication import (
     connect_to_socket_interface,
     close_connection,
     send_result,
     receive_instruction
 )
```

### Comparing `pympipool-0.5.7/versioneer.py` & `pympipool-0.5.8/versioneer.py`

 * *Files identical despite different names*

