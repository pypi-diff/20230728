# Comparing `tmp/neptune_pytorch-1.0.0.tar.gz` & `tmp/neptune_pytorch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_pytorch-1.0.0.tar", max compression
+gzip compressed data, was "neptune_pytorch-1.0.1.tar", max compression
```

## Comparing `neptune_pytorch-1.0.0.tar` & `neptune_pytorch-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1115 2023-06-28 09:21:18.678046 neptune_pytorch-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-06-28 09:21:18.678046 neptune_pytorch-1.0.0/LICENSE
--rw-r--r--   0        0        0      132 2023-06-28 09:21:18.678046 neptune_pytorch-1.0.0/README.md
--rw-r--r--   0        0        0     2565 2023-06-28 09:21:29.902198 neptune_pytorch-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      724 2023-06-28 09:21:18.678046 neptune_pytorch-1.0.0/src/neptune_pytorch/__init__.py
--rw-r--r--   0        0        0     8984 2023-06-28 09:21:18.678046 neptune_pytorch-1.0.0/src/neptune_pytorch/impl/__init__.py
--rw-r--r--   0        0        0      738 2023-06-28 09:21:18.678046 neptune_pytorch-1.0.0/src/neptune_pytorch/impl/version.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 neptune_pytorch-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1246 2023-07-28 12:09:18.039488 neptune_pytorch-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-07-28 12:09:18.039488 neptune_pytorch-1.0.1/LICENSE
+-rw-r--r--   0        0        0      132 2023-07-28 12:09:18.039488 neptune_pytorch-1.0.1/README.md
+-rw-r--r--   0        0        0     2581 2023-07-28 12:09:33.811617 neptune_pytorch-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      724 2023-07-28 12:09:18.039488 neptune_pytorch-1.0.1/src/neptune_pytorch/__init__.py
+-rw-r--r--   0        0        0     8984 2023-07-28 12:09:18.039488 neptune_pytorch-1.0.1/src/neptune_pytorch/impl/__init__.py
+-rw-r--r--   0        0        0      738 2023-07-28 12:09:18.039488 neptune_pytorch-1.0.1/src/neptune_pytorch/impl/version.py
+-rw-r--r--   0        0        0     2095 1970-01-01 00:00:00.000000 neptune_pytorch-1.0.1/PKG-INFO
```

### Comparing `neptune_pytorch-1.0.0/CHANGELOG.md` & `neptune_pytorch-1.0.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune-pytorch 1.0.1
+
+### Fixes
+- Make `torchviz` optional dependency. (https://github.com/neptune-ai/neptune-pytorch/pull/8)
+
 ## neptune-pytorch 1.0.0
 
 ### Fixes
 - Change where `checkpoints` are logged. Previously they we logged under `base_namespace/model` but now they will be logged under `base_namespace/model/checkpoints` (https://github.com/neptune-ai/neptune-pytorch/pull/5)
 - Add warning if `dot` is not installed instead of hard error. Also, improve clean-up of visualization files (https://github.com/neptune-ai/neptune-pytorch/pull/6)
 ### Features
 - Create `NeptuneLogger` for logging metadata (https://github.com/neptune-ai/neptune-pytorch/pull/1)
```

### Comparing `neptune_pytorch-1.0.0/LICENSE` & `neptune_pytorch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-1.0.0/pyproject.toml` & `neptune_pytorch-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,28 @@
 [tool.poetry.extras]
 dev = [
     "pre-commit",
     "pytest",
     "pytest-cov",
     "pydot",
     "neptune",
+    "torchviz",
 ]
 
 [tool.poetry]
 authors = ["neptune.ai <contact@neptune.ai>"]
 description = "Neptune.ai pytorch integration library"
 repository = "https://github.com/neptune-ai/neptune-pytorch"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/pytorch"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-pytorch"
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_pytorch-1.0.0/src/neptune_pytorch/__init__.py` & `neptune_pytorch-1.0.1/src/neptune_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-1.0.0/src/neptune_pytorch/impl/__init__.py` & `neptune_pytorch-1.0.1/src/neptune_pytorch/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-1.0.0/src/neptune_pytorch/impl/version.py` & `neptune_pytorch-1.0.1/src/neptune_pytorch/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-1.0.0/PKG-INFO` & `neptune_pytorch-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-pytorch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Neptune.ai pytorch integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -31,15 +31,15 @@
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: neptune (>=1.0.0) ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydot ; extra == "dev"
 Requires-Dist: pytest (>=5.0) ; extra == "dev"
 Requires-Dist: pytest-cov (==2.10.1) ; extra == "dev"
 Requires-Dist: torch (>1.8.0)
-Requires-Dist: torchviz
+Requires-Dist: torchviz ; extra == "dev"
 Project-URL: Documentation, https://docs.neptune.ai/integrations-and-supported-tools/model-training/pytorch
 Project-URL: Repository, https://github.com/neptune-ai/neptune-pytorch
 Project-URL: Tracker, https://github.com/neptune-ai/neptune-pytorch/issues
 Description-Content-Type: text/markdown
 
 # Neptune - PyTorch integration
```

