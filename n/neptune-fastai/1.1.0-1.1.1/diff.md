# Comparing `tmp/neptune_fastai-1.1.0.tar.gz` & `tmp/neptune_fastai-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_fastai-1.1.0.tar", max compression
+gzip compressed data, was "neptune_fastai-1.1.1.tar", max compression
```

## Comparing `neptune_fastai-1.1.0.tar` & `neptune_fastai-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2120 2023-03-16 12:35:44.072020 neptune_fastai-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-03-16 12:35:44.072020 neptune_fastai-1.1.0/LICENSE
--rw-r--r--   0        0        0     2387 2023-03-16 12:35:44.072020 neptune_fastai-1.1.0/README.md
--rw-r--r--   0        0        0     2619 2023-03-16 12:35:57.749529 neptune_fastai-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      777 2023-03-16 12:35:44.072020 neptune_fastai-1.1.0/src/neptune_fastai/__init__.py
--rw-r--r--   0        0        0    12896 2023-03-16 12:35:44.076021 neptune_fastai-1.1.0/src/neptune_fastai/impl/__init__.py
--rw-r--r--   0        0        0      735 2023-03-16 12:35:44.076021 neptune_fastai-1.1.0/src/neptune_fastai/impl/version.py
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 neptune_fastai-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2261 2023-07-28 06:56:24.753722 neptune_fastai-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-07-28 06:56:24.753722 neptune_fastai-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2460 2023-07-28 06:56:24.753722 neptune_fastai-1.1.1/README.md
+-rw-r--r--   0        0        0     2619 2023-07-28 06:56:36.750016 neptune_fastai-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      777 2023-07-28 06:56:24.753722 neptune_fastai-1.1.1/src/neptune_fastai/__init__.py
+-rw-r--r--   0        0        0    13344 2023-07-28 06:56:24.753722 neptune_fastai-1.1.1/src/neptune_fastai/impl/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-28 06:56:24.753722 neptune_fastai-1.1.1/src/neptune_fastai/impl/version.py
+-rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 neptune_fastai-1.1.1/PKG-INFO
```

### Comparing `neptune_fastai-1.1.0/CHANGELOG.md` & `neptune_fastai-1.1.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune-fastai 1.1.1
+
+### Fixes
+- Don't error if `optim.__name__` is not present. (https://github.com/neptune-ai/neptune-fastai/pull/54)
+
 ## neptune-fastai 1.1.0
 
 ### Changes
 - Updated integration for compatibility with `neptune 1.X`
 - Removed `neptune` and `neptune-client` from base requirements - installation is checked at runtime
 - Functions outside the callback accept `Handler` as well
```

### Comparing `neptune_fastai-1.1.0/LICENSE` & `neptune_fastai-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_fastai-1.1.0/README.md` & `neptune_fastai-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 *Example dashboard with train-valid metrics and selected parameters*
 
 
 ## Resources
 
 * [Documentation](https://docs.neptune.ai/integrations/fastai)
 * [Code example on GitHub](https://github.com/neptune-ai/examples/tree/main/integrations-and-supported-tools/fastai/scripts)
-* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/fastai-integration/e/FAS-61/dashboard/fastai-dashboard-1f456716-f509-4432-b8b3-a7f5242703b6)
+* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/fastai-integration/runs/details?viewId=standard-view&detailsTab=dashboard&dashboardId=fastai-dashboard-1f456716-f509-4432-b8b3-a7f5242703b6&shortId=FAS-1895&type=run)
 * [Run example in Google Colab](https://colab.research.google.com/github/neptune-ai/examples/blob/main/integrations-and-supported-tools/fastai/notebooks/Neptune_fastai.ipynb)
 
 ## Example
 
 On the command line:
 
 ```
-pip install neptune[fastai]
+pip install neptune-fastai
 ```
 
 In Python:
 
 ```python
 import neptune
```

### Comparing `neptune_fastai-1.1.0/pyproject.toml` & `neptune_fastai-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 repository = "https://github.com/neptune-ai/neptune-fastai"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/fastai"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-fastai"
 readme = "README.md"
-version = "1.1.0"
+version = "1.1.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_fastai-1.1.0/src/neptune_fastai/__init__.py` & `neptune_fastai-1.1.1/src/neptune_fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_fastai-1.1.0/src/neptune_fastai/impl/__init__.py` & `neptune_fastai-1.1.1/src/neptune_fastai/impl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,25 @@
 
     @property
     def _batch_size(self) -> int:
         return self.dls.bs
 
     @property
     def _optimizer_name(self) -> Optional[str]:
-        return self.opt_func.__name__
+        NA = "N/A"
+        optim_name = getattr(self.opt_func, "__name__", NA)
+        if optim_name == NA:
+            warning_msg = (
+                "NeptuneCallback: Couldn't retrieve the optimizer name, "
+                "so it will be logged as 'N/A'. You can set the optimizer "
+                "name by assigning it to the __name__ attribute. "
+                "Eg. >>> optimizer.__name__ = 'NAME'"
+            )
+            warnings.warn(warning_msg)
+        return optim_name
 
     @property
     def _device(self) -> str:
         return default_device() or getattr(self.dls, "device", default_device())
 
     @property
     def _vocab(self) -> List[str]:
```

### Comparing `neptune_fastai-1.1.0/src/neptune_fastai/impl/version.py` & `neptune_fastai-1.1.1/src/neptune_fastai/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_fastai-1.1.0/PKG-INFO` & `neptune_fastai-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-fastai
-Version: 1.1.0
+Version: 1.1.1
 Summary: Neptune.ai fast.ai integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -64,23 +64,23 @@
 *Example dashboard with train-valid metrics and selected parameters*
 
 
 ## Resources
 
 * [Documentation](https://docs.neptune.ai/integrations/fastai)
 * [Code example on GitHub](https://github.com/neptune-ai/examples/tree/main/integrations-and-supported-tools/fastai/scripts)
-* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/fastai-integration/e/FAS-61/dashboard/fastai-dashboard-1f456716-f509-4432-b8b3-a7f5242703b6)
+* [Example dashboard in the Neptune app](https://app.neptune.ai/o/common/org/fastai-integration/runs/details?viewId=standard-view&detailsTab=dashboard&dashboardId=fastai-dashboard-1f456716-f509-4432-b8b3-a7f5242703b6&shortId=FAS-1895&type=run)
 * [Run example in Google Colab](https://colab.research.google.com/github/neptune-ai/examples/blob/main/integrations-and-supported-tools/fastai/notebooks/Neptune_fastai.ipynb)
 
 ## Example
 
 On the command line:
 
 ```
-pip install neptune[fastai]
+pip install neptune-fastai
 ```
 
 In Python:
 
 ```python
 import neptune
```

