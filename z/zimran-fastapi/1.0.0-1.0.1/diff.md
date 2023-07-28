# Comparing `tmp/zimran-fastapi-1.0.0.tar.gz` & `tmp/zimran-fastapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-fastapi-1.0.0.tar", last modified: Wed Jul 26 07:17:56 2023, max compression
+gzip compressed data, was "zimran-fastapi-1.0.1.tar", last modified: Fri Jul 28 10:09:14 2023, max compression
```

## Comparing `zimran-fastapi-1.0.0.tar` & `zimran-fastapi-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:17:56.582755 zimran-fastapi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-26 07:17:56.582755 zimran-fastapi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-26 07:17:45.000000 zimran-fastapi-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:17:56.582755 zimran-fastapi-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-26 07:17:45.000000 zimran-fastapi-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:17:56.582755 zimran-fastapi-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 07:17:45.000000 zimran-fastapi-1.0.0/tests/test_health_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:17:56.578755 zimran-fastapi-1.0.0/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:17:56.582755 zimran-fastapi-1.0.0/zimran/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-26 07:17:45.000000 zimran-fastapi-1.0.0/zimran/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:17:56.582755 zimran-fastapi-1.0.0/zimran_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-26 07:17:56.000000 zimran-fastapi-1.0.0/zimran_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 07:17:56.000000 zimran-fastapi-1.0.0/zimran_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:17:56.000000 zimran-fastapi-1.0.0/zimran_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 07:17:56.000000 zimran-fastapi-1.0.0/zimran_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 07:17:56.000000 zimran-fastapi-1.0.0/zimran_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:09:14.622876 zimran-fastapi-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-28 10:09:14.622876 zimran-fastapi-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 10:09:03.000000 zimran-fastapi-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:09:14.622876 zimran-fastapi-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 10:09:03.000000 zimran-fastapi-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:09:14.618876 zimran-fastapi-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 10:09:03.000000 zimran-fastapi-1.0.1/tests/test_check_trailing_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 10:09:03.000000 zimran-fastapi-1.0.1/tests/test_health_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:09:14.618876 zimran-fastapi-1.0.1/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:09:14.618876 zimran-fastapi-1.0.1/zimran/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 10:09:03.000000 zimran-fastapi-1.0.1/zimran/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:09:14.622876 zimran-fastapi-1.0.1/zimran_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-28 10:09:14.000000 zimran-fastapi-1.0.1/zimran_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-28 10:09:14.000000 zimran-fastapi-1.0.1/zimran_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:09:14.000000 zimran-fastapi-1.0.1/zimran_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 10:09:14.000000 zimran-fastapi-1.0.1/zimran_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:09:14.000000 zimran-fastapi-1.0.1/zimran_fastapi.egg-info/top_level.txt
```

### Comparing `zimran-fastapi-1.0.0/setup.py` & `zimran-fastapi-1.0.1/setup.py`

 * *Files identical despite different names*

