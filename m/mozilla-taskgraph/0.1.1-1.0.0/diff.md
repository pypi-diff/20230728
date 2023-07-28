# Comparing `tmp/mozilla-taskgraph-0.1.1.tar.gz` & `tmp/mozilla-taskgraph-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-0.1.1.tar", last modified: Wed Jun 21 16:25:39 2023, max compression
+gzip compressed data, was "dist/mozilla-taskgraph-1.0.0.tar", last modified: Fri Jul 28 15:22:16 2023, max compression
```

## Comparing `mozilla-taskgraph-0.1.1.tar` & `mozilla-taskgraph-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-04-05 14:08:49.000000 mozilla-taskgraph-0.1.1/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      659 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1061 2023-06-21 15:31:38.000000 mozilla-taskgraph-0.1.1/README.md
--rw-r--r--   0 ahal      (1000) ahal      (1000)      531 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.1/pyproject.toml
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1186 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.1/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.104461 mozilla-taskgraph-0.1.1/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-06-21 16:24:47.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:24:47.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:24:47.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1993 2023-06-20 19:46:53.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      659 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)      490 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       29 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       18 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      126 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.1/test/test_version.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-04-05 14:08:49.000000 mozilla-taskgraph-1.0.0/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      731 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1061 2023-07-17 15:06:27.000000 mozilla-taskgraph-1.0.0/README.md
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      531 2023-07-17 15:06:27.000000 mozilla-taskgraph-1.0.0/pyproject.toml
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1133 2023-07-27 20:32:05.000000 mozilla-taskgraph-1.0.0/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      629 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      315 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/config.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-07-17 15:06:27.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-07-17 15:06:27.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1993 2023-06-20 19:46:53.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1448 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      402 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/worker_types.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      731 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      724 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       27 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       18 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-28 15:22:16.000000 mozilla-taskgraph-1.0.0/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1186 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/test/test_register.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      347 2023-07-28 15:16:05.000000 mozilla-taskgraph-1.0.0/test/test_worker_types.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mozilla-taskgraph-0.1.1/LICENSE` & `mozilla-taskgraph-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.1/PKG-INFO` & `mozilla-taskgraph-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: mozilla-taskgraph
-Version: 0.1.1
+Version: 1.0.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
+Author: UNKNOWN
+Author-email: UNKNOWN
+License: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-License-File: LICENSE
```

### Comparing `mozilla-taskgraph-0.1.1/README.md` & `mozilla-taskgraph-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.1/pyproject.toml` & `mozilla-taskgraph-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.1/setup.py` & `mozilla-taskgraph-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import os
 from distutils.util import convert_path
 
 from setuptools import find_packages, setup
 
 project_dir = os.path.abspath(os.path.dirname(__file__))
 
-namespace = {}
-version_file = convert_path("src/mozilla_taskgraph/__init__.py")
+version_file = convert_path("version.txt")
 with open(version_file) as fh:
-    exec(fh.read(), namespace)
+    version = fh.read().strip()
 
 with open(os.path.join(project_dir, "requirements/base.in")) as fp:
     requirements = fp.read().splitlines()
 
 setup(
     name="mozilla-taskgraph",
-    version=namespace["__version__"],
+    version=version,
     description="Mozilla-specific transforms and utilities for Taskgraph",
     url="https://github.com/mozilla-releng/mozilla-taskgraph",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=requirements,
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py` & `mozilla-taskgraph-1.0.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-1.0.0/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: mozilla-taskgraph
-Version: 0.1.1
+Version: 1.0.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
+Author: UNKNOWN
+Author-email: UNKNOWN
+License: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-License-File: LICENSE
```

