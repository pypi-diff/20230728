# Comparing `tmp/thetis-0.1.1.tar.gz` & `tmp/thetis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetis-0.1.1.tar", last modified: Fri Jul 28 09:25:31 2023, max compression
+gzip compressed data, was "thetis-0.1.2.tar", last modified: Fri Jul 28 12:15:32 2023, max compression
```

## Comparing `thetis-0.1.1.tar` & `thetis-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 09:25:31.963148 thetis-0.1.1/
--rw-rw-r--   0 thetis    (1002) thetis    (1002)     5105 2023-07-28 09:25:20.000000 thetis-0.1.1/LICENSE.md
--rw-r--r--   0 thetis    (1002) thetis    (1002)    14145 2023-07-28 09:25:31.963148 thetis-0.1.1/PKG-INFO
--rw-rw-r--   0 thetis    (1002) thetis    (1002)    13337 2023-07-28 09:25:20.000000 thetis-0.1.1/README.md
-drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 09:25:31.963148 thetis-0.1.1/docs/
-drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 09:25:31.963148 thetis-0.1.1/docs/source/
--rw-rw-r--   0 thetis    (1002) thetis    (1002)     1875 2023-07-28 09:25:20.000000 thetis-0.1.1/docs/source/conf.py
--rw-rw-r--   0 thetis    (1002) thetis    (1002)     1640 2023-07-28 09:25:20.000000 thetis-0.1.1/pyproject.toml
--rw-rw-r--   0 thetis    (1002) thetis    (1002)       17 2023-07-28 09:25:20.000000 thetis-0.1.1/requirements.txt
--rw-r--r--   0 thetis    (1002) thetis    (1002)       38 2023-07-28 09:25:31.963148 thetis-0.1.1/setup.cfg
--rw-rw-r--   0 thetis    (1002) thetis    (1002)      409 2023-07-28 09:25:20.000000 thetis-0.1.1/setup.py
-drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 09:25:31.963148 thetis-0.1.1/thetis/
--rw-rw-r--   0 thetis    (1002) thetis    (1002)      694 2023-07-28 09:25:20.000000 thetis-0.1.1/thetis/__init__.py
--rw-rw-r--   0 thetis    (1002) thetis    (1002)    16839 2023-07-28 09:25:20.000000 thetis-0.1.1/thetis/mlflow.py
--rw-rw-r--   0 thetis    (1002) thetis    (1002)     9335 2023-07-28 09:25:20.000000 thetis-0.1.1/thetis/service.py
-drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 09:25:31.963148 thetis-0.1.1/thetis.egg-info/
--rw-r--r--   0 thetis    (1002) thetis    (1002)    14145 2023-07-28 09:25:31.000000 thetis-0.1.1/thetis.egg-info/PKG-INFO
--rw-r--r--   0 thetis    (1002) thetis    (1002)      284 2023-07-28 09:25:31.000000 thetis-0.1.1/thetis.egg-info/SOURCES.txt
--rw-r--r--   0 thetis    (1002) thetis    (1002)        1 2023-07-28 09:25:31.000000 thetis-0.1.1/thetis.egg-info/dependency_links.txt
--rw-r--r--   0 thetis    (1002) thetis    (1002)       18 2023-07-28 09:25:31.000000 thetis-0.1.1/thetis.egg-info/requires.txt
--rw-r--r--   0 thetis    (1002) thetis    (1002)       17 2023-07-28 09:25:31.000000 thetis-0.1.1/thetis.egg-info/top_level.txt
+drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 12:15:32.730863 thetis-0.1.2/
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)     5105 2023-07-28 12:15:21.000000 thetis-0.1.2/LICENSE.md
+-rw-r--r--   0 thetis    (1002) thetis    (1002)    14154 2023-07-28 12:15:32.730863 thetis-0.1.2/PKG-INFO
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)    13346 2023-07-28 12:15:21.000000 thetis-0.1.2/README.md
+drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 12:15:32.726863 thetis-0.1.2/docs/
+drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 12:15:32.726863 thetis-0.1.2/docs/source/
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)     1875 2023-07-28 12:15:21.000000 thetis-0.1.2/docs/source/conf.py
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)     1640 2023-07-28 12:15:21.000000 thetis-0.1.2/pyproject.toml
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)       17 2023-07-28 12:15:21.000000 thetis-0.1.2/requirements.txt
+-rw-r--r--   0 thetis    (1002) thetis    (1002)       38 2023-07-28 12:15:32.730863 thetis-0.1.2/setup.cfg
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)      409 2023-07-28 12:15:21.000000 thetis-0.1.2/setup.py
+drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 12:15:32.726863 thetis-0.1.2/thetis/
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)      694 2023-07-28 12:15:21.000000 thetis-0.1.2/thetis/__init__.py
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)    16839 2023-07-28 12:15:21.000000 thetis-0.1.2/thetis/mlflow.py
+-rw-rw-r--   0 thetis    (1002) thetis    (1002)     9335 2023-07-28 12:15:21.000000 thetis-0.1.2/thetis/service.py
+drwxr-xr-x   0 thetis    (1002) thetis    (1002)        0 2023-07-28 12:15:32.730863 thetis-0.1.2/thetis.egg-info/
+-rw-r--r--   0 thetis    (1002) thetis    (1002)    14154 2023-07-28 12:15:32.000000 thetis-0.1.2/thetis.egg-info/PKG-INFO
+-rw-r--r--   0 thetis    (1002) thetis    (1002)      284 2023-07-28 12:15:32.000000 thetis-0.1.2/thetis.egg-info/SOURCES.txt
+-rw-r--r--   0 thetis    (1002) thetis    (1002)        1 2023-07-28 12:15:32.000000 thetis-0.1.2/thetis.egg-info/dependency_links.txt
+-rw-r--r--   0 thetis    (1002) thetis    (1002)       18 2023-07-28 12:15:32.000000 thetis-0.1.2/thetis.egg-info/requires.txt
+-rw-r--r--   0 thetis    (1002) thetis    (1002)       17 2023-07-28 12:15:32.000000 thetis-0.1.2/thetis.egg-info/top_level.txt
```

### Comparing `thetis-0.1.1/LICENSE.md` & `thetis-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `thetis-0.1.1/PKG-INFO` & `thetis-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Service to examine data processing pipelines (e.g., machine learning or deep learning pipelines) for uncertainty consistency (calibration), fairness, and other safety-relevant aspects.
 Author: e:fs TechHub GmbH
 Author-email: fabian.kueppers@efs-techhub.com
 Maintainer: e:fs TechHub GmbH
 Maintainer-email: fabian.kueppers@efs-techhub.com
 License: Proprietary
 Project-URL: Homepage, https://efs-techhub.com/efs-portfolio/loesungen/thetis
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-![Thetis Logo](https://github.com/EFS-OpenSource/Thetis/blob/main/docs/source/_static/thetis-logo.png)
+![Thetis Logo](https://github.com/EFS-OpenSource/Thetis/blob/main/docs/source/_static/thetis-logo.png?raw=true)
 
 --------------------------------------------------------------------------------
 
 _Even if your AI is as strong as Achilles, Thetis will certainly know about its weaknesses._
 
 Thetis is a service to examine safety-relevant aspects of AI algorithms (e.g., machine learning or deep learning models)
 for uncertainty consistency (calibration), fairness, data quality, and robustness.
```

