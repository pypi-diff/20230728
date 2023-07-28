# Comparing `tmp/z3log-1.0.3.tar.gz` & `tmp/z3log-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z3log-1.0.3.tar", last modified: Fri Jul 28 21:03:54 2023, max compression
+gzip compressed data, was "dist/z3log-1.0.4.tar", last modified: Fri Jul 28 21:08:24 2023, max compression
```

## Comparing `z3log-1.0.3.tar` & `z3log-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:03:54.394183 z3log-1.0.3/
--rw-rw-r--   0 morell    (1001) morell    (1001)    35149 2023-06-14 13:43:45.000000 z3log-1.0.3/LICENSE
--rw-rw-r--   0 morell    (1001) morell    (1001)      587 2023-07-28 21:03:54.394183 z3log-1.0.3/PKG-INFO
--rw-rw-r--   0 morell    (1001) morell    (1001)        8 2023-06-14 13:43:45.000000 z3log-1.0.3/README.md
-drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:03:54.394183 z3log-1.0.3/Z3Log/
--rw-rw-r--   0 morell    (1001) morell    (1001)        2 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/__init__.py
--rw-rw-r--   0 morell    (1001) morell    (1001)     4586 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/argument.py
-drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:03:54.394183 z3log-1.0.3/Z3Log/config/
--rw-rw-r--   0 morell    (1001) morell    (1001)        2 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/config/__init__.py
--rw-rw-r--   0 morell    (1001) morell    (1001)     1552 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/config/config.py
--rw-rw-r--   0 morell    (1001) morell    (1001)      804 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/config/path.py
--rw-rw-r--   0 morell    (1001) morell    (1001)    19738 2023-07-28 20:12:22.000000 z3log-1.0.3/Z3Log/graph.py
--rw-rw-r--   0 morell    (1001) morell    (1001)    13745 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/result.py
--rw-rw-r--   0 morell    (1001) morell    (1001)     1657 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/specs.py
--rw-rw-r--   0 morell    (1001) morell    (1001)     3731 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/stats.py
--rw-rw-r--   0 morell    (1001) morell    (1001)     4583 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/testbench.py
--rw-rw-r--   0 morell    (1001) morell    (1001)     2144 2023-06-14 13:43:45.000000 z3log-1.0.3/Z3Log/utils.py
--rw-rw-r--   0 morell    (1001) morell    (1001)    20123 2023-06-14 14:32:46.000000 z3log-1.0.3/Z3Log/verilog.py
--rw-rw-r--   0 morell    (1001) morell    (1001)    70405 2023-07-28 20:08:57.000000 z3log-1.0.3/Z3Log/z3solver.py
--rw-rw-r--   0 morell    (1001) morell    (1001)       38 2023-07-28 21:03:54.394183 z3log-1.0.3/setup.cfg
--rw-rw-r--   0 morell    (1001) morell    (1001)     1742 2023-07-28 20:13:55.000000 z3log-1.0.3/setup.py
-drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:03:54.394183 z3log-1.0.3/z3log.egg-info/
--rw-rw-r--   0 morell    (1001) morell    (1001)      587 2023-07-28 21:03:54.000000 z3log-1.0.3/z3log.egg-info/PKG-INFO
--rw-rw-r--   0 morell    (1001) morell    (1001)      405 2023-07-28 21:03:54.000000 z3log-1.0.3/z3log.egg-info/SOURCES.txt
--rw-rw-r--   0 morell    (1001) morell    (1001)        1 2023-07-28 21:03:54.000000 z3log-1.0.3/z3log.egg-info/dependency_links.txt
--rw-rw-r--   0 morell    (1001) morell    (1001)      352 2023-07-28 21:03:54.000000 z3log-1.0.3/z3log.egg-info/requires.txt
--rw-rw-r--   0 morell    (1001) morell    (1001)        6 2023-07-28 21:03:54.000000 z3log-1.0.3/z3log.egg-info/top_level.txt
+drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:08:24.836934 z3log-1.0.4/
+-rw-rw-r--   0 morell    (1001) morell    (1001)    35149 2023-06-14 13:43:45.000000 z3log-1.0.4/LICENSE
+-rw-rw-r--   0 morell    (1001) morell    (1001)      587 2023-07-28 21:08:24.836934 z3log-1.0.4/PKG-INFO
+-rw-rw-r--   0 morell    (1001) morell    (1001)        8 2023-06-14 13:43:45.000000 z3log-1.0.4/README.md
+drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:08:24.836934 z3log-1.0.4/Z3Log/
+-rw-rw-r--   0 morell    (1001) morell    (1001)        2 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/__init__.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)     4586 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/argument.py
+drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:08:24.836934 z3log-1.0.4/Z3Log/config/
+-rw-rw-r--   0 morell    (1001) morell    (1001)        2 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/config/__init__.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)     1552 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/config/config.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)      804 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/config/path.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)    19770 2023-07-28 21:07:58.000000 z3log-1.0.4/Z3Log/graph.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)    13745 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/result.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)     1657 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/specs.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)     3731 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/stats.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)     4583 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/testbench.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)     2144 2023-06-14 13:43:45.000000 z3log-1.0.4/Z3Log/utils.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)    20123 2023-06-14 14:32:46.000000 z3log-1.0.4/Z3Log/verilog.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)    70405 2023-07-28 20:08:57.000000 z3log-1.0.4/Z3Log/z3solver.py
+-rw-rw-r--   0 morell    (1001) morell    (1001)       38 2023-07-28 21:08:24.836934 z3log-1.0.4/setup.cfg
+-rw-rw-r--   0 morell    (1001) morell    (1001)     1742 2023-07-28 21:08:06.000000 z3log-1.0.4/setup.py
+drwxrwxr-x   0 morell    (1001) morell    (1001)        0 2023-07-28 21:08:24.836934 z3log-1.0.4/z3log.egg-info/
+-rw-rw-r--   0 morell    (1001) morell    (1001)      587 2023-07-28 21:08:24.000000 z3log-1.0.4/z3log.egg-info/PKG-INFO
+-rw-rw-r--   0 morell    (1001) morell    (1001)      405 2023-07-28 21:08:24.000000 z3log-1.0.4/z3log.egg-info/SOURCES.txt
+-rw-rw-r--   0 morell    (1001) morell    (1001)        1 2023-07-28 21:08:24.000000 z3log-1.0.4/z3log.egg-info/dependency_links.txt
+-rw-rw-r--   0 morell    (1001) morell    (1001)      352 2023-07-28 21:08:24.000000 z3log-1.0.4/z3log.egg-info/requires.txt
+-rw-rw-r--   0 morell    (1001) morell    (1001)        6 2023-07-28 21:08:24.000000 z3log-1.0.4/z3log.egg-info/top_level.txt
```

### Comparing `z3log-1.0.3/LICENSE` & `z3log-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/PKG-INFO` & `z3log-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3log
-Version: 1.0.3
+Version: 1.0.4
 Summary: Paper Title: ErrorEval: an Open-Source Worst-Case-Error Evaluation Framework for Approximate Computing
 Author: Morteza Rezaalipour (MorellRAP)
 Author-email: <rezaalipour.usi@gmail.com>
 Keywords: python,verilog,circuits,synthesis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `z3log-1.0.3/Z3Log/argument.py` & `z3log-1.0.4/Z3Log/argument.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/config/config.py` & `z3log-1.0.4/Z3Log/config/config.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/config/path.py` & `z3log-1.0.4/Z3Log/config/path.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/graph.py` & `z3log-1.0.4/Z3Log/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,24 +147,24 @@
         return self.__sorted_node_list
 
     def set_sorted_node_list(self, sorted_node_list):
         self.__sorted_node_list = sorted_node_list
 
     def remove_output_outgoing_edges(self):
         for n in self.graph.nodes:
-        if self.is_cleaned_po(n):
-            if len(list(self.graph.successors(n))) > 0:
+            if self.is_cleaned_po(n):
+                if len(list(self.graph.successors(n))) > 0:
 
-                if len(list(self.graph.predecessors(n))) > 1:
-                    raise Exception(Fore.RED + f'Output {n} has more than 1 predecessors!' + Style.RESET_ALL)
+                    if len(list(self.graph.predecessors(n))) > 1:
+                        raise Exception(Fore.RED + f'Output {n} has more than 1 predecessors!' + Style.RESET_ALL)
 
-                pred = list(self.graph.predecessors(n))[0]
-                for s in list(self.graph.successors(n)):
-                    self.graph.remove_edge(n, s)
-                    self.graph.add_edge(pred, s)
+                    pred = list(self.graph.predecessors(n))[0]
+                    for s in list(self.graph.successors(n)):
+                        self.graph.remove_edge(n, s)
+                        self.graph.add_edge(pred, s)
 
     def extract_inputs(self):
         # print(f'Extracting inputs...')
         input_dict = {}
         idx = 0
         for n in self.graph.nodes():
             if self.is_pi(n):
```

