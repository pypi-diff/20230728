# Comparing `tmp/datarails-0.2.2.tar.gz` & `tmp/datarails-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.2.2.tar", last modified: Fri Jul 28 13:50:03 2023, max compression
+gzip compressed data, was "datarails-0.2.3.tar", last modified: Fri Jul 28 19:22:05 2023, max compression
```

## Comparing `datarails-0.2.2.tar` & `datarails-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:50:03.254701 datarails-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:49:39.000000 datarails-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 13:49:39.000000 datarails-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:50:03.254701 datarails-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 13:49:39.000000 datarails-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 13:49:39.000000 datarails-0.2.2/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-28 13:49:39.000000 datarails-0.2.2/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 13:49:39.000000 datarails-0.2.2/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.831837 datarails-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-28 19:22:05.831837 datarails-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-28 19:21:46.000000 datarails-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.827837 datarails-0.2.3/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.827837 datarails-0.2.3/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 19:21:46.000000 datarails-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:22:05.831837 datarails-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 19:21:46.000000 datarails-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.827837 datarails-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_step.py
```

### Comparing `datarails-0.2.2/datarails/runner.py` & `datarails-0.2.3/datarails/runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from typing import Optional
+from typing import List, Optional
 
-from datarails.databox import DataBox
+from datarails.contexts import DataBox, DataRailsContext
 
 
 class StepRunner:
     """
     Class to facilitate sequential execution of steps, primarily with DataBox as input.
 
     Attributes:
         steps (list): A list of steps to be executed.
         steps_iterator (iterator): An iterator object to iterate over steps.
         dbx (DataBox): A DataBox object for data management.
     """
 
-    def __init__(self, steps: list) -> None:
+    def __init__(self, steps: List, dbx: Optional[DataBox] = None, ctx: Optional[DataRailsContext] = None) -> None:
         """
         Constructs all the necessary attributes for the StepRunner object.
 
         Args:
             steps (list): A list of steps to be executed.
         """
         self.steps = steps
         self.steps_iterator = iter(self.steps)
-        self.dbx = DataBox()
+        self.dbx = dbx or DataBox()
+        self.ctx = ctx or DataRailsContext()
 
     def reset(self):
         """
         Resets the steps_iterator to its initial state.
         """
         self.steps_iterator = iter(self.steps)
 
@@ -40,15 +41,15 @@
             execute, otherwise raises StopIteration. Defaults to True.
 
         Raises:
             StopIteration: If stepper is False and no more steps are left to execute.
         """
         try:
             step = next(self.steps_iterator)
-            step_instance = step(self.dbx)
+            step_instance = step(self.dbx, self.ctx)
             self.dbx = step_instance.run_steps()
         except StopIteration:
             if stepper:
                 print("No more steps to execute. Reset and try again.")
             else:
                 raise
```

### Comparing `datarails-0.2.2/datarails/step.py` & `datarails-0.2.3/datarails/step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Callable, Optional
 
-from datarails.databox import DataBox
+from datarails.contexts import DataBox, DataRailsContext
 
 
-class StepMeta(type):
+class _StepMeta(type):
     def __new__(cls, name, bases, attrs):
         # Create the class as normal.
         klass = super().__new__(cls, name, bases, attrs)
 
         # Add a list to the class that contains all the methods starting with 'step_'.
         # We don't include 'self' in these methods yet, because we don't have an instance.
         klass.step_methods = [k for k, v in attrs.items() if callable(v) and k.startswith("step_")]
 
         return klass
 
 
-class DataRailsStep(metaclass=StepMeta):
+class DataRailsStep(metaclass=_StepMeta):
     """
     Represents a step in a data pipeline process. This class is meant to be inherited from and not used directly.
     All methods that are declared with the prefix 'step_' on the child class will be run in order in which they are
     declared.
 
     Please check the examples directory of this repo for a more detailed example of how this class can be used.
 
@@ -27,25 +27,30 @@
         dbx (DataBox): The data box object that stores and handles data for the step.
         on_entry_callback (Callable, optional): The function to call upon entering a step. Default is None.
         on_exit_callback (Callable, optional): The function to call upon exiting a step. Default is None.
         step_method_name_generator (Generator): A generator that yields names of step methods.
     """
 
     def __init__(
-        self, dbx: DataBox, on_entry_callback: Optional[Callable] = None, on_exit_callback: Optional[Callable] = None
+        self,
+        dbx: DataBox,
+        ctx: DataRailsContext,
+        on_entry_callback: Optional[Callable] = None,
+        on_exit_callback: Optional[Callable] = None,
     ) -> None:
         """
         Constructs all the necessary attributes for the DataRailsStep object.
 
         Args:
             dbx (DataBox): The data box object that stores and handles data for the step.
             on_entry_callback (Callable, optional): The function to call upon entering a step. Default is None.
             on_exit_callback (Callable, optional): The function to call upon exiting a step. Default is None.
         """
         self.dbx = dbx
+        self.ctx = ctx
         self.step_method_name_generator = None
         self.on_entry_callback = on_entry_callback
         self.on_exit_callback = on_exit_callback
         self.reset()
 
     def __str__(self) -> str:
         """
