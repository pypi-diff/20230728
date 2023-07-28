# Comparing `tmp/localstack-extension-hello-world-0.1.0.tar.gz` & `tmp/localstack-extension-hello-world-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-extension-hello-world-0.1.0.tar", last modified: Fri Jul 28 13:39:27 2023, max compression
+gzip compressed data, was "localstack-extension-hello-world-0.1.0.dev1.tar", last modified: Fri Jul 28 13:34:50 2023, max compression
```

## Comparing `localstack-extension-hello-world-0.1.0.tar` & `localstack-extension-hello-world-0.1.0.dev1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 13:39:27.393909 localstack-extension-hello-world-0.1.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      640 2023-07-28 13:39:27.393909 localstack-extension-hello-world-0.1.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      335 2023-07-28 13:38:40.000000 localstack-extension-hello-world-0.1.0/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 13:39:27.389909 localstack-extension-hello-world-0.1.0/helloworld/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       20 2023-02-17 21:15:09.000000 localstack-extension-hello-world-0.1.0/helloworld/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      288 2023-07-28 13:38:40.000000 localstack-extension-hello-world-0.1.0/helloworld/extension.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 13:39:27.393909 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      640 2023-07-28 13:39:27.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      483 2023-07-28 13:39:27.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 13:39:27.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       79 2023-07-28 13:39:27.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 13:39:21.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       16 2023-07-28 13:39:27.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       11 2023-07-28 13:39:27.000000 localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      424 2023-07-28 13:38:40.000000 localstack-extension-hello-world-0.1.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2023-07-28 13:39:27.393909 localstack-extension-hello-world-0.1.0/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)       60 2023-02-17 21:15:09.000000 localstack-extension-hello-world-0.1.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 13:34:50.207124 localstack-extension-hello-world-0.1.0.dev1/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      645 2023-07-28 13:34:50.207124 localstack-extension-hello-world-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      335 2023-07-28 13:33:53.000000 localstack-extension-hello-world-0.1.0.dev1/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 13:34:50.203124 localstack-extension-hello-world-0.1.0.dev1/helloworld/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       20 2023-02-17 21:15:09.000000 localstack-extension-hello-world-0.1.0.dev1/helloworld/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      288 2023-07-28 13:30:46.000000 localstack-extension-hello-world-0.1.0.dev1/helloworld/extension.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 13:34:50.203124 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      645 2023-07-28 13:34:50.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      483 2023-07-28 13:34:50.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 13:34:50.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       79 2023-07-28 13:34:50.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 13:34:45.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       16 2023-07-28 13:34:50.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       11 2023-07-28 13:34:50.000000 localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      424 2023-07-28 13:28:50.000000 localstack-extension-hello-world-0.1.0.dev1/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      670 2023-07-28 13:34:50.207124 localstack-extension-hello-world-0.1.0.dev1/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       60 2023-02-17 21:15:09.000000 localstack-extension-hello-world-0.1.0.dev1/setup.py
```

### Comparing `localstack-extension-hello-world-0.1.0/PKG-INFO` & `localstack-extension-hello-world-0.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-extension-hello-world
-Version: 0.1.0
+Version: 0.1.0.dev1
 Summary: LocalStack Extension: Hello World
 Home-page: https://github.com/localstack/localstack-extensions/tree/main/hello-world
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 Description-Content-Type: text/markdown
 
 Hello World LocalStack extension
```

### Comparing `localstack-extension-hello-world-0.1.0/localstack_extension_hello_world.egg-info/PKG-INFO` & `localstack-extension-hello-world-0.1.0.dev1/localstack_extension_hello_world.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-extension-hello-world
-Version: 0.1.0
+Version: 0.1.0.dev1
 Summary: LocalStack Extension: Hello World
 Home-page: https://github.com/localstack/localstack-extensions/tree/main/hello-world
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 Description-Content-Type: text/markdown
 
 Hello World LocalStack extension
```

### Comparing `localstack-extension-hello-world-0.1.0/setup.cfg` & `localstack-extension-hello-world-0.1.0.dev1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-extension-hello-world
-version = 0.1.0
+version = 0.1.0.dev1
 summary = LocalStack Extension: Hello World
 description = A hello world example extension for Localstack, showing how extensions should be organized
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/localstack/localstack-extensions/tree/main/hello-world
 author = Thomas Rausch
 author_email = thomas@localstack.cloud
```

