# Comparing `tmp/flytekitplugins-pandera-1.8.2.tar.gz` & `tmp/flytekitplugins-pandera-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pandera-1.8.2.tar", last modified: Fri Jul 28 00:24:50 2023, max compression
+gzip compressed data, was "flytekitplugins-pandera-1.9.0a0.tar", last modified: Thu Jul 20 18:58:24 2023, max compression
```

## Comparing `flytekitplugins-pandera-1.8.2.tar` & `flytekitplugins-pandera-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:50.416024 flytekitplugins-pandera-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 00:24:50.416024 flytekitplugins-pandera-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 00:24:26.000000 flytekitplugins-pandera-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:50.416024 flytekitplugins-pandera-1.8.2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:50.416024 flytekitplugins-pandera-1.8.2/flytekitplugins/pandera/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 00:24:26.000000 flytekitplugins-pandera-1.8.2/flytekitplugins/pandera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-28 00:24:26.000000 flytekitplugins-pandera-1.8.2/flytekitplugins/pandera/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:50.416024 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 00:24:50.000000 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 00:24:50.000000 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:24:50.000000 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 00:24:50.000000 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 00:24:50.000000 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 00:24:50.000000 flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:24:50.416024 flytekitplugins-pandera-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 00:24:41.000000 flytekitplugins-pandera-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.008724 flytekitplugins-pandera-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-20 18:58:24.008724 flytekitplugins-pandera-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-20 18:57:54.000000 flytekitplugins-pandera-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.008724 flytekitplugins-pandera-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.008724 flytekitplugins-pandera-1.9.0a0/flytekitplugins/pandera/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-20 18:57:54.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins/pandera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-20 18:57:54.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins/pandera/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.008724 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-20 18:58:23.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 18:58:23.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:23.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 18:58:23.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:24.008724 flytekitplugins-pandera-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 18:58:12.000000 flytekitplugins-pandera-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-pandera-1.8.2/PKG-INFO` & `flytekitplugins-pandera-1.9.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.8.2
+Version: 1.9.0a0
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.8.2/README.md` & `flytekitplugins-pandera-1.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.8.2/flytekitplugins/pandera/schema.py` & `flytekitplugins-pandera-1.9.0a0/flytekitplugins/pandera/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.8.2/flytekitplugins_pandera.egg-info/PKG-INFO` & `flytekitplugins-pandera-1.9.0a0/flytekitplugins_pandera.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.8.2
+Version: 1.9.0a0
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.8.2/setup.py` & `flytekitplugins-pandera-1.9.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "pandera"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pandera>=0.7.1"]
 
-__version__ = "1.8.2"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Pandera plugin for flytekit",
```