```

### Comparing `datarails-0.2.2/pyproject.toml` & `datarails-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.2.2/tests/test_databox.py` & `datarails-0.2.3/tests/test_databox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import pytest
 
-from datarails.databox import DataBox
+from datarails.contexts import DataBox
 
 
 # This is a fixture that provides a fresh DataBox for each test that uses it.
 @pytest.fixture
 def dbx():
     return DataBox()
 
 
 def test_add_df(dbx):
     df = [1, 2, 3]  # Mock DataFrame
-    dbx.add_df("test_df", df)
+    dbx.put_df("test_df", df)
     assert hasattr(dbx, "test_df"), "DataBox should have attribute 'test_df' after adding."
     assert dbx.test_df == df, "DataBox.test_df should be equal to the added DataFrame."
 
 
 def test_get_df(dbx):
     df = [4, 5, 6]  # Mock DataFrame
-    dbx.add_df("test_df", df)
+    dbx.put_df("test_df", df)
     fetched_df = dbx.get_df("test_df")
     assert fetched_df == df, "get_df should return the added DataFrame."
 
 
 def test_pop_df(dbx):
     df = [7, 8, 9]  # Mock DataFrame
-    dbx.add_df("pop_test_df", df)
+    dbx.put_df("pop_test_df", df)
     popped_df = dbx.pop_df("pop_test_df")
     assert popped_df == df, "pop_df should return the added DataFrame."
     assert not hasattr(dbx, "pop_test_df"), "pop_test_df attribute should be deleted after popping."
 
 
 def test_delete_df(dbx):
     df = [10, 11, 12]  # Mock DataFrame
-    dbx.add_df("delete_test_df", df)
+    dbx.put_df("delete_test_df", df)
     dbx.delete_df("delete_test_df")
     assert not hasattr(dbx, "delete_test_df"), "delete_test_df attribute should be deleted."
 
 
 def test_get_df_nonexistent(dbx):
     with pytest.raises(AttributeError):
         dbx.get_df("nonexistent_df")
@@ -47,7 +47,16 @@
     with pytest.raises(AttributeError):
         dbx.pop_df("nonexistent_df")
 
 
 def test_delete_df_nonexistent(dbx):
     with pytest.raises(AttributeError):
         dbx.delete_df("nonexistent_df")
+
+
+def test_databox_constructor():
+    test_kwargs = {"test_attr_1": "test_value_1", "test_attr_2": "test_value_2", "test_attr_3": "test_value_3"}
+    context = DataBox(**test_kwargs)
+
+    for key, value in test_kwargs.items():
+        assert hasattr(context, key)
+        assert getattr(context, key) == value
```

### Comparing `datarails-0.2.2/tests/test_runner.py` & `datarails-0.2.3/tests/test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from datarails.databox import DataBox
+from datarails.contexts import DataBox
 from datarails.runner import (
     StepRunner,  # Replace with actual module where StepRunner is defined
 )
 from datarails.step import DataRailsStep
 
 
 class MockStep(DataRailsStep):
```

### Comparing `datarails-0.2.2/tests/test_step.py` & `datarails-0.2.3/tests/test_step.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pytest
 
-from datarails.databox import DataBox
+from datarails.contexts import DataBox, DataRailsContext
 from datarails.step import DataRailsStep
 
 
-class TestStep(DataRailsStep):
+class DummyStep(DataRailsStep):
     def step_one(self):
         pass
 
     def step_two(self):
         pass
 
 
 @pytest.fixture
 def test_step_instance():
     dbx = DataBox()
-    return TestStep(dbx)
+    ctx = DataRailsContext()
+    return DummyStep(dbx, ctx)
 
 
 def test_constructor(test_step_instance: DataRailsStep) -> None:
     assert test_step_instance.dbx is not None
     assert isinstance(test_step_instance.step_method_name_generator, type(iter([])))
     assert test_step_instance.step_methods == ["step_one", "step_two"]
 
@@ -52,10 +53,12 @@
     assert isinstance(dbx, DataBox)
 
 
 def test_on_entry_exit_callbacks():
     def mock_callback():
         return True
 
-    step_instance_with_callback = TestStep(DataBox(), on_entry_callback=mock_callback, on_exit_callback=mock_callback)
+    step_instance_with_callback = DummyStep(
+        DataBox(), DataRailsContext(), on_entry_callback=mock_callback, on_exit_callback=mock_callback
+    )
     assert step_instance_with_callback.on_entry_callback() == True
     assert step_instance_with_callback.on_exit_callback() == True
```

