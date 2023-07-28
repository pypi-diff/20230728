# Comparing `tmp/vdk-lineage-model-0.0.824443273.tar.gz` & `tmp/vdk-lineage-model-0.0.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-lineage-model-0.0.824443273.tar", last modified: Fri Mar 31 14:25:31 2023, max compression
+gzip compressed data, was "vdk-lineage-model-0.0.948436673.tar", last modified: Fri Jul 28 09:42:41 2023, max compression
```

## Comparing `vdk-lineage-model-0.0.824443273.tar` & `vdk-lineage-model-0.0.948436673.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/
--rw-r--r--   0 root         (0) root         (0)     1192 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-03-31 14:25:20.000000 vdk-lineage-model-0.0.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-03-31 14:25:23.000000 vdk-lineage-model-0.0.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/logger/
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-03-31 14:25:20.000000 vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/logger/lineage_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/sql/
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-03-31 14:25:20.000000 vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/sql/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/src/vdk_lineage_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1192 2023-03-31 14:25:31.000000 vdk-lineage-model-0.0.824443273/src/vdk_lineage_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      312 2023-03-31 14:25:31.000000 vdk-lineage-model-0.0.824443273/src/vdk_lineage_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:31.000000 vdk-lineage-model-0.0.824443273/src/vdk_lineage_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:31.000000 vdk-lineage-model-0.0.824443273/src/vdk_lineage_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:31.430324 vdk-lineage-model-0.0.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-03-31 14:25:20.000000 vdk-lineage-model-0.0.824443273/tests/test_sql_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.504079 vdk-lineage-model-0.0.948436673/
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-07-28 09:42:41.504079 vdk-lineage-model-0.0.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-28 09:42:20.000000 vdk-lineage-model-0.0.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:41.504079 vdk-lineage-model-0.0.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-07-28 09:42:29.000000 vdk-lineage-model-0.0.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/logger/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-07-28 09:42:20.000000 vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/logger/lineage_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/sql/
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-07-28 09:42:20.000000 vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/sql/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/src/vdk_lineage_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-07-28 09:42:41.000000 vdk-lineage-model-0.0.948436673/src/vdk_lineage_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-28 09:42:41.000000 vdk-lineage-model-0.0.948436673/src/vdk_lineage_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:41.000000 vdk-lineage-model-0.0.948436673/src/vdk_lineage_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:41.000000 vdk-lineage-model-0.0.948436673/src/vdk_lineage_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.500079 vdk-lineage-model-0.0.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-28 09:42:20.000000 vdk-lineage-model-0.0.948436673/tests/test_sql_model.py
```

### Comparing `vdk-lineage-model-0.0.824443273/PKG-INFO` & `vdk-lineage-model-0.0.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-lineage-model
-Version: 0.0.824443273
+Version: 0.0.948436673
 Summary: VDK Lineage Model plugin defines common lineage model and classes used for managing lineageinformation in other VDK plugins.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-lineage-model-0.0.824443273/README.md` & `vdk-lineage-model-0.0.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-lineage-model-0.0.824443273/setup.py` & `vdk-lineage-model-0.0.948436673/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.0.824443273"
+__version__ = "0.0.948436673"
 
 setuptools.setup(
     name="vdk-lineage-model",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="VDK Lineage Model plugin defines common lineage model and classes used for managing lineage"
     "information in other VDK plugins.",
```

### Comparing `vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/logger/lineage_logger.py` & `vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/logger/lineage_logger.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-model-0.0.824443273/src/vdk/api/lineage/model/sql/model.py` & `vdk-lineage-model-0.0.948436673/src/vdk/api/lineage/model/sql/model.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-model-0.0.824443273/src/vdk_lineage_model.egg-info/PKG-INFO` & `vdk-lineage-model-0.0.948436673/src/vdk_lineage_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-lineage-model
-Version: 0.0.824443273
+Version: 0.0.948436673
 Summary: VDK Lineage Model plugin defines common lineage model and classes used for managing lineageinformation in other VDK plugins.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

