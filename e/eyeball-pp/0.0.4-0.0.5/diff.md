# Comparing `tmp/eyeball_pp-0.0.4.tar.gz` & `tmp/eyeball_pp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.4.tar", last modified: Thu Jul 27 05:25:10 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.5.tar", last modified: Fri Jul 28 06:34:15 2023, max compression
```

## Comparing `eyeball_pp-0.0.4.tar` & `eyeball_pp-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-27 05:25:10.454950 eyeball_pp-0.0.4/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.4/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-27 05:25:10.455108 eyeball_pp-0.0.4/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8520 2023-07-12 19:49:37.000000 eyeball_pp-0.0.4/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-27 05:25:10.441351 eyeball_pp-0.0.4/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.4/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     2307 2023-07-13 18:39:56.000000 eyeball_pp-0.0.4/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.4/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.4/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    39726 2023-07-27 05:16:31.000000 eyeball_pp-0.0.4/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    36797 2023-07-27 05:09:22.000000 eyeball_pp-0.0.4/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)      728 2023-07-26 18:52:02.000000 eyeball_pp-0.0.4/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-27 05:25:10.454599 eyeball_pp-0.0.4/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-27 05:25:10.000000 eyeball_pp-0.0.4/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-27 05:25:10.000000 eyeball_pp-0.0.4/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-27 05:25:10.000000 eyeball_pp-0.0.4/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-27 05:25:10.000000 eyeball_pp-0.0.4/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-27 05:25:10.455935 eyeball_pp-0.0.4/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.4/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-28 06:34:15.066982 eyeball_pp-0.0.5/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.5/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-28 06:34:15.067147 eyeball_pp-0.0.5/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8520 2023-07-12 19:49:37.000000 eyeball_pp-0.0.5/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-28 06:34:15.065050 eyeball_pp-0.0.5/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.5/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     2307 2023-07-13 18:39:56.000000 eyeball_pp-0.0.5/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.5/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.5/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    40130 2023-07-28 06:25:03.000000 eyeball_pp-0.0.5/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    36960 2023-07-28 05:50:48.000000 eyeball_pp-0.0.5/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)      728 2023-07-26 18:52:02.000000 eyeball_pp-0.0.5/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-28 06:34:15.066717 eyeball_pp-0.0.5/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-28 06:34:15.067987 eyeball_pp-0.0.5/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.5/setup.py
```

### Comparing `eyeball_pp-0.0.4/LICENSE` & `eyeball_pp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.4/PKG-INFO` & `eyeball_pp-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `eyeball_pp-0.0.4/README.md` & `eyeball_pp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.4/eyeball_pp/__init__.py` & `eyeball_pp-0.0.5/eyeball_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.4/eyeball_pp/classes.py` & `eyeball_pp-0.0.5/eyeball_pp/classes.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.4/eyeball_pp/comparators.py` & `eyeball_pp-0.0.5/eyeball_pp/comparators.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.4/eyeball_pp/eval.py` & `eyeball_pp-0.0.5/eyeball_pp/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 from contextlib import contextmanager
 from enum import Enum
 import inspect
 import json
 import os
+import types
 from .recorders import (
     ApiClientRecorder,
     Checkpoint,
     ComparisonResult,
     DiskRecorder,
     FileRecorder,
     MemoryRecorder,
@@ -99,38 +100,48 @@
     RATE_EXAMPLES = "rate_examples"
 
 
 class Evaluator:
     def __init__(self, **config_kwargs) -> None:
         self.config = EvaluatorConfig()
         self.mode: EvaluatorMode = EvaluatorMode.RECORD
-        self.current_recorder_state = threading.local()
+        self.running_in_notebook = False
+        try:
+            get_ipython()  # type: ignore
+            self.running_in_notebook = True
+            self.current_recorder_state = types.SimpleNamespace()
+        except NameError:
+            self.current_recorder_state = threading.local()  # type: ignore
         self.set_config(**config_kwargs)
 
     def _get_config(self, **override_config_kwargs) -> EvaluatorConfig:
         return EvaluatorConfig._merge(self.config, **override_config_kwargs)
 
     def set_config(self, **config_kwargs) -> None:
         self.config = EvaluatorConfig._merge(self.config, **config_kwargs)
         self.data_dir = os.path.join(self.config.dir_path, "eyeball_data")
         if self.config.api_key is not None:
             self.recorder: EvalRecorder = ApiClientRecorder(
                 api_key=self.config.api_key, api_url=self.config.api_url
             )
+        elif self.running_in_notebook:
+            self.recorder = MemoryRecorder()
         else:
             self.recorder = FileRecorder(self.data_dir)
 
     @contextmanager
     def start_recording_session(
         self,
         task_name: str,
         checkpoint_id: Optional[str] = None,
         checkpoint_id_to_rerun: Optional[str] = None,
     ) -> Iterator[None]:
-        if hasattr(self.current_recorder_state, "recorder_checkpoint_id"):
+        if not self.running_in_notebook and hasattr(
+            self.current_recorder_state, "recorder_checkpoint_id"
+        ):
             # This should not happen but if it does, we should not overwrite the previous checkpoint id
             # Instead we should set it to None so there is no confusion
             # If the user calls get_eval_params this will raise an error
             self.current_recorder_state.task_name = None
             self.current_recorder_state.recorder_checkpoint_id = None
             self.current_recorder_state.checkpoint_id_to_rerun = None
             yield None
```

### Comparing `eyeball_pp-0.0.4/eyeball_pp/recorders.py` & `eyeball_pp-0.0.5/eyeball_pp/recorders.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,14 +635,20 @@
         task = self.tasks[task_name]
         if input_hash not in task.input_hashes:
             return
         for checkpoint_id in task.input_hashes[input_hash]:
             del task.checkpoints[checkpoint_id]
         del task.input_hashes[input_hash]
 
+    def edit_checkpoint(
+        self, task_name: str, checkpoint_id: str, edit_dict: dict[str, Any]
+    ) -> None:
+        # TODO: implement
+        return None
+
 
 class FileRecorder(EvalRecorder):
     def __init__(self, dir_path: str) -> None:
         self.dir_path = dir_path
         if not os.path.exists(self.dir_path):
             os.makedirs(self.dir_path)
         self.yaml_dicts: dict[str, dict[str, str]] = {}
```

### Comparing `eyeball_pp-0.0.4/eyeball_pp/utils.py` & `eyeball_pp-0.0.5/eyeball_pp/utils.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.4/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.5/eyeball_pp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball-pp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `eyeball_pp-0.0.4/setup.cfg` & `eyeball_pp-0.0.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eyeball_pp
-version = 0.0.4
+version = 0.0.5
 description = A python package for evaluating tasks which use llms
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Revant
 author_email = revant.kapoor@gmail.com
 url = https://github.com/revantk/eyeball-plus-plus
 license_files = LICENSE
```

