# Comparing `tmp/logtalk-jupyter-kernel-0.3.0.tar.gz` & `tmp/logtalk-jupyter-kernel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logtalk-jupyter-kernel-0.3.0.tar", last modified: Mon Jul 17 09:31:32 2023, max compression
+gzip compressed data, was "logtalk-jupyter-kernel-0.4.0.tar", last modified: Fri Jul 28 09:14:01 2023, max compression
```

## Comparing `logtalk-jupyter-kernel-0.3.0.tar` & `logtalk-jupyter-kernel-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.638483 logtalk-jupyter-kernel-0.3.0/
--rw-r--r--   0 pmoura     (501) staff       (20)     1129 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/LICENSE
--rw-r--r--   0 pmoura     (501) staff       (20)      164 2023-02-15 15:11:09.000000 logtalk-jupyter-kernel-0.3.0/MANIFEST.in
--rw-r--r--   0 pmoura     (501) staff       (20)    16472 2023-07-17 09:31:32.638671 logtalk-jupyter-kernel-0.3.0/PKG-INFO
--rw-r--r--   0 pmoura     (501) staff       (20)    14295 2023-07-15 19:06:11.000000 logtalk-jupyter-kernel-0.3.0/README.md
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.626451 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/
--rw-r--r--   0 pmoura     (501) staff       (20)    16472 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/PKG-INFO
--rw-r--r--   0 pmoura     (501) staff       (20)     1207 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 pmoura     (501) staff       (20)        1 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 pmoura     (501) staff       (20)       97 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/requires.txt
--rw-r--r--   0 pmoura     (501) staff       (20)       32 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/top_level.txt
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.629099 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/
--rw-r--r--   0 pmoura     (501) staff       (20)     1497 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__init__.py
--rw-r--r--   0 pmoura     (501) staff       (20)     1526 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__main__.py
--rw-r--r--   0 pmoura     (501) staff       (20)     3388 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/install.py
--rw-r--r--   0 pmoura     (501) staff       (20)    29462 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernel.py
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.629486 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernelspec/
--rw-r--r--   0 pmoura     (501) staff       (20)     4957 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernelspec/kernel.js
--rw-r--r--   0 pmoura     (501) staff       (20)    30599 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_base_implementation.py
--rw-r--r--   0 pmoura     (501) staff       (20)     8218 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_config.py
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.635172 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/
--rw-r--r--   0 pmoura     (501) staff       (20)    16216 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    14513 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     2733 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     4393 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    13945 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    13816 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     5875 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_server.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    62311 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     7583 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     2111 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/loader.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     8264 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/sicstus_kernel_implementation.py
--rw-r--r--   0 pmoura     (501) staff       (20)     3854 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/swi_kernel_implementation.py
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.636977 logtalk-jupyter-kernel-0.3.0/notebooks/
--rw-r--r--   0 pmoura     (501) staff       (20)    45691 2023-07-17 09:09:11.000000 logtalk-jupyter-kernel-0.3.0/notebooks/JupyterKernelForLogtalkOverview.ipynb
--rw-r--r--   0 pmoura     (501) staff       (20)    44419 2023-02-09 20:56:59.000000 logtalk-jupyter-kernel-0.3.0/notebooks/LogtalkTutorial.ipynb
--rw-r--r--   0 pmoura     (501) staff       (20)     1156 2023-07-17 09:23:37.000000 logtalk-jupyter-kernel-0.3.0/pyproject.toml
--rw-r--r--   0 pmoura     (501) staff       (20)      200 2023-07-17 09:31:32.639206 logtalk-jupyter-kernel-0.3.0/setup.cfg
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-28 09:14:01.514371 logtalk-jupyter-kernel-0.4.0/
+-rw-r--r--   0 pmoura     (501) staff       (20)     1129 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/LICENSE
+-rw-r--r--   0 pmoura     (501) staff       (20)      164 2023-02-15 15:11:09.000000 logtalk-jupyter-kernel-0.4.0/MANIFEST.in
+-rw-r--r--   0 pmoura     (501) staff       (20)    16472 2023-07-28 09:14:01.514625 logtalk-jupyter-kernel-0.4.0/PKG-INFO
+-rw-r--r--   0 pmoura     (501) staff       (20)    14295 2023-07-15 19:06:11.000000 logtalk-jupyter-kernel-0.4.0/README.md
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-28 09:14:01.507164 logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/
+-rw-r--r--   0 pmoura     (501) staff       (20)    16472 2023-07-28 09:14:01.000000 logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 pmoura     (501) staff       (20)     1207 2023-07-28 09:14:01.000000 logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 pmoura     (501) staff       (20)        1 2023-07-28 09:14:01.000000 logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 pmoura     (501) staff       (20)       97 2023-07-28 09:14:01.000000 logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/requires.txt
+-rw-r--r--   0 pmoura     (501) staff       (20)       32 2023-07-28 09:14:01.000000 logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/top_level.txt
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-28 09:14:01.509531 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/
+-rw-r--r--   0 pmoura     (501) staff       (20)     1497 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/__init__.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     1526 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/__main__.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     3388 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/install.py
+-rw-r--r--   0 pmoura     (501) staff       (20)    29462 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/kernel.py
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-28 09:14:01.509873 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/kernelspec/
+-rw-r--r--   0 pmoura     (501) staff       (20)     4957 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/kernelspec/kernel.js
+-rw-r--r--   0 pmoura     (501) staff       (20)    30599 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_kernel_base_implementation.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     8218 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_kernel_config.py
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-28 09:14:01.513208 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/
+-rw-r--r--   0 pmoura     (501) staff       (20)    16216 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    14513 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     2733 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     4393 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    13945 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    13816 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     5615 2023-07-28 09:00:54.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_server.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    62326 2023-07-28 08:58:48.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     7583 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     2111 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/loader.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     8264 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/sicstus_kernel_implementation.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     3854 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.4.0/logtalk_kernel/swi_kernel_implementation.py
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-28 09:14:01.514014 logtalk-jupyter-kernel-0.4.0/notebooks/
+-rw-r--r--   0 pmoura     (501) staff       (20)    45691 2023-07-17 09:09:11.000000 logtalk-jupyter-kernel-0.4.0/notebooks/JupyterKernelForLogtalkOverview.ipynb
+-rw-r--r--   0 pmoura     (501) staff       (20)    44419 2023-02-09 20:56:59.000000 logtalk-jupyter-kernel-0.4.0/notebooks/LogtalkTutorial.ipynb
+-rw-r--r--   0 pmoura     (501) staff       (20)     1156 2023-07-28 09:05:46.000000 logtalk-jupyter-kernel-0.4.0/pyproject.toml
+-rw-r--r--   0 pmoura     (501) staff       (20)      200 2023-07-28 09:14:01.515280 logtalk-jupyter-kernel-0.4.0/setup.cfg
```

### Comparing `logtalk-jupyter-kernel-0.3.0/LICENSE` & `logtalk-jupyter-kernel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/PKG-INFO` & `logtalk-jupyter-kernel-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logtalk-jupyter-kernel
-Version: 0.3.0
+Version: 0.4.0
 Summary: Hercutalk - A Jupyter Kernel for Logtalk
 Author: Paulo Moura, Anne Brecklinghaus, Michael Leuschel, dgelessus
 License: Copyright (c) 2022-2023 Paulo Moura  
         Copyright (c) 2022 Anne Brecklinghaus, Michael Leuschel, dgelessus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `logtalk-jupyter-kernel-0.3.0/README.md` & `logtalk-jupyter-kernel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/PKG-INFO` & `logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logtalk-jupyter-kernel
-Version: 0.3.0
+Version: 0.4.0
 Summary: Hercutalk - A Jupyter Kernel for Logtalk
 Author: Paulo Moura, Anne Brecklinghaus, Michael Leuschel, dgelessus
 License: Copyright (c) 2022-2023 Paulo Moura  
         Copyright (c) 2022 Anne Brecklinghaus, Michael Leuschel, dgelessus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt` & `logtalk-jupyter-kernel-0.4.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__init__.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__main__.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/install.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/install.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernel.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernelspec/kernel.js` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/kernelspec/kernel.js`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_base_implementation.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_kernel_base_implementation.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_config.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_kernel_config.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_server.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_server.lgt`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 % The requests and corresponding replies are JSON-RPC 2.0 (https://www.jsonrpc.org/specification) messages sent over the standard streams.
 % The handling of those is based on code from 'jsonrpc_server.pl' from SICStus 4.5.1
 
 
 :- object(jupyter_server).
 
 	:- info([
-		version is 0:1:0,
+		version is 0:2:0,
 		author is 'Anne Brecklinghaus, Michael Leuschel, and Paulo Moura',
-		date is 2022-11-23,
+		date is 2023-07-28,
 		comment is 'Main object of the server.'
 	]).
 
 	:- public(start/0).
 	:- mode(start, one).
 	:- info(start/0, [
 		comment is 'Starts the server at the default verbosity level (1).'
@@ -58,24 +58,18 @@
 	:- uses(jupyter_term_handling, [assert_sld_data/4]).
 	:- uses(jupyter_preferences, [set_preference/2]).
 
 	start :-
 		start(1).
 
 	start(JupyterKernelVerbosityLevel) :-
-		setup,
-		set_preference(verbosity,JupyterKernelVerbosityLevel), % useful for testing purposes
+		set_preference(verbosity, JupyterKernelVerbosityLevel), % useful for testing purposes
 		% Start the loop handling requests from the client
 		loop(continue, [], _ContOut).
 
-	setup :-
-		% The tests in jupyter_server_tests.pl need to be started without printing informational messages
-		% In order for those messages to be printed during an execution, a corresponding Prolog flag has to be set
-		set_logtalk_flag(report, on).
-
 	:- multifile(logtalk::trace_event/2).
 	:- dynamic(logtalk::trace_event/2).
 
 	% the Logtalk runtime calls all defined logtalk::trace_event/2 hooks using
 	% a failure-driven loop; thus we don't have to worry about handling all
 	% events or failing after handling an event to give other hooks a chance
 	logtalk::trace_event(top_goal(Goal, _), _) :-
```

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt`

 * *Files 0% similar despite different names*

```diff
@@ -101,19 +101,20 @@
 	%
 	% Bindings is a list of Name=Var pairs, where Name is the name of a variable Var occurring in the term Term.
 	% Check which type of term Term is and handle it accordingly.
 	% Queries
 	handle_term(Query, CallRequestId, Stack, Bindings, Cont) :-
 		handle_query_term(Query, CallRequestId, Stack, Bindings, continue, Cont).
 
-	format_to_atom(_,_,Atom) :-
-		get_preference(verbosity,L), L < 2,
+	format_to_atom(_, _, Atom) :-
+		get_preference(verbosity, Level),
+		Level < 2,
 		!,
 		Atom = ''.
-	format_to_atom(Msg,Args,Atom) :-
+	format_to_atom(Msg, Args, Atom) :-
 		format_to_codes(Msg, Args, Codes),
 		atom_codes(Atom, Codes).
 
 
 	% Queries
 
 	% In case of any other query not handled by any of the predicates defined above, the query is called by jupyter_query_handling::call_query_with_output_to_file/7.
```

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/loader.lgt` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/logtalk_server/loader.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/sicstus_kernel_implementation.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/sicstus_kernel_implementation.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/swi_kernel_implementation.py` & `logtalk-jupyter-kernel-0.4.0/logtalk_kernel/swi_kernel_implementation.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/notebooks/JupyterKernelForLogtalkOverview.ipynb` & `logtalk-jupyter-kernel-0.4.0/notebooks/JupyterKernelForLogtalkOverview.ipynb`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/notebooks/LogtalkTutorial.ipynb` & `logtalk-jupyter-kernel-0.4.0/notebooks/LogtalkTutorial.ipynb`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.3.0/pyproject.toml` & `logtalk-jupyter-kernel-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.0"
 ]
 
 [project]
 name = "logtalk-jupyter-kernel"
-version = "0.3.0"
+version = "0.4.0"
 authors = [ {name="Paulo Moura"}, { name="Anne Brecklinghaus" }, { name="Michael Leuschel" }, { name="dgelessus" } ]
 description = "Hercutalk - A Jupyter Kernel for Logtalk"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
   "Development Status :: 4 - Beta",
```

