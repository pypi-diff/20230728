# Comparing `tmp/perftester-0.6.3.tar.gz` & `tmp/perftester-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perftester-0.6.3.tar", last modified: Mon Jun 12 10:47:18 2023, max compression
+gzip compressed data, was "perftester-0.7.0.tar", last modified: Fri Jul 28 06:53:19 2023, max compression
```

## Comparing `perftester-0.6.3.tar` & `perftester-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-12 10:47:18.526709 perftester-0.6.3/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1063 2023-06-03 01:55:57.000000 perftester-0.6.3/LICENSE
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-12 10:47:18.525710 perftester-0.6.3/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-03 01:55:57.000000 perftester-0.6.3/README.md
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-12 10:47:18.486144 perftester-0.6.3/perftester/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      307 2023-06-11 02:27:34.000000 perftester-0.6.3/perftester/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5212 2023-06-03 02:47:03.000000 perftester-0.6.3/perftester/__main__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    34428 2023-06-12 10:45:09.000000 perftester-0.6.3/perftester/perftester.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-12 10:47:18.521714 perftester-0.6.3/perftester.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      303 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/entry_points.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-12 10:47:18.527709 perftester-0.6.3/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      917 2023-06-11 02:17:46.000000 perftester-0.6.3/setup.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-07-28 06:53:19.990430 perftester-0.7.0/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1063 2023-06-03 01:55:57.000000 perftester-0.7.0/LICENSE
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28607 2023-07-28 06:53:19.989429 perftester-0.7.0/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24562 2023-07-28 06:51:52.000000 perftester-0.7.0/README.md
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-07-28 06:53:19.947992 perftester-0.7.0/perftester/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      295 2023-07-28 06:47:42.000000 perftester-0.7.0/perftester/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5212 2023-06-15 06:55:33.000000 perftester-0.7.0/perftester/__main__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    34809 2023-07-28 06:47:42.000000 perftester-0.7.0/perftester/perftester.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      725 2023-06-16 02:56:05.000000 perftester-0.7.0/perftester/tmp_singleton.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-07-28 06:53:19.984877 perftester-0.7.0/perftester.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28607 2023-07-28 06:53:19.000000 perftester-0.7.0/perftester.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      331 2023-07-28 06:53:19.000000 perftester-0.7.0/perftester.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-07-28 06:53:19.000000 perftester-0.7.0/perftester.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-07-28 06:53:19.000000 perftester-0.7.0/perftester.egg-info/entry_points.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-07-28 06:53:19.000000 perftester-0.7.0/perftester.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-07-28 06:53:19.000000 perftester-0.7.0/perftester.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-07-28 06:53:19.991433 perftester-0.7.0/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      917 2023-07-28 06:47:42.000000 perftester-0.7.0/setup.py
```

### Comparing `perftester-0.6.3/LICENSE` & `perftester-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perftester-0.6.3/PKG-INFO` & `perftester-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.3
+Version: 0.7.0
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
         
@@ -413,108 +413,14 @@
         
         This does not mean, however, that raw tests are useless. In fact, in a production environment, you may wish to use raw tests. Imagine a client expects that an app never takes longer than an hour to perform a particular task (note that this strongly depends on what other processes are run in the production environment). You can create an automated test for that using `perftester`, in a very simple way - just several lines of code.
         
         You can of course combine both types of tests, and you can do it in a very simple way. Then, the test is run once, but the results are checked with raw limits and relative limits.
         
         > Warning! Relative results can be different between operating systems.
         
