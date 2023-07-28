# Comparing `tmp/benchmark_utils-0.2.1.tar.gz` & `tmp/benchmark_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmark_utils-0.2.1.tar", last modified: Wed Sep 21 14:02:32 2022, max compression
+gzip compressed data, was "benchmark_utils-0.2.3.tar", last modified: Fri Jul 28 08:35:27 2023, max compression
```

## Comparing `benchmark_utils-0.2.1.tar` & `benchmark_utils-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-09-21 14:02:32.554570 benchmark_utils-0.2.1/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2021-03-12 13:54:12.000000 benchmark_utils-0.2.1/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)     1267 2022-09-21 14:02:32.554570 benchmark_utils-0.2.1/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      606 2022-09-09 17:42:59.000000 benchmark_utils-0.2.1/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      166 2022-09-09 15:50:02.000000 benchmark_utils-0.2.1/pyproject.toml
--rw-rw-r--   0 aya       (1000) aya       (1000)      752 2022-09-21 14:02:32.554570 benchmark_utils-0.2.1/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-09-09 15:26:29.000000 benchmark_utils-0.2.1/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-09-21 14:02:32.554570 benchmark_utils-0.2.1/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-09-21 14:02:32.554570 benchmark_utils-0.2.1/src/benchmark_utils/
--rw-rw-r--   0 aya       (1000) aya       (1000)       81 2022-09-09 15:39:57.000000 benchmark_utils-0.2.1/src/benchmark_utils/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     9627 2022-09-21 14:02:11.000000 benchmark_utils-0.2.1/src/benchmark_utils/benchmark.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       42 2022-09-21 14:02:11.000000 benchmark_utils-0.2.1/src/benchmark_utils/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-09-21 14:02:32.554570 benchmark_utils-0.2.1/src/benchmark_utils.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)     1267 2022-09-21 14:02:32.000000 benchmark_utils-0.2.1/src/benchmark_utils.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      361 2022-09-21 14:02:32.000000 benchmark_utils-0.2.1/src/benchmark_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2022-09-21 14:02:32.000000 benchmark_utils-0.2.1/src/benchmark_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       57 2022-09-21 14:02:32.000000 benchmark_utils-0.2.1/src/benchmark_utils.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       16 2022-09-21 14:02:32.000000 benchmark_utils-0.2.1/src/benchmark_utils.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 08:35:27.488237 benchmark_utils-0.2.3/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2022-12-14 09:27:50.000000 benchmark_utils-0.2.3/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)     8011 2023-07-28 08:35:27.488237 benchmark_utils-0.2.3/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7347 2023-07-28 08:28:09.000000 benchmark_utils-0.2.3/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      166 2023-01-27 09:27:24.000000 benchmark_utils-0.2.3/pyproject.toml
+-rw-rw-r--   0 aya       (1000) aya       (1000)      755 2023-07-28 08:35:27.488237 benchmark_utils-0.2.3/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-12-14 09:27:50.000000 benchmark_utils-0.2.3/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 08:35:27.484237 benchmark_utils-0.2.3/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 08:35:27.484237 benchmark_utils-0.2.3/src/benchmark_utils/
+-rw-rw-r--   0 aya       (1000) aya       (1000)       81 2022-12-14 09:27:50.000000 benchmark_utils-0.2.3/src/benchmark_utils/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11434 2023-07-27 18:48:48.000000 benchmark_utils-0.2.3/src/benchmark_utils/benchmark.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       42 2023-07-28 08:28:40.000000 benchmark_utils-0.2.3/src/benchmark_utils/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 08:35:27.488237 benchmark_utils-0.2.3/src/benchmark_utils.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     8011 2023-07-28 08:35:27.000000 benchmark_utils-0.2.3/src/benchmark_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      385 2023-07-28 08:35:27.000000 benchmark_utils-0.2.3/src/benchmark_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-28 08:35:27.000000 benchmark_utils-0.2.3/src/benchmark_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       57 2023-07-28 08:35:27.000000 benchmark_utils-0.2.3/src/benchmark_utils.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       16 2023-07-28 08:35:27.000000 benchmark_utils-0.2.3/src/benchmark_utils.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 08:35:27.488237 benchmark_utils-0.2.3/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     8381 2023-07-27 13:13:08.000000 benchmark_utils-0.2.3/tests/test_benchmark.py
```

### Comparing `benchmark_utils-0.2.1/LICENSE` & `benchmark_utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmark_utils-0.2.1/setup.cfg` & `benchmark_utils-0.2.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 author_email = a.yasyrev@gmail.com
 description = Utils for benchmark.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ayasyrev/benchmark_utils
 license = apache2
 classifiers = 
