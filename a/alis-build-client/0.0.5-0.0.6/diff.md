# Comparing `tmp/alis_build_client-0.0.5.tar.gz` & `tmp/alis_build_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alis_build_client-0.0.5.tar", max compression
+gzip compressed data, was "alis_build_client-0.0.6.tar", max compression
```

## Comparing `alis_build_client-0.0.5.tar` & `alis_build_client-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      174 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/README.md
--rw-r--r--   0        0        0       75 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/alis/build/client/__init__.py
--rw-r--r--   0        0        0     2893 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/alis/build/client/grpc.py
--rw-r--r--   0        0        0      809 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 alis_build_client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      174 2023-07-28 12:44:09.907896 alis_build_client-0.0.6/README.md
+-rw-r--r--   0        0        0       75 2023-07-28 12:44:09.907896 alis_build_client-0.0.6/alis/build/client/__init__.py
+-rw-r--r--   0        0        0     2893 2023-07-28 12:44:09.907896 alis_build_client-0.0.6/alis/build/client/grpc.py
+-rw-r--r--   0        0        0      809 2023-07-28 12:44:09.907896 alis_build_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 alis_build_client-0.0.6/PKG-INFO
```

### Comparing `alis_build_client-0.0.5/alis/build/client/grpc.py` & `alis_build_client-0.0.6/alis/build/client/grpc.py`

 * *Files identical despite different names*

### Comparing `alis_build_client-0.0.5/PKG-INFO` & `alis_build_client-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: alis-build-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: A grpc client package for python applications.
-Home-page: https://github.com/yourusername/grpc_client
+Home-page: https://pypi.org/project/alis-build-client/
 License: MIT
 Author: Thomas Scholtz
 Author-email: tom.scholtz@alisx.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