-        ## Tracing full memory usage
-        
-        Currently, `perftester` contains a beta version (under heavy testing) of a new feature that can be used to trace full memory usage of a Python program.
-        
-        >  Warning: Backward compatibility of this feature is not guaranteed! It does not affect the main functionality of `perftester`, however, so its backward compatibility should be kept.
-        
-        The feature works in the following way. When you import `perftester` — but you need to do it with `import perftester`, not via importing particular objects — you will be able to see new objects in the global space. One of the is `MEMLOGS`:
-        
-        ```python-repl
-        >>> import perftester
-        >>> MEMLOGS[0].ID
-        'perftester import'
-        
-        ```
-        
-        It's an empty list for the moment. When you start tracing memory using `perftester`, this list will collect the subsequent measurements. You can measure them in two ways. One is via a `MEMPOINT()` function, and another via a  `MEMTRACE` decorator. They, too, are in the global scope, so you can use them in any module inside a session in which `perftester` was already imported.
-        
-        The  `MEMLOGS` list will contain elements being instances of `MemLog`, which is a `functools.namedtuple `data type, with two attributes:`"ID"`and `"memory"`. This data type is imported with `perftester`, so if you want to use it, you can reach it as `perftester.MemLog`. You don't have to use it, though. Since it's a named tuple, you can treat it as a regular tuple.
-        
-        #### What sort of memory is measured?
-        
-        The feature uses `pympler.asizeof.asizeof(all=True)` to measure the size of all current gc objects, including module, global and stack frame objects, minus the size of `MEMLOGS`. The memory is measured in MB.
-        
-        #### Using `MEMPOINT()`
-        
-        `MEMPOINT()` creates a point of full-memory measurement. It will be appended into `MEMLOGS`.
-        
-        ```python-repl
-        3>>> import perftester
-        >>> def foo(n):
-        ...     x = [i for i in range(n)]
-        ...     MEMPOINT()
-        ...     return x
-        >>> _ = foo(100)
-        >>> _ = foo(1_000_000)
-        >>> len(MEMLOGS)
-        3
-        >>> MEMLOGS[2].memory > MEMLOGS[1].memory
-        True
-        
-        ```
-        
-        The last tests checks whether the second measurement — that is, from the function with `n` of a million — uses more memory that the function using `n` of a hundred. Makes sense, and indeed the test passes.
-        
-        When creating a point, you can use an ID, for instance, `MEMPOINT("from sth() function")`.
-        
-        `MEMPOINT()` can be used to create a point anywhere inside the code. Nevertheless, if you want to trace memory for a function, you can use a `MEMTRACE` decorator:
-        
-        ```python-repl
-        >>> @MEMTRACE
-        ... def bar(n):
-        ...     return [i for i in range(n)]
-        >>> _ = bar(1_000_000)
-        >>> MEMLOGS[-2].memory < MEMLOGS[-1].memory
-        True
-        
-        ```
-        
-        The decorator creates two points: one right before running the test and another right after returning.
-        
-        The last line tests whether memory before running the function is smaller than that after running it — and given so big `n`, it should be.
-        
-        Look here:
-        
-        ```python-repl
-        >>> @MEMTRACE
-        ... def bar(n):
-        ...     x = [i for i in range(n)]
-        ...     y = [i/3 for i in x]
-        ...     z = [i/3 for i in y]
-        ...     MEMPOINT("with x, y, z")
-        ...     del x
-        ...     MEMPOINT("without x")
-        ...     del y
-        ...     MEMPOINT("without x and y")
-        ...     del z
-        ...     MEMPOINT("without x and y and z")
-        ...     return 
-        >>> _ = bar(100_000)
-        >>> MEMLOGS[-3].memory > MEMLOGS[-2].memory > MEMLOGS[-1].memory
-        True
-        
-        ```
-        
-        ### Print `MEMLOGS`
-        
-        You can do whatever you want with `MEMLOGS`. However, when you want to see this object nicely printed, use the `MEMPRINT()` function, available from the global scope, too. You will see the results printed in a pretty way, with memory provided in MB.
-        
-        ### Why the global scope?
-        
-        Since this feature of `perftester` is to be used to debug memory use from various modules, it'd be inconvinient to import the required objects in all these modules. That's why for the moment, the required objects are kept in the global scope — but this can change in future versions.
-        
-        If you have any comments about this, please share them via Issues of the package's repository.
-        
         ## Other tools
         
         Of course, Python comes with various powerful tools for profiling, benchmarking and testing. Here are some of them:
         
         * [`cProfile` and `profile`](https://docs.python.org/3/library/profile.html), the built-in powerful tools for deterministic profiling
         * [the built-in `timeit` module](https://docs.python.org/3/library/timeit.html), for benchmarking
         * [`memory_profiler`](https://pypi.org/project/memory-profiler/), a powerful memory profiler (`memory_profiler` is utilized by `perftester`)
@@ -523,14 +429,20 @@
         
         ## Manipulating the traceback
         
         The default behavior of `perftester` is to **not** include the full traceback when a test does not pass. This is because when running performance tests, you're not interested in finding bugs, and this is what traceback is for. Instead, you want to see which test did not pass and how.
         
         > This behavior will not affect any other function than the two `perftester` testing functions: `pt.time_test()` and `pt.memory_usage_test()`. If you want to use this behavior for other functions, too, you can use `pt.config.cut_traceback()`; to reverse, use `pt.config.full_traceback()`.
         
+        ## Tracing full memory usage → Moved to `tracemem`
+        
+        Since the `0.5.*` versions, `perftester` contained a beta version of a memory tracer that could be used to trace full memory usage of a Python session.
+        
+        Since `perftester` requires some memory to load, it over-measured session memory. In order to avoid this, this feature was moved to a separate Python package, called `tracemem`. You can install it from [PyPi](https://pypi.org/project/tracemem/), and you will find its Git repository [here](https://github.com/nyggus/tracemem).
+        
         ## Caveats
         
         * `perftester` does not work with multiple threads or processes.
         * `perftester` is still in a beta version and so is still under testing.
         * Watch out when you're running the same test in different operating systems. Even relative tests can differ from OS to OS.
         
         ## Operating systems
```

### Comparing `perftester-0.6.3/README.md` & `perftester-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -405,108 +405,14 @@
 
 This does not mean, however, that raw tests are useless. In fact, in a production environment, you may wish to use raw tests. Imagine a client expects that an app never takes longer than an hour to perform a particular task (note that this strongly depends on what other processes are run in the production environment). You can create an automated test for that using `perftester`, in a very simple way - just several lines of code.
 
 You can of course combine both types of tests, and you can do it in a very simple way. Then, the test is run once, but the results are checked with raw limits and relative limits.
 
 > Warning! Relative results can be different between operating systems.
 
-## Tracing full memory usage
-
-Currently, `perftester` contains a beta version (under heavy testing) of a new feature that can be used to trace full memory usage of a Python program.
-
->  Warning: Backward compatibility of this feature is not guaranteed! It does not affect the main functionality of `perftester`, however, so its backward compatibility should be kept.
-
-The feature works in the following way. When you import `perftester` — but you need to do it with `import perftester`, not via importing particular objects — you will be able to see new objects in the global space. One of the is `MEMLOGS`:
-
-```python-repl
->>> import perftester
->>> MEMLOGS[0].ID
-'perftester import'
-
-```
-
-It's an empty list for the moment. When you start tracing memory using `perftester`, this list will collect the subsequent measurements. You can measure them in two ways. One is via a `MEMPOINT()` function, and another via a  `MEMTRACE` decorator. They, too, are in the global scope, so you can use them in any module inside a session in which `perftester` was already imported.
-
-The  `MEMLOGS` list will contain elements being instances of `MemLog`, which is a `functools.namedtuple `data type, with two attributes:`"ID"`and `"memory"`. This data type is imported with `perftester`, so if you want to use it, you can reach it as `perftester.MemLog`. You don't have to use it, though. Since it's a named tuple, you can treat it as a regular tuple.
-
-#### What sort of memory is measured?
-
-The feature uses `pympler.asizeof.asizeof(all=True)` to measure the size of all current gc objects, including module, global and stack frame objects, minus the size of `MEMLOGS`. The memory is measured in MB.
-
-#### Using `MEMPOINT()`
-
-`MEMPOINT()` creates a point of full-memory measurement. It will be appended into `MEMLOGS`.
-
-```python-repl
-3>>> import perftester
->>> def foo(n):
-...     x = [i for i in range(n)]
-...     MEMPOINT()
-...     return x
->>> _ = foo(100)
->>> _ = foo(1_000_000)
->>> len(MEMLOGS)
-3
->>> MEMLOGS[2].memory > MEMLOGS[1].memory
-True
-
-```
-
-The last tests checks whether the second measurement — that is, from the function with `n` of a million — uses more memory that the function using `n` of a hundred. Makes sense, and indeed the test passes.
-
-When creating a point, you can use an ID, for instance, `MEMPOINT("from sth() function")`.
-
-`MEMPOINT()` can be used to create a point anywhere inside the code. Nevertheless, if you want to trace memory for a function, you can use a `MEMTRACE` decorator:
-
-```python-repl
->>> @MEMTRACE
-... def bar(n):
-...     return [i for i in range(n)]
->>> _ = bar(1_000_000)
->>> MEMLOGS[-2].memory < MEMLOGS[-1].memory
-True
-
-```
-
-The decorator creates two points: one right before running the test and another right after returning.
-
-The last line tests whether memory before running the function is smaller than that after running it — and given so big `n`, it should be.
-
-Look here:
-
-```python-repl
->>> @MEMTRACE
-... def bar(n):
-...     x = [i for i in range(n)]
-...     y = [i/3 for i in x]
-...     z = [i/3 for i in y]
-...     MEMPOINT("with x, y, z")
-...     del x
-...     MEMPOINT("without x")
-...     del y
-...     MEMPOINT("without x and y")
-...     del z
-...     MEMPOINT("without x and y and z")
-...     return 
->>> _ = bar(100_000)
->>> MEMLOGS[-3].memory > MEMLOGS[-2].memory > MEMLOGS[-1].memory
-True
-
-```
-
-### Print `MEMLOGS`
-
-You can do whatever you want with `MEMLOGS`. However, when you want to see this object nicely printed, use the `MEMPRINT()` function, available from the global scope, too. You will see the results printed in a pretty way, with memory provided in MB.
-
-### Why the global scope?
-
-Since this feature of `perftester` is to be used to debug memory use from various modules, it'd be inconvinient to import the required objects in all these modules. That's why for the moment, the required objects are kept in the global scope — but this can change in future versions.
-
-If you have any comments about this, please share them via Issues of the package's repository.
-
 ## Other tools
 
 Of course, Python comes with various powerful tools for profiling, benchmarking and testing. Here are some of them:
 
 * [`cProfile` and `profile`](https://docs.python.org/3/library/profile.html), the built-in powerful tools for deterministic profiling
 * [the built-in `timeit` module](https://docs.python.org/3/library/timeit.html), for benchmarking
 * [`memory_profiler`](https://pypi.org/project/memory-profiler/), a powerful memory profiler (`memory_profiler` is utilized by `perftester`)
@@ -515,14 +421,20 @@
 
 ## Manipulating the traceback
 
 The default behavior of `perftester` is to **not** include the full traceback when a test does not pass. This is because when running performance tests, you're not interested in finding bugs, and this is what traceback is for. Instead, you want to see which test did not pass and how.
 
 > This behavior will not affect any other function than the two `perftester` testing functions: `pt.time_test()` and `pt.memory_usage_test()`. If you want to use this behavior for other functions, too, you can use `pt.config.cut_traceback()`; to reverse, use `pt.config.full_traceback()`.
 
+## Tracing full memory usage → Moved to `tracemem`
+
+Since the `0.5.*` versions, `perftester` contained a beta version of a memory tracer that could be used to trace full memory usage of a Python session.
+
+Since `perftester` requires some memory to load, it over-measured session memory. In order to avoid this, this feature was moved to a separate Python package, called `tracemem`. You can install it from [PyPi](https://pypi.org/project/tracemem/), and you will find its Git repository [here](https://github.com/nyggus/tracemem).
+
 ## Caveats
 
 * `perftester` does not work with multiple threads or processes.
 * `perftester` is still in a beta version and so is still under testing.
 * Watch out when you're running the same test in different operating systems. Even relative tests can differ from OS to OS.
 
 ## Operating systems
```

### Comparing `perftester-0.6.3/perftester/__main__.py` & `perftester-0.7.0/perftester/__main__.py`

 * *Files identical despite different names*

### Comparing `perftester-0.6.3/perftester/perftester.py` & `perftester-0.7.0/perftester/perftester.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 WARNING: Unlike memory_profiler.memory_usage(), which reports memory in MiB,
 perftester provides data in MB. That way, the data from 
 memory_profiler.memory_usage() and pympler.asizeof.asizeof() are provided in
 the same units. If you want to recalculate the data to MiB, you can divide the
 memory by perftester.MiB_TO_MB_FACTOR.
 
+WARNING: Calculating memory can take quite some time when the 
+
 For the sake of pretty-printing the benchmarks, perftester comes with a pp
 function, which rounds all numbers to four significant digits and prints
 the object using pprint.pprint:
 >>> import perftester as pt
 >>> pt.pp([2.1212, 2.93135])
 [2.121, 2.931]
 
@@ -28,69 +30,79 @@
 >>> pt.config.digits_for_printing = 2
 >>> pt.pp([2.1212, 2.93135])
 [2.1, 2.9]
 
 Let's return to previous settings:
 >>> pt.config.digits_for_printing = 4
 """
+import warnings
+from pympler.asizeof import asizeof
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    STARTING_MEMORY = asizeof(all=True)
+
 import builtins
 import copy
+import inspect
+import gc
 import os
 import rounder
 import sys
 import timeit
-import warnings
 
 from collections import namedtuple
 from collections.abc import Callable
 from easycheck import (
     check_argument,
     check_if,
     check_if_not,
-    check_instance,
+    check_type,
     check_if_paths_exist,
-    assert_instance, # required for doctests
+    assert_instance,  # required for doctests
 )
 from functools import wraps
 from memory_profiler import memory_usage
 from pathlib import Path
 from pprint import pprint
-from pympler.asizeof import asizeof
 from statistics import mean
 
 
 MiB_TO_MB_FACTOR = 1.048576
 
 
+class IncorrectUseOfMEMLOGSError(Exception):
+    """MEMLOGS was used incorrectly."""
+
+
 class CLIPathError(Exception):
     """Exception class to be used for the CLI perftester app."""
 
 
 class LogFilePathError(Exception):
-    """Exception class to be used when incorrect path is provided for a log file."""
+    """Incorrect path provided for a log file."""
 
 
 class LackingLimitsError(Exception):
-    """Exception class to be used when no limits are set for a test."""
+    """No limits has been set for test."""
 
 
 class IncorrectArgumentError(Exception):
-    """Exception class to be used when function args are incorrect."""
+    """Function arguments are incorrect."""
 
 
 class TimeTestError(Exception):
-    """Exception class to be used when time_test() does not pass."""
+    """The time test has not passed."""
 
 
 class MemoryTestError(Exception):
-    """Exception class to be used when memory_usage_test() does not pass."""
+    """The memory usage test has not passed."""
 
 
 class FunctionError(Exception):
-    """Exception class to be used when the tested code throws an error."""
+    """The tested code has thrown an error."""
 
 
 # Configuration
 
 
 class Config:
     """Default configuration for testing.
@@ -139,28 +151,28 @@
 
     @property
     def digits_for_printing(self):
         return self._digits_for_printing
 
     @digits_for_printing.setter
     def digits_for_printing(self, value):
-        check_instance(
+        check_type(
             value,
             int,
             message=f"Argument value must be an int, not {type(value).__name__}",
         )
         self._digits_for_printing = value
 
     @property
     def log_to_file(self):
         return self._log_to_file
 
     @log_to_file.setter
     def log_to_file(self, value):
-        check_instance(
+        check_type(
             value,
             bool,
             message=f"Argument value must be an int, not {type(value).__name__}",
         )
         self._log_to_file = value
 
     @property
@@ -220,15 +232,15 @@
             func (Callable): a callable for which the setting is to be changed
             which (str): either "time" or "memory", for which the setting is
                 to be changed
             item (str): either "repeat" or "number"
         """
         whiches = ("time", "memory")
         items = ("number", "repeat")
-        check_instance(
+        check_type(
             func,
             Callable,
             IncorrectArgumentError,
             message="Argument func must be a callable.",
         )
         check_argument(
             which,
@@ -293,15 +305,17 @@
         Returns:
             float: the minimum maximum memory usage over time across all runs.
         """
         memory_results = [
             memory_usage((self.benchmark_function, (), {}))
             for _ in range(self.defaults["memory"]["repeat"])
         ]
-        self.memory_benchmark = MiB_TO_MB_FACTOR * min(max(r) for r in memory_results)
+        self.memory_benchmark = MiB_TO_MB_FACTOR * min(
+            max(r) for r in memory_results
+        )
 
     def set_defaults(
         self, which, number=None, repeat=None, Number=None, Repeat=None
     ):
         """Change the default settings.
 
         Beware! This does not change particular settings for a particular test,
@@ -367,15 +381,15 @@
         # Below, which must be "memory"; this is checked by ._check_args() above,
         # so we do not have to worry about that here.
         if repeat is not None:
             self.settings[func][which]["repeat"] = repeat
 
     def _check_args(self, func, which, number, repeat):
         """Check instances of arguments func, which, number and repeat."""
-        check_instance(
+        check_type(
             func,
             Callable,
             IncorrectArgumentError,
             message=(
                 "Argument func must be an int (or None), not "
                 f"{type(func).__name__}"
             ),
@@ -401,24 +415,24 @@
 
         if number is not None:
             if int(number) == number:
                 number = int(number)
         if repeat is not None:
             if int(repeat) == repeat:
                 repeat = int(repeat)
-        check_instance(
+        check_type(
             number,
             (int, None),
             IncorrectArgumentError,
             message=(
                 "Argument number must be an int (or None), not "
                 f"{type(number).__name__}"
             ),
         )
-        check_instance(
+        check_type(
             repeat,
             (int, None),
             IncorrectArgumentError,
             message=(
                 "Argument repeat must be an int (or None), not "
                 f"{type(repeat).__name__}"
             ),
@@ -613,15 +627,15 @@
     a limit for a relative test (against a function defined in the config);
     then use raw_limit=None. But you can also use both at the same time, and
     the tests passes only when both the raw and the relative tests pass.
 
     When you use Repeat, it has a higher priority than the corresponding
     setting from config.settings, and it will be used. This is used in this
     single call only, and so it does not overwrite the config settings.
-    
+
     WARNING: Unlike memory_profiler.memory_usage(), which reports memory in MiB,
     perftester provides data in MB.
 
     Args:
         func (Callable): the tested function.
         raw_limit (float): raw limit for the test. It is the maximum memory
             that the function can use; if it's exceeded, the test does not pass.
@@ -657,15 +671,15 @@
     dict_keys(['raw_results', 'relative_results', 'mean_result_per_run', 'max_result_per_run', 'max_result_per_run_relative', 'mean', 'max', 'max_relative'])
     >>> type(first_run['raw_results'])
     <class 'list'>
     >>> first_run['mean'] < first_run['max']
     True
     >>> memory_usage_test(sum1, raw_limit=first_run['max']*2, n=100_000)
     """
-    check_instance(
+    check_type(
         func,
         Callable,
         IncorrectArgumentError,
         "Argument func must be a callable.",
     )
     check_if_not(
         raw_limit is None and relative_limit is None,
@@ -682,23 +696,23 @@
             message=(
                 f"Memory test not passed for function {func.__name__}:\n"
                 f"memory_limit = {raw_limit}\n"
                 f"maximum memory usage = {rounder.signif(results['max'], config.digits_for_printing)}"
             ),
         )
     if relative_limit is not None:
-        relatve_got_memory = results["max"] / config.memory_benchmark
+        relative_got_memory = results["max"] / config.memory_benchmark
         check_if(
-            relatve_got_memory <= relative_limit,
+            relative_got_memory <= relative_limit,
             handle_with=MemoryTestError,
             message=(
                 f"Memory test not passed for function {func.__name__}:\n"
                 f"relative memory limit = {relative_limit}\n"
                 f"maximum obtained relative memory usage = "
-                f"{rounder.signif(relatve_got_memory, config.digits_for_printing)}"
+                f"{rounder.signif(relative_got_memory, config.digits_for_printing)}"
             ),
         )
     config.full_traceback()
 
 
 def memory_usage_benchmark(func, *args, Repeat=None, **kwargs):
     """Run memory benchmarks for a callable.
@@ -710,15 +724,15 @@
     be added to config.settings.
 
     When you use Repeat, it has a higher priority than the corresponding
     setting from config.settings, and it will be used. This is used in this
     single call only, and so it does not overwrite the config settings.
 
     The function returns a dict that you can pretty-print using function pp().
-    
+
     WARNING: Unlike memory_profiler.memory_usage(), which reports memory in MiB,
     perftester provides data in MB.
 
     Args:
         func (Callable): a function (or a callable) to run benchmarks for
         Repeat (int): a repeat setting, overwriting (for this function call)
             the setting in config.settings[func]["memory"]["repeat"]
@@ -729,47 +743,41 @@
             memory_usage_test()
 
     >>> def f(x): return x
     >>> f_bench = memory_usage_benchmark(f, x=10)
     >>> f_bench.keys()
     dict_keys(['raw_results', 'relative_results', 'mean_result_per_run', 'max_result_per_run', 'max_result_per_run_relative', 'mean', 'max', 'max_relative'])
     """
-    check_instance(func, Callable, message="Argument func must be a callable.")
+    check_type(func, Callable, message="Argument func must be a callable.")
     _add_func_to_config(func)
 
     n = Repeat or config.settings[func]["memory"]["repeat"]
 
     try:
-        memory_results = [
-            memory_usage((func, args, kwargs))
-            for i in range(n)
-        ]
+        memory_results = [memory_usage((func, args, kwargs)) for i in range(n)]
     except Exception as e:
         raise FunctionError(
             f"The tested function raised {type(e).__name__}: {str(e)}"
         )
 
     for i, result in enumerate(memory_results):
         for j, _ in enumerate(result):
             memory_results[i][j] *= MiB_TO_MB_FACTOR
 
-    memory_results_mean = [
-        mean(this_result)
-        for this_result in memory_results
-    ]
+    memory_results_mean = [mean(this_result) for this_result in memory_results]
     memory_results_max = [max(this_result) for this_result in memory_results]
     overall_mean = mean(memory_results_mean)
     # We take the min of the max values
     overall_max = min(memory_results_max)
 
     relative_results = copy.deepcopy(memory_results)
     for i, result in enumerate(relative_results):
         for j, r in enumerate(result):
             relative_results[i][j] = r / config.memory_benchmark
-            
+
     return {
         "raw_results": memory_results,
         "relative_results": relative_results,
         "mean_result_per_run": memory_results_mean,
         "max_result_per_run": memory_results_max,
         "max_result_per_run_relative": [
             r / config.memory_benchmark for r in memory_results_max
@@ -817,15 +825,15 @@
     Of course, we do have to remember that the execution time can depend on
     the function's arguments:
     >>> def f(n): return list(range(n))
     >>> time_benchmark(f, n=1000)["min"] > time_benchmark(f, n=1)["min"]
     True
 
     """
-    check_instance(func, Callable, message="Argument func must be a callable.")
+    check_type(func, Callable, message="Argument func must be a callable.")
     _add_func_to_config(func)
 
     try:
         results = _repeat(func, *args, Number=Number, Repeat=Repeat, **kwargs)
     except Exception as e:
         raise FunctionError(
             f"The tested function raised {type(e).__name__}: {str(e)}"
@@ -857,96 +865,106 @@
     line break used as a separator.
 
     >>> pp(.122242)
     0.1222
     >>> pp(dict(a=.12121212, b=23.234234234), ["system failure", 345345.345])
     {'a': 0.1212, 'b': 23.23}
     ['system failure', 345300.0]
+    >>> t = time_benchmark(lambda: 0, Number=1, Repeat=1)
+    >>> pp(t)
+    Time data are printed in seconds.
+    {'max': ...,
+     'mean': ...,
+     'min': ...,
+     'min_relative': ...,
+     'raw_times': [...],
+     'raw_times_relative': [...]}
+    >>> m = memory_usage_benchmark(lambda: 0)
+    >>> pp(m)
+    Memory data are printed in MB.
+    {'max': ...,
+     'max_relative': ...,
+     'max_result_per_run': [...],
+     'max_result_per_run_relative': [...],
+     'mean': ...,
+     'mean_result_per_run': [...],
+     'raw_results': [[..., ..., ...]],
+     'relative_results': [[..., ..., ...]]}
     """
     for arg in args:
+        is_benchmark = _check_if_benchmarks(arg)
+        if is_benchmark == "time benchmark":
+            print("Time data are printed in seconds.")
+        elif is_benchmark == "memory benchmark":
+            print("Memory data are printed in MB.")
         pprint(
             rounder.signif_object(
                 arg, digits=config.digits_for_printing, use_copy=True
             )
         )
 
 
+def _check_if_benchmarks(obj):
+    """Check if obj comes from time or memory benchmarks.
+
+    >>> _check_if_benchmarks(10)
+    >>> _check_if_benchmarks("10")
+    >>> _check_if_benchmarks([10, ])
+    >>> _check_if_benchmarks((10, ))
+    >>> _check_if_benchmarks({10, 20})
+    >>> _check_if_benchmarks(dict(x=10, y=20))
+    >>> t = time_benchmark(lambda: 0, Number=1, Repeat=1)
+    >>> m = memory_usage_benchmark(lambda: 0)
+    >>> _check_if_benchmarks(t)
+    'time benchmark'
+    >>> _check_if_benchmarks(m)
+    'memory benchmark'
+    """
+    time_keys = {
+        "min",
+        "min_relative",
+        "raw_times",
+        "raw_times_relative",
+        "mean",
+        "max",
+    }
+    memory_keys = {
+        "raw_results",
+        "relative_results",
+        "mean_result_per_run",
+        "max_result_per_run",
+        "max_result_per_run_relative",
+        "mean",
+        "max",
+        "max_relative",
+    }
+    try:
+        if obj.keys() == time_keys:
+            return "time benchmark"
+    except AttributeError:
+        pass
+    try:
+        if obj.keys() == memory_keys:
+            return "memory benchmark"
+    except AttributeError:
+        return None
+
+
 def _add_func_to_config(func):
     if func not in config.settings.keys():
         config.settings[func] = {}
         config.settings[func]["time"] = dict(
             number=config.defaults["time"]["number"],
             repeat=config.defaults["time"]["repeat"],
         )
         config.settings[func]["memory"] = dict(
             repeat=config.defaults["memory"]["repeat"],
         )
 
 
-# Full memory measurement
-
-builtins.__dict__["MEMLOGS"] = []
-
-
-MemLog = namedtuple("MemLog", "ID memory")
-
-
-def MEMPRINT():
-    """Pretty-print MEMLOGS."""
-    for i, memlog in enumerate(MEMLOGS):  # type: ignore
-        ID = memlog.ID if memlog.ID else ""
-        print(
-            f"{i: < 4} "
-            f"{round(memlog.memory / 1024/1024, 1): <6} → "
-            f"{ID}"
-        )
-
-
-def MEMPOINT(ID=None):
-    """Global function to measure full memory and log it into MEMLOGS.
-
-    The function is available from any module of a session. It logs into
-    MEMLOGS, also available from any module.
-
-    Memory is collected using pympler.asizeof.asizeof(), and reported in
-    bytes. So, the function measures the size of all current gc objects,
-    including module, global and stack frame objects, minus the size
-    of `MEMLOGS`.
-    """
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        MEMLOGS.append(
-            MemLog(  # type: ignore
-                ID, (asizeof(all=True) - asizeof(MEMLOGS))
-            )  # type: ignore
-        )
-
-
-def MEMTRACE(func, ID_before=None, ID_after=None):
-    """Decorator to log memory before and after running a function."""
-
-    @wraps(func)
-    def inner(*args, **kwargs):
-        before = ID_before if ID_before else f"Before {func.__name__}()"
-        MEMPOINT(before)
-        f = func(*args, **kwargs)
-        after = ID_after if ID_after else f"After {func.__name__}()"
-        MEMPOINT(after)
-        return f
-
-    return inner
-
-
-builtins.__dict__["MEMPOINT"] = MEMPOINT
-builtins.__dict__["MEMPRINT"] = MEMPRINT
-builtins.__dict__["MEMTRACE"] = MEMTRACE
-
-MEMPOINT("perftester import")
-
-
 if __name__ == "__main__":
     import doctest
 
     flags = flags = (
         doctest.ELLIPSIS
         | doctest.NORMALIZE_WHITESPACE
         | doctest.IGNORE_EXCEPTION_DETAIL
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `perftester-0.6.3/perftester.egg-info/PKG-INFO` & `perftester-0.7.0/perftester.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.3
+Version: 0.7.0
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
         
@@ -413,108 +413,14 @@
         
         This does not mean, however, that raw tests are useless. In fact, in a production environment, you may wish to use raw tests. Imagine a client expects that an app never takes longer than an hour to perform a particular task (note that this strongly depends on what other processes are run in the production environment). You can create an automated test for that using `perftester`, in a very simple way - just several lines of code.
         
         You can of course combine both types of tests, and you can do it in a very simple way. Then, the test is run once, but the results are checked with raw limits and relative limits.
         
         > Warning! Relative results can be different between operating systems.
         
-        ## Tracing full memory usage
-        
-        Currently, `perftester` contains a beta version (under heavy testing) of a new feature that can be used to trace full memory usage of a Python program.
-        
-        >  Warning: Backward compatibility of this feature is not guaranteed! It does not affect the main functionality of `perftester`, however, so its backward compatibility should be kept.
-        
-        The feature works in the following way. When you import `perftester` — but you need to do it with `import perftester`, not via importing particular objects — you will be able to see new objects in the global space. One of the is `MEMLOGS`:
-        
-        ```python-repl
-        >>> import perftester
-        >>> MEMLOGS[0].ID
-        'perftester import'
-        
-        ```
-        
-        It's an empty list for the moment. When you start tracing memory using `perftester`, this list will collect the subsequent measurements. You can measure them in two ways. One is via a `MEMPOINT()` function, and another via a  `MEMTRACE` decorator. They, too, are in the global scope, so you can use them in any module inside a session in which `perftester` was already imported.
-        
-        The  `MEMLOGS` list will contain elements being instances of `MemLog`, which is a `functools.namedtuple `data type, with two attributes:`"ID"`and `"memory"`. This data type is imported with `perftester`, so if you want to use it, you can reach it as `perftester.MemLog`. You don't have to use it, though. Since it's a named tuple, you can treat it as a regular tuple.
-        
-        #### What sort of memory is measured?
-        
-        The feature uses `pympler.asizeof.asizeof(all=True)` to measure the size of all current gc objects, including module, global and stack frame objects, minus the size of `MEMLOGS`. The memory is measured in MB.
-        
-        #### Using `MEMPOINT()`
-        
-        `MEMPOINT()` creates a point of full-memory measurement. It will be appended into `MEMLOGS`.
-        
-        ```python-repl
-        3>>> import perftester
-        >>> def foo(n):
-        ...     x = [i for i in range(n)]
-        ...     MEMPOINT()
-        ...     return x
-        >>> _ = foo(100)
-        >>> _ = foo(1_000_000)
-        >>> len(MEMLOGS)
-        3
-        >>> MEMLOGS[2].memory > MEMLOGS[1].memory
-        True
-        
-        ```
-        
-        The last tests checks whether the second measurement — that is, from the function with `n` of a million — uses more memory that the function using `n` of a hundred. Makes sense, and indeed the test passes.
-        
-        When creating a point, you can use an ID, for instance, `MEMPOINT("from sth() function")`.
-        
-        `MEMPOINT()` can be used to create a point anywhere inside the code. Nevertheless, if you want to trace memory for a function, you can use a `MEMTRACE` decorator:
-        
-        ```python-repl
-        >>> @MEMTRACE
-        ... def bar(n):
-        ...     return [i for i in range(n)]
-        >>> _ = bar(1_000_000)
-        >>> MEMLOGS[-2].memory < MEMLOGS[-1].memory
-        True
-        
-        ```
-        
-        The decorator creates two points: one right before running the test and another right after returning.
-        
-        The last line tests whether memory before running the function is smaller than that after running it — and given so big `n`, it should be.
-        
-        Look here:
-        
-        ```python-repl
-        >>> @MEMTRACE
-        ... def bar(n):
-        ...     x = [i for i in range(n)]
-        ...     y = [i/3 for i in x]
-        ...     z = [i/3 for i in y]
-        ...     MEMPOINT("with x, y, z")
-        ...     del x
-        ...     MEMPOINT("without x")
-        ...     del y
-        ...     MEMPOINT("without x and y")
-        ...     del z
-        ...     MEMPOINT("without x and y and z")
-        ...     return 
-        >>> _ = bar(100_000)
-        >>> MEMLOGS[-3].memory > MEMLOGS[-2].memory > MEMLOGS[-1].memory
-        True
-        
-        ```
-        
-        ### Print `MEMLOGS`
-        
-        You can do whatever you want with `MEMLOGS`. However, when you want to see this object nicely printed, use the `MEMPRINT()` function, available from the global scope, too. You will see the results printed in a pretty way, with memory provided in MB.
-        
-        ### Why the global scope?
-        
-        Since this feature of `perftester` is to be used to debug memory use from various modules, it'd be inconvinient to import the required objects in all these modules. That's why for the moment, the required objects are kept in the global scope — but this can change in future versions.
-        
-        If you have any comments about this, please share them via Issues of the package's repository.
-        
         ## Other tools
         
         Of course, Python comes with various powerful tools for profiling, benchmarking and testing. Here are some of them:
         
         * [`cProfile` and `profile`](https://docs.python.org/3/library/profile.html), the built-in powerful tools for deterministic profiling
         * [the built-in `timeit` module](https://docs.python.org/3/library/timeit.html), for benchmarking
         * [`memory_profiler`](https://pypi.org/project/memory-profiler/), a powerful memory profiler (`memory_profiler` is utilized by `perftester`)
@@ -523,14 +429,20 @@
         
         ## Manipulating the traceback
         
         The default behavior of `perftester` is to **not** include the full traceback when a test does not pass. This is because when running performance tests, you're not interested in finding bugs, and this is what traceback is for. Instead, you want to see which test did not pass and how.
         
         > This behavior will not affect any other function than the two `perftester` testing functions: `pt.time_test()` and `pt.memory_usage_test()`. If you want to use this behavior for other functions, too, you can use `pt.config.cut_traceback()`; to reverse, use `pt.config.full_traceback()`.
         
+        ## Tracing full memory usage → Moved to `tracemem`
+        
+        Since the `0.5.*` versions, `perftester` contained a beta version of a memory tracer that could be used to trace full memory usage of a Python session.
+        
+        Since `perftester` requires some memory to load, it over-measured session memory. In order to avoid this, this feature was moved to a separate Python package, called `tracemem`. You can install it from [PyPi](https://pypi.org/project/tracemem/), and you will find its Git repository [here](https://github.com/nyggus/tracemem).
+        
         ## Caveats
         
         * `perftester` does not work with multiple threads or processes.
         * `perftester` is still in a beta version and so is still under testing.
         * Watch out when you're running the same test in different operating systems. Even relative tests can differ from OS to OS.
         
         ## Operating systems
```

### Comparing `perftester-0.6.3/setup.py` & `perftester-0.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 extras_requirements = {
     "dev": ["wheel", "black"],
 }
 
 setuptools.setup(
     name="perftester",
-    version="0.6.3",
+    version="0.7.0",
     author="Nyggus",
     author_email="nyggus@gmail.com",
     description="Lightweight performance testing in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyggus/perftester",
     packages=setuptools.find_packages(),
```

