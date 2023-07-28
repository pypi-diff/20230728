# Comparing `tmp/casavo-log-formatter-1.0.1.tar.gz` & `tmp/casavo-log-formatter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casavo-log-formatter-1.0.1.tar", last modified: Fri Jul 28 15:20:02 2023, max compression
+gzip compressed data, was "casavo-log-formatter-1.0.2.tar", last modified: Fri Jul 28 15:26:18 2023, max compression
```

## Comparing `casavo-log-formatter-1.0.1.tar` & `casavo-log-formatter-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:20:02.345241 casavo-log-formatter-1.0.1/
--rw-r--r--   0 giorgio    (501) staff       (20)     1072 2023-06-07 08:54:51.000000 casavo-log-formatter-1.0.1/LICENSE.txt
--rw-r--r--   0 giorgio    (501) staff       (20)     3344 2023-07-28 15:20:02.345097 casavo-log-formatter-1.0.1/PKG-INFO
--rw-r--r--   0 giorgio    (501) staff       (20)     1190 2023-07-28 15:19:38.000000 casavo-log-formatter-1.0.1/README.md
--rw-r--r--   0 giorgio    (501) staff       (20)     1609 2023-06-26 06:28:55.000000 casavo-log-formatter-1.0.1/pyproject.toml
--rw-r--r--   0 giorgio    (501) staff       (20)       38 2023-07-28 15:20:02.345277 casavo-log-formatter-1.0.1/setup.cfg
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:20:02.343342 casavo-log-formatter-1.0.1/src/
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:20:02.343995 casavo-log-formatter-1.0.1/src/casavo_log_formatter/
--rw-r--r--   0 giorgio    (501) staff       (20)       22 2023-07-28 15:19:51.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter/__init__.py
--rw-r--r--   0 giorgio    (501) staff       (20)     2475 2023-06-26 06:33:20.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter/formatters.py
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:20:02.344732 casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/
--rw-r--r--   0 giorgio    (501) staff       (20)     3344 2023-07-28 15:20:02.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/PKG-INFO
--rw-r--r--   0 giorgio    (501) staff       (20)      376 2023-07-28 15:20:02.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 giorgio    (501) staff       (20)        1 2023-07-28 15:20:02.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 giorgio    (501) staff       (20)       85 2023-07-28 15:20:02.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/requires.txt
--rw-r--r--   0 giorgio    (501) staff       (20)       21 2023-07-28 15:20:02.000000 casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/top_level.txt
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:20:02.344875 casavo-log-formatter-1.0.1/tests/
--rw-r--r--   0 giorgio    (501) staff       (20)    10499 2023-06-26 06:39:39.000000 casavo-log-formatter-1.0.1/tests/test_formatters.py
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:26:18.873948 casavo-log-formatter-1.0.2/
+-rw-r--r--   0 giorgio    (501) staff       (20)     1072 2023-06-07 08:54:51.000000 casavo-log-formatter-1.0.2/LICENSE.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)     3495 2023-07-28 15:26:18.873821 casavo-log-formatter-1.0.2/PKG-INFO
+-rw-r--r--   0 giorgio    (501) staff       (20)     1341 2023-07-28 15:25:37.000000 casavo-log-formatter-1.0.2/README.md
+-rw-r--r--   0 giorgio    (501) staff       (20)     1609 2023-06-26 06:28:55.000000 casavo-log-formatter-1.0.2/pyproject.toml
+-rw-r--r--   0 giorgio    (501) staff       (20)       38 2023-07-28 15:26:18.873979 casavo-log-formatter-1.0.2/setup.cfg
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:26:18.872320 casavo-log-formatter-1.0.2/src/
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:26:18.872940 casavo-log-formatter-1.0.2/src/casavo_log_formatter/
+-rw-r--r--   0 giorgio    (501) staff       (20)       22 2023-07-28 15:23:47.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter/__init__.py
+-rw-r--r--   0 giorgio    (501) staff       (20)     2475 2023-06-26 06:33:20.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter/formatters.py
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:26:18.873520 casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/
+-rw-r--r--   0 giorgio    (501) staff       (20)     3495 2023-07-28 15:26:18.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 giorgio    (501) staff       (20)      376 2023-07-28 15:26:18.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)        1 2023-07-28 15:26:18.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)       85 2023-07-28 15:26:18.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/requires.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)       21 2023-07-28 15:26:18.000000 casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/top_level.txt
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2023-07-28 15:26:18.873651 casavo-log-formatter-1.0.2/tests/
+-rw-r--r--   0 giorgio    (501) staff       (20)    10499 2023-06-26 06:39:39.000000 casavo-log-formatter-1.0.2/tests/test_formatters.py
```

### Comparing `casavo-log-formatter-1.0.1/LICENSE.txt` & `casavo-log-formatter-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `casavo-log-formatter-1.0.1/PKG-INFO` & `casavo-log-formatter-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casavo-log-formatter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A pre-configured JSON formatter for the Casavo logging format
 Author-email: Casavo <tech.internals@casavo.com>
 Maintainer-email: Casavo <tech.internals@casavo.com>
 License: Copyright 2023 Casavo Management S.p.A.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -30,14 +30,18 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # casavo-log-formatter
 
 An utility library that exposes a pre-configured log formatter for the Casavo JSON logging format.
 
+## Installation
+
+`pip install casavo-log-formatter`, or `pip install casavo-log-formatter[orjson]` if you prefer using `orjson` as a json serializer.
+
 ## Usage
 
 Referring to https://docs.python.org/3/library/logging.config.html#logging-config-dictschema,
 we suggest to configure your logging `dictConfig` by adding those 2 keys:
 
 ```python
 formatters = {
```

### Comparing `casavo-log-formatter-1.0.1/README.md` & `casavo-log-formatter-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # casavo-log-formatter
 
 An utility library that exposes a pre-configured log formatter for the Casavo JSON logging format.
 
+## Installation
+
+`pip install casavo-log-formatter`, or `pip install casavo-log-formatter[orjson]` if you prefer using `orjson` as a json serializer.
+
 ## Usage
 
 Referring to https://docs.python.org/3/library/logging.config.html#logging-config-dictschema,
 we suggest to configure your logging `dictConfig` by adding those 2 keys:
 
 ```python
 formatters = {
```

### Comparing `casavo-log-formatter-1.0.1/pyproject.toml` & `casavo-log-formatter-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `casavo-log-formatter-1.0.1/src/casavo_log_formatter/formatters.py` & `casavo-log-formatter-1.0.2/src/casavo_log_formatter/formatters.py`

 * *Files identical despite different names*

### Comparing `casavo-log-formatter-1.0.1/src/casavo_log_formatter.egg-info/PKG-INFO` & `casavo-log-formatter-1.0.2/src/casavo_log_formatter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casavo-log-formatter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A pre-configured JSON formatter for the Casavo logging format
 Author-email: Casavo <tech.internals@casavo.com>
 Maintainer-email: Casavo <tech.internals@casavo.com>
 License: Copyright 2023 Casavo Management S.p.A.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -30,14 +30,18 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # casavo-log-formatter
 
 An utility library that exposes a pre-configured log formatter for the Casavo JSON logging format.
 
+## Installation
+
+`pip install casavo-log-formatter`, or `pip install casavo-log-formatter[orjson]` if you prefer using `orjson` as a json serializer.
+
 ## Usage
 
 Referring to https://docs.python.org/3/library/logging.config.html#logging-config-dictschema,
 we suggest to configure your logging `dictConfig` by adding those 2 keys:
 
 ```python
 formatters = {
```

### Comparing `casavo-log-formatter-1.0.1/tests/test_formatters.py` & `casavo-log-formatter-1.0.2/tests/test_formatters.py`

 * *Files identical despite different names*