### Comparing `z3log-1.0.3/Z3Log/result.py` & `z3log-1.0.4/Z3Log/result.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/specs.py` & `z3log-1.0.4/Z3Log/specs.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/stats.py` & `z3log-1.0.4/Z3Log/stats.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/testbench.py` & `z3log-1.0.4/Z3Log/testbench.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/utils.py` & `z3log-1.0.4/Z3Log/utils.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/verilog.py` & `z3log-1.0.4/Z3Log/verilog.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/Z3Log/z3solver.py` & `z3log-1.0.4/Z3Log/z3solver.py`

 * *Files identical despite different names*

### Comparing `z3log-1.0.3/setup.py` & `z3log-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = """
 Paper Title: ErrorEval: an Open-Source Worst-Case-Error Evaluation Framework for Approximate Computing
 
 Short Description: The open-source toolchain that proposes a methodology called ErrorEval which relies on 
 SMT (Satisfiability Modulo Theories) solvers.
 
 Authors:
```

### Comparing `z3log-1.0.3/z3log.egg-info/PKG-INFO` & `z3log-1.0.4/z3log.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3log
-Version: 1.0.3
+Version: 1.0.4
 Summary: Paper Title: ErrorEval: an Open-Source Worst-Case-Error Evaluation Framework for Approximate Computing
 Author: Morteza Rezaalipour (MorellRAP)
 Author-email: <rezaalipour.usi@gmail.com>
 Keywords: python,verilog,circuits,synthesis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