### Comparing `thetis-0.1.1/README.md` & `thetis-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Thetis Logo](https://github.com/EFS-OpenSource/Thetis/blob/main/docs/source/_static/thetis-logo.png)
+![Thetis Logo](https://github.com/EFS-OpenSource/Thetis/blob/main/docs/source/_static/thetis-logo.png?raw=true)
 
 --------------------------------------------------------------------------------
 
 _Even if your AI is as strong as Achilles, Thetis will certainly know about its weaknesses._
 
 Thetis is a service to examine safety-relevant aspects of AI algorithms (e.g., machine learning or deep learning models)
 for uncertainty consistency (calibration), fairness, data quality, and robustness.
```

### Comparing `thetis-0.1.1/docs/source/conf.py` & `thetis-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `thetis-0.1.1/pyproject.toml` & `thetis-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thetis-0.1.1/thetis/__init__.py` & `thetis-0.1.2/thetis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 """
 
 from .service import thetis
 from .mlflow import thetis_mlflow
 
 name = "thetis"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `thetis-0.1.1/thetis/mlflow.py` & `thetis-0.1.2/thetis/mlflow.py`

 * *Files identical despite different names*

### Comparing `thetis-0.1.1/thetis/service.py` & `thetis-0.1.2/thetis/service.py`

 * *Files identical despite different names*

### Comparing `thetis-0.1.1/thetis.egg-info/PKG-INFO` & `thetis-0.1.2/thetis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Service to examine data processing pipelines (e.g., machine learning or deep learning pipelines) for uncertainty consistency (calibration), fairness, and other safety-relevant aspects.
 Author: e:fs TechHub GmbH
 Author-email: fabian.kueppers@efs-techhub.com
 Maintainer: e:fs TechHub GmbH
 Maintainer-email: fabian.kueppers@efs-techhub.com
 License: Proprietary
 Project-URL: Homepage, https://efs-techhub.com/efs-portfolio/loesungen/thetis
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-![Thetis Logo](https://github.com/EFS-OpenSource/Thetis/blob/main/docs/source/_static/thetis-logo.png)
+![Thetis Logo](https://github.com/EFS-OpenSource/Thetis/blob/main/docs/source/_static/thetis-logo.png?raw=true)
 
 --------------------------------------------------------------------------------
 
 _Even if your AI is as strong as Achilles, Thetis will certainly know about its weaknesses._
 
 Thetis is a service to examine safety-relevant aspects of AI algorithms (e.g., machine learning or deep learning models)
 for uncertainty consistency (calibration), fairness, data quality, and robustness.
```

