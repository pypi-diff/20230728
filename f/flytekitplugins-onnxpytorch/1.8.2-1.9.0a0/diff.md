# Comparing `tmp/flytekitplugins-onnxpytorch-1.8.2.tar.gz` & `tmp/flytekitplugins-onnxpytorch-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxpytorch-1.8.2.tar", last modified: Fri Jul 28 00:24:49 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxpytorch-1.9.0a0.tar", last modified: Thu Jul 20 18:58:23 2023, max compression
```

## Comparing `flytekitplugins-onnxpytorch-1.8.2.tar` & `flytekitplugins-onnxpytorch-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:49.660007 flytekitplugins-onnxpytorch-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-28 00:24:49.660007 flytekitplugins-onnxpytorch-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 00:24:26.000000 flytekitplugins-onnxpytorch-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:49.660007 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:49.660007 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins/onnxpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 00:24:26.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins/onnxpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-28 00:24:26.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins/onnxpytorch/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:24:49.660007 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-28 00:24:49.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 00:24:49.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:24:49.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 00:24:49.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 00:24:49.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 00:24:49.000000 flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:24:49.660007 flytekitplugins-onnxpytorch-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-28 00:24:41.000000 flytekitplugins-onnxpytorch-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 18:57:54.000000 flytekitplugins-onnxpytorch-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.056715 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-20 18:57:54.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-20 18:57:54.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-20 18:58:12.000000 flytekitplugins-onnxpytorch-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-onnxpytorch-1.8.2/PKG-INFO` & `flytekitplugins-onnxpytorch-1.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.8.2
+Version: 1.9.0a0
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.8.2/flytekitplugins/onnxpytorch/schema.py` & `flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-onnxpytorch-1.8.2/flytekitplugins_onnxpytorch.egg-info/PKG-INFO` & `flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.8.2
+Version: 1.9.0a0
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.8.2/setup.py` & `flytekitplugins-onnxpytorch-1.9.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "torch>=1.11.0"]
 
-__version__ = "1.8.2"
+__version__ = "1.9.0a0"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX PyTorch Plugin for Flytekit",
```