-	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
```

### Comparing `benchmark_utils-0.2.1/setup.py` & `benchmark_utils-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `benchmark_utils-0.2.1/src/benchmark_utils/benchmark.py` & `benchmark_utils-0.2.3/src/benchmark_utils/benchmark.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,128 @@
+"""Wrapper over timeit to easy benchmark.
+"""
+from collections import defaultdict
+from functools import partial
 from timeit import timeit
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
-from rich import print
+from rich import print as rprint
 from rich.progress import (
-    Progress,
-    TextColumn,
     BarColumn,
+    Progress,
     TaskProgressColumn,
+    TextColumn,
     TimeRemainingColumn,
 )
 
+AnyFunc = Callable[[Union[Any, None]], Union[Any, None]]
+
 
 def benchmark(
-    name: str, func: Callable, num_repeats: int, progress_bar: Progress
+    name: str,
+    func: AnyFunc,
+    num_repeats: int,
+    progress_bar: Progress,
 ) -> List[float]:
     """Return list of run times for func, num_repeats times"""
-    run_times = []
+    run_times: List[float] = []
     text_color = "[blue]"
     task = progress_bar.add_task(f"{text_color}{name}", total=num_repeats)
     for i in range(num_repeats):
         progress_bar.tasks[
             task
         ].description = f"{text_color}{name}: run {i + 1}/{num_repeats}"
-        run_times.append(timeit(func, number=1))
+        run_times.append(timeit(func, number=1))  # type: ignore
         progress_bar.update(task, advance=1)
     run_time_avg = sum(run_times) / len(run_times)
     progress_bar.tasks[
         task
     ].description = f"{text_color}{name}: {run_time_avg:0.2f} sec/run."
     return run_times
 
 
+def get_func_name(func: AnyFunc) -> str:
+    """Return name of Callable - function ot partial"""
+    if isinstance(func, partial):
+        args = ", ".join(
+            [str(arg) for arg in func.args] + [
+                f"{k}={v}" for k, v in func.keywords.items()
+            ]
+        )
+        return f"{func.func.__name__}({args})"
+    return func.__name__
+
+
 class Benchmark:
-    """Bench func, num_repeats times"""
+    """Benchmark functions, num_repeats times"""
+
+    _max_name_len: int = 0
+    progress_bar: Progress
+    _results: Dict[str, List[float]]
+    func_dict: Dict[str, AnyFunc]
 
     def __init__(
         self,
-        func: Union[Callable, Dict[str, Callable], List[Callable]],
+        func: Union[AnyFunc, Dict[str, AnyFunc], List[AnyFunc]],
         num_repeats: int = 5,
         clear_progress: bool = True,
     ):
         self.num_repeats = num_repeats
-        self._results: Dict[str, List[float]] = {}
-        self.func_dict: Dict[str, Callable]
         if isinstance(func, dict):
             self.func_dict = func
         elif isinstance(func, list):
-            self.func_dict = {fn.__name__: fn for fn in func}
+            self.func_dict = {get_func_name(func_item): func_item for func_item in func}
         else:
-            self.func_dict = {func.__name__: func}
+            self.func_dict = {get_func_name(func): func}
         self._benchmark = benchmark
         self.results_header = " Func name  | Sec / run"
         self.clear_progress = clear_progress
+        self._reset_results()
 
     def run(
         self,
         func_name: Union[str, None, List[str]] = None,
         exclude: Union[str, List[str], None] = None,
         num_repeats: Union[int, None] = None,
     ) -> None:
+        """Run benchmark, can run only ones you need, exclude that you don't need"""
         if func_name:
             if isinstance(func_name, str):
                 func_name = [func_name]
-            func_to_test = [
-                key for key in set(self.func_dict).intersection(func_name)
-            ]
+            func_to_test = list(set(self.func_dict).intersection(func_name))
             if len(func_name) != len(func_to_test):  # something missed
                 self._print_missed(func_name)
 
         elif exclude:
             if isinstance(exclude, str):
                 exclude = [exclude]
-            func_to_test = [
-                key for key in self.func_dict
-                if key not in exclude
-            ]
+            func_to_test = [key for key in self.func_dict if key not in exclude]
             if len(exclude) != len(func_to_test):  # something missed
                 self._print_missed(exclude)
         else:
             func_to_test = list(self.func_dict)
 
         self._run(func_to_test, num_repeats)
 
     def _print_missed(self, func_names: List[str]) -> None:
         for func in func_names:
             if func not in self.func_dict:
-                print(f"{func} is not in func_dict")
+                rprint(f"{func} is not in func_dict")
 
     def _reset_results(self) -> None:
         self._results = {}  # ? if exists add new
 
     def _run(
-        self, func_names: List[str], num_repeats: Union[int, None] = None
+        self,
+        func_names: Union[List[str], Dict[str, AnyFunc]],
+        num_repeats: Union[int, None] = None,
     ) -> None:
         self._reset_results()
         if len(func_names) == 0:
-            print("Nothing to test")
+            rprint("Nothing to test")
         else:
             if num_repeats is None:
                 num_repeats = self.num_repeats
             # func_names = func_dict.keys()
             num_funcs = len(func_names)
             self._max_name_len = max(len(func_name) for func_name in func_names)
             text_color = "[green]"
@@ -109,24 +132,24 @@
                 TaskProgressColumn(),
                 TimeRemainingColumn(elapsed_when_finished=True),
                 transient=self.clear_progress,
             ) as progress_bar:
                 self.progress_bar = progress_bar
                 main_task = self.progress_bar.add_task("starting...", total=num_funcs)
                 for num, func_name in enumerate(func_names):
-                    self.progress_bar.tasks[
+                    self.progress_bar.tasks[  # pylint: disable=invalid-sequence-index
                         main_task
                     ].description = (
                         f"{text_color}running {func_name} {num + 1}/{num_funcs}"
                     )
                     self._results[func_name] = self._run_benchmark(
                         func_name, num_repeats=num_repeats
                     )
                     self.progress_bar.update(main_task, advance=1)
-                self.progress_bar.tasks[
+                self.progress_bar.tasks[  # pylint: disable=invalid-sequence-index
                     main_task
                 ].description = f"{text_color}done {num_funcs} runs."
                 columns = self.progress_bar.columns
                 self.progress_bar.columns = (
                     columns[0],
                     columns[3],
                 )  # remove BarColumn and TaskProgressColumn
@@ -147,130 +170,166 @@
     def __call__(self, num_repeats: Union[int, None] = None) -> None:
         if num_repeats is None:
             num_repeats = self.num_repeats
         self._run(self.func_dict, num_repeats)
 
     @property
     def results(self) -> Dict[str, float]:
+        """Return dict w/ results"""
         if self._results:
             return {
-                res: sum(self._results[res]) / len(self._results[res])
-                for res in self._results
+                name: sum(res_list) / len(res_list)
+                for name, res_list in self._results.items()
             }
-        else:
-            return {}
+        return {}
 
     def print_results(
-        self, results=None, results_header=None, sort=True, reverse=False, compare=True
+        self,
+        results_header: Optional[str] = None,
+        sort: bool = True,
+        reverse: bool = False,
+        compare: bool = True,
     ) -> None:
+        """Print results of benchmark"""
         self._print_results(
-            results=results,
-            results_header=None,
+            results=None,
+            results_header=results_header,
             sort=sort,
             reverse=reverse,
             compare=compare,
         )
 
     def _print_results(
         self,
-        results: Union[Dict[str, float], None] = None,
-        results_header=None,
-        sort=True,
-        reverse=False,
-        compare=False,
+        results: Optional[Dict[str, float]] = None,
+        results_header: Optional[str] = None,
+        sort: bool = True,
+        reverse: bool = False,
+        compare: bool = False,
     ) -> None:
         if results_header is None:
             results_header = self.results_header
+        rprint(results_header)
         if results is None:
             results = self.results
-        print(results_header)
-        func_names = list(results.keys())
+        func_names: list[str] = list(results.keys())
         if sort:
-            func_names = sorted(results, key=results.get, reverse=reverse)  # type: ignore
-            results = {func_name: results[func_name] for func_name in func_names}
+            func_names = sorted(func_names, key=results.get, reverse=reverse)  # type: ignore
         best_res = results[func_names[0]]
         for func_name in func_names:
             line = f"{func_name:12}: {results[func_name]:6.2f}"
             if compare:
                 line += f" {(best_res / results[func_name]) - 1:0.1%}"
-            print(line)
+            rprint(line)
 
     @property
     def func_names(self) -> str:
+        """Return func names as string"""
         return ", ".join(self.func_dict.keys())
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.func_names})"
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.func_names})"
 
 
 class BenchmarkIter(Benchmark):
     """Benchmark func over item_list"""
 
+    _num_samples: Optional[int] = None
+
     def __init__(
         self,
-        func: Union[Callable, Dict[str, Callable], List[Callable]],
+        func: Union[AnyFunc, Dict[str, AnyFunc], List[AnyFunc]],
         item_list: List[Any],
         num_repeats: int = 5,
         clear_progress: bool = True,
     ):
         super().__init__(func, num_repeats=num_repeats, clear_progress=clear_progress)
         self.item_list = item_list
-        self.exceptions: Union[Dict[str, List[Dict[str, Any]]], None] = None
+        self.exceptions: Dict[str, List[Dict[str, Any]]] = defaultdict(list)
 
     def _run_benchmark(self, func_name: str, num_repeats: int) -> List[float]:
         return self._benchmark(
             f"{func_name:{self._max_name_len}}",
             self.run_func_iter(func_name),
             num_repeats,
             self.progress_bar,
         )
 
     def _reset_results(self) -> None:
-        self.exceptions = None
+        self.exceptions = defaultdict(list)
         super()._reset_results()
 
-    def run_func_iter(self, func_name: str) -> Callable:
+    def run_func_iter(self, func_name: str) -> AnyFunc:
         """Return func, that run func over item_list"""
 
-        def inner(self=self, func_name=func_name):
+        def inner(self=self, func_name: str = func_name):
             func = self.func_dict[func_name]
+            num_samples = self._num_samples or len(self.item_list)
             task = self.progress_bar.add_task(
-                f"iterating {func_name}", total=len(self.item_list)
+                f"iterating {func_name}", total=num_samples
             )
-            for item in self.item_list:
+            for item in self.item_list[:num_samples]:
                 try:
                     func(item)
-                except Exception as excpt:
-                    if self.exceptions is None:
-                        self.exceptions = {}
+                except Exception as excpt:  # pylint: disable=broad-except
                     exception_info = {"exception": excpt, "item": item}
-                    if func_name in self.exceptions.keys():
-                        self.exceptions[func_name].append(exception_info)
-                    else:
-                        self.exceptions[func_name] = [exception_info]
+                    self.exceptions[func_name].append(exception_info)
                 self.progress_bar.update(task, advance=1)
             self.progress_bar.tasks[task].visible = False
 
         return inner
 
-    def print_results_per_item(self, sort=True, reverse=True, compare=False) -> None:
-        if self.exceptions is not None:
-            print(f"Got {len(self.exceptions)} exceptions: {', '.join(self.exceptions.keys())}.")
-        num_items = len(self.item_list)
-        results = self.results
+    def print_results_per_item(
+        self,
+        sort: bool = True,
+        reverse: bool = True,
+        compare: bool = False,
+    ) -> None:
+        """Print results per item, you can compare and sort them"""
+        if self.exceptions:
+            rprint(
+                f"Got {len(self.exceptions)} exceptions: {', '.join(self.exceptions.keys())}."
+            )
+        num_items = self._num_samples or len(self.item_list)
         results = {
-            func_name: (1 / results[func_name] * num_items) for func_name in results
+            func_name: (1 / result * num_items)
+            for func_name, result in self.results.items()
         }
         results_header = " Func name  | Items/sec"
         self._print_results(
             results=results,
             results_header=results_header,
             sort=sort,
             reverse=reverse,
             compare=compare,
         )
 
     def _after_run(self) -> None:
         self.print_results_per_item()
+
+    def __call__(
+        self,
+        num_repeats: Union[int, None] = None,
+        num_samples: Optional[int] = None,
+    ) -> None:
+        """Run benchmark - `num_repeats` times, use `num_samples` or all items."""
+        self._num_samples = num_samples
+        super().__call__(num_repeats)
+        self._num_samples = None
+
+    def run(
+        self,
+        func_name: Union[str, None, List[str]] = None,
+        exclude: Union[str, List[str], None] = None,
+        num_repeats: Union[int, None] = None,
+        num_samples: Optional[int] = None,
+    ) -> None:
+        self._num_samples = num_samples
+        super().run(
+            func_name=func_name,
+            exclude=exclude,
+            num_repeats=num_repeats,
+        )
+        self._num_samples = None
```

