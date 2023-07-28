# Comparing `tmp/deepsensor-0.1.5.tar.gz` & `tmp/deepsensor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.1.5.tar", last modified: Mon Jul 17 17:08:16 2023, max compression
+gzip compressed data, was "deepsensor-0.1.6.tar", last modified: Fri Jul 28 21:05:21 2023, max compression
```

## Comparing `deepsensor-0.1.5.tar` & `deepsensor-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 17:08:16.088207 deepsensor-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-17 17:08:02.000000 deepsensor-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/active_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/active_learning/acquisition_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19422 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/active_learning/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27308 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/convnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/nps.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/train/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 17:08:02.000000 deepsensor-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-17 17:08:16.088207 deepsensor-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 17:08:02.000000 deepsensor-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_active_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.427621 deepsensor-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-28 21:05:21.427621 deepsensor-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-28 21:05:12.000000 deepsensor-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/active_learning/acquisition_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/active_learning/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23532 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/convnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/nps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 21:05:12.000000 deepsensor-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 21:05:21.427621 deepsensor-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 21:05:12.000000 deepsensor-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/utils.py
```

### Comparing `deepsensor-0.1.5/PKG-INFO` & `deepsensor-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: deepsensor
-Version: 0.1.5
-Summary: A Python package for modelling xarray and pandas data with neural processes.
-Home-page: https://github.com/tom-andersson/deepsensor
-Author: Tom R. Andersson
-Author-email: tomand@bas.ac.uk
-License: MIT
-Platform: unix
-Platform: linux
-Platform: osx
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-
 [//]: # (![]&#40;figs/DeepSensorLogo.png&#41;)
 <ul style="text-align: center;">
 <img src="figs/DeepSensorLogo.png" width="700"/>
 </ul>
 
 <ul style="margin-top:0px;">
 
@@ -26,18 +11,22 @@
 
 -----------
 
 [![release](https://img.shields.io/badge/release-v0.1.5-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/tom-andersson/deepsensor/blob/main/LICENSE)
 
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
+For demonstrators, use cases, and videos showcasing the functionality of DeepSensor, check out the
+[DeepSensor Gallery](https://github.com/tom-andersson/deepsensor_gallery)!
+
 Why neural processes?
 -----------
 NPs are a highly flexible class of probabilistic models that can:
 - ingest multiple context sets (i.e. data streams) containing gridded or pointwise observations
 - handle multiple gridded resolutions
 - predict at arbitrary target locations
 - quantify prediction uncertainty
@@ -147,15 +136,15 @@
            40.0 250.0  277.947373
 2014-12-02 50.0 280.0   261.08943
            40.0 250.0  278.219599
 2014-12-03 50.0 280.0  257.128185
            40.0 250.0  278.444229
 ```
 
-This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/quickstart_example.ipynb) with added visualisations.
+This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor_demos/blob/main/demonstrators/quickstart.ipynb) with added visualisations.
 
 Extending DeepSensor with new models
 ----------
 To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
 and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
 such as `.mean` and `.stddev`.
 ```python
@@ -171,21 +160,9 @@
     def stddev(self, task: Task):
         """Compute stddev at target locations"""
         return 0.1
     
     ...
 ```
 `NewModel` can then be used in the same way as the built-in `ConvNP` model.
-See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/extending_models.ipynb)
+See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor_gallery/blob/main/demonstrators/extending_models.ipynb)
 for more details.
-
-Learn more
-----------
-- Documentation: TODO
-- Issue tracker: https://github.com/tom-andersson/deepsensor/issues
-- Source code: https://github.com/tom-andersson/deepsensor
-
-**Talks**
-- Environmental Sensor Placement with ConvGNPs: https://youtu.be/v0pmqh09u1Y
-
-**Papers**
-- TODO
```

### Comparing `deepsensor-0.1.5/README.md` & `deepsensor-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: deepsensor
+Version: 0.1.6
+Summary: A Python package for modelling xarray and pandas data with neural processes.
+Home-page: https://github.com/tom-andersson/deepsensor
+Author: Tom R. Andersson
+Author-email: tomand@bas.ac.uk
+License: MIT
+Platform: unix
+Platform: linux
+Platform: osx
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+
 [//]: # (![]&#40;figs/DeepSensorLogo.png&#41;)
 <ul style="text-align: center;">
 <img src="figs/DeepSensorLogo.png" width="700"/>
 </ul>
 
 <ul style="margin-top:0px;">
 
@@ -11,18 +26,22 @@
 
 -----------
 
 [![release](https://img.shields.io/badge/release-v0.1.5-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/tom-andersson/deepsensor/blob/main/LICENSE)
 
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
+For demonstrators, use cases, and videos showcasing the functionality of DeepSensor, check out the
+[DeepSensor Gallery](https://github.com/tom-andersson/deepsensor_gallery)!
+
 Why neural processes?
 -----------
 NPs are a highly flexible class of probabilistic models that can:
 - ingest multiple context sets (i.e. data streams) containing gridded or pointwise observations
 - handle multiple gridded resolutions
 - predict at arbitrary target locations
 - quantify prediction uncertainty
@@ -132,15 +151,15 @@
            40.0 250.0  277.947373
 2014-12-02 50.0 280.0   261.08943
            40.0 250.0  278.219599
 2014-12-03 50.0 280.0  257.128185
            40.0 250.0  278.444229
 ```
 
-This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/quickstart_example.ipynb) with added visualisations.
+This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor_demos/blob/main/demonstrators/quickstart.ipynb) with added visualisations.
 
 Extending DeepSensor with new models
 ----------
 To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
 and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
 such as `.mean` and `.stddev`.
 ```python
@@ -156,21 +175,9 @@
     def stddev(self, task: Task):
         """Compute stddev at target locations"""
         return 0.1
     
     ...
 ```
 `NewModel` can then be used in the same way as the built-in `ConvNP` model.
-See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/extending_models.ipynb)
+See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor_gallery/blob/main/demonstrators/extending_models.ipynb)
 for more details.
-
-Learn more
-----------
-- Documentation: TODO
-- Issue tracker: https://github.com/tom-andersson/deepsensor/issues
-- Source code: https://github.com/tom-andersson/deepsensor
-
-**Talks**
-- Environmental Sensor Placement with ConvGNPs: https://youtu.be/v0pmqh09u1Y
-
-**Papers**
-- TODO
```

### Comparing `deepsensor-0.1.5/deepsensor/__init__.py` & `deepsensor-0.1.6/deepsensor/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/active_learning/acquisition_fns.py` & `deepsensor-0.1.6/deepsensor/active_learning/acquisition_fns.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         """
         Args:
             model (ProbabilisticModel):
             context_set_idx (int): Index of context set to add new observations to when computing
                 the acquisition function.
         """
         self.model = model
+        self.min_or_max = -1
 
     def __call__(self, task: Task):
         """
         Args:
             task (Task): Task object containing context and target sets.
 
         Returns:
@@ -53,102 +54,137 @@
         """
         raise NotImplementedError
 
 
 class MeanStddev(AcquisitionFunction):
     """Mean of the marginal variances."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task, target_set_idx=0):
         return np.mean(self.model.stddev(task)[target_set_idx])
 
 
 class MeanVariance(AcquisitionFunction):
     """Mean of the marginal variances."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task, target_set_idx=0):
         return np.mean(self.model.variance(task)[target_set_idx])
 
 
 class pNormStddev(AcquisitionFunction):
     """p-norm of the vector of marginal standard deviations."""
 
     def __init__(self, *args, p=1, **kwargs):
         super().__init__(*args, **kwargs)
         self.p = p
+        self.min_or_max = "min"
 
     def __call__(self, task, target_set_idx=0):
         return np.linalg.norm(
             self.model.stddev(task)[target_set_idx].ravel(), ord=self.p
         )
 
 
 class MeanMarginalEntropy(AcquisitionFunction):
     """Mean of the entropies of the marginal predictive distributions."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task):
         marginal_entropy = self.model.mean_marginal_entropy(task)
         return marginal_entropy
 
 
 class JointEntropy(AcquisitionFunction):
     """Joint entropy of the predictive distribution."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task):
         return self.model.joint_entropy(task)
 
 
 class OracleMAE(AcquisitionFunctionOracle):
     """Oracle mean absolute error."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task):
         pred = self.model.mean(task)
         true = task["Y_t"]
         return np.mean(np.abs(pred - true))
 
 
 class OracleRMSE(AcquisitionFunctionOracle):
     """Oracle root mean squared error."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task):
         pred = self.model.mean(task)
         true = task["Y_t"]
         return np.sqrt(np.mean((pred - true) ** 2))
 
 
 class OracleMarginalNLL(AcquisitionFunctionOracle):
     """Oracle marginal negative log-likelihood."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task):
         pred = self.model.mean(task)
         true = task["Y_t"]
         return -np.mean(norm.logpdf(true, loc=pred, scale=self.model.stddev(task)))
 
 
 class OracleJointNLL(AcquisitionFunctionOracle):
     """Oracle joint negative log-likelihood."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task):
         return -self.model.logpdf(task)
 
 
 class Random(AcquisitionFunctionParallel):
     """Random acquisition function."""
 
     def __init__(self, seed: int = 42):
         self.rng = np.random.default_rng(seed)
+        self.min_or_max = "max"
 
     def __call__(self, task, X_s):
         return self.rng.random(X_s.shape[1])
 
 
 class ContextDist(AcquisitionFunctionParallel):
     """Distance to closest context point."""
 
-    def __init__(self, context_set_idx):
-        self.context_set_idx = context_set_idx
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "max"
 
     def __call__(self, task, X_s):
         X_c = task["X_c"][self.context_set_idx]
 
         if X_c.size == 0:
             # No sensors placed yet, so arbitrarily choose first query point by setting its
             #    acquisition fn to non-zero and all others to zero
@@ -165,14 +201,18 @@
             dist_to_closest_sensor = dists_all.min(axis=1)
         return dist_to_closest_sensor
 
 
 class Stddev(AcquisitionFunctionParallel):
     """Random acquisition function."""
 
+    def __init__(self, model: ProbabilisticModel):
+        super().__init__(model)
+        self.min_or_max = "min"
+
     def __call__(self, task, X_s, target_set_idx=0):
         # Set the target points to the search points
         task = copy.deepcopy(task)
         task["X_t"] = X_s
 
         return self.model.stddev(task)[target_set_idx]
 
@@ -188,14 +228,15 @@
         Args:
             model (ProbabilisticModel):
             context_set_idx (int): Index of context set to add new observations to when computing
                 the acquisition function.
         """
         super().__init__(model)
         self.context_set_idx = context_set_idx
+        self.min_or_max = "max"
 
     def __call__(self, task: Task, X_s: np.ndarray, target_set_idx: int = 0):
         """
         Args:
             task (Task): Task object containing context and target sets.
             X_s (np.ndarray): Search points. Shape (2, N_search).
             target_set_idx (int): Index of target set to compute acquisition function for.
```

### Comparing `deepsensor-0.1.5/deepsensor/active_learning/algorithms.py` & `deepsensor-0.1.6/deepsensor/active_learning/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,22 +106,21 @@
                 print("proposed_infill not on search grid, interpolating.")
             proposed_infill = interp_da1_to_da2(proposed_infill, self.X_s)
         self.query_infill = query_infill
         self.proposed_infill = proposed_infill
 
         # Convert target coords to numpy arrays and assign to tasks
         if isinstance(X_t, (xr.Dataset, xr.DataArray)):
-            if self.X_t_mask is None:
-                # Targets on grid
-                self.X_t_arr = (X_t["x1"].values, X_t["x2"].values)
-            else:
+            # Targets on grid
+            self.X_t_arr = xarray_to_coord_array_normalised(X_t)
+            if self.X_t_mask is not None:
                 # Remove points that lie outside the mask
-                X_t_arr_all = xarray_to_coord_array_normalised(X_t)
-                self.X_t_arr = mask_coord_array_normalised(X_t_arr_all, self.X_t_mask)
+                self.X_t_arr = mask_coord_array_normalised(self.X_t_arr, self.X_t_mask)
         elif isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index)):
+            # Targets off-grid
             self.X_t_arr = X_t.reset_index()[["x1", "x2"]].values.T
         else:
             raise TypeError(f"Unsupported type for X_t: {type(X_t)}")
 
         # Construct search array
         if isinstance(X_s, (xr.Dataset, xr.DataArray)):
             X_s_arr = xarray_to_coord_array_normalised(X_s)
@@ -395,15 +394,14 @@
 
         return best_x_query
 
     def __call__(
         self,
         acquisition_fn: AcquisitionFunction,
         tasks: Union[List[Task], Task],
-        min_or_max: str = "min",
     ) -> Tuple[pd.DataFrame, xr.Dataset]:  # TODO is this correct use of typing?
         """
         Iteratively... docstring TODO
 
         Returns a tensor of proposed new sensor locations (in greedy iteration/priority order)
             and their corresponding list of indexes in the search space.
         """
@@ -411,15 +409,19 @@
             isinstance(acquisition_fn, AcquisitionFunctionOracle)
             and self.task_loader is None
         ):
             raise ValueError(
                 "AcquisitionFunctionOracle requires a task_loader function to be passed to the GreedyOptimal constructor."
             )
 
-        self.min_or_max = min_or_max
+        self.min_or_max = acquisition_fn.min_or_max
+        if self.min_or_max not in ["min", "max"]:
+            raise ValueError(
+                f"min_or_max must be either 'min' or 'max', got {self.min_or_max}."
+            )
 
         if isinstance(tasks, Task):
             tasks = [tasks]
 
         # Make deepcopys so that original tasks are not modified
         tasks = copy.deepcopy(tasks)
```

### Comparing `deepsensor-0.1.5/deepsensor/data/loader.py` & `deepsensor-0.1.6/deepsensor/data/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from deepsensor.data.task import Task
+from deepsensor.data.task import Task, flatten_X
 
 import numpy as np
 import xarray as xr
 import pandas as pd
 
 from typing import List, Tuple, Union
 
@@ -20,80 +20,98 @@
         ],
         target: Union[
             xr.DataArray,
             xr.Dataset,
             pd.DataFrame,
             List[Union[xr.DataArray, xr.Dataset, pd.DataFrame]],
         ],
+        aux_at_targets: Union[
+            xr.DataArray,
+            xr.Dataset,
+        ] = None,
         links: Union[Tuple, List[Tuple[int, int]], None] = None,
         context_delta_t: Union[int, List[int]] = 0,
         target_delta_t: Union[int, List[int]] = 0,
         time_freq: str = "D",
         xarray_interp_method: str = "linear",
         discrete_xarray_sampling: bool = False,
         dtype: object = "float32",
     ) -> None:
         """Initialise a TaskLoader object
 
-        :param context: Context data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
-            or a list/tuple of these.
-        :param target: Target data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
-            or a list/tuple of these.
-        :param links: Specifies links between context and target data. Each link is a tuple of
-            two integers, where the first integer is the index of the context data and the second
-            integer is the index of the target data. Can be a single tuple in the case of a single
-            link. If None, no links are specified. Default: None.
-        :param context_delta_t: Time difference between context data and t=0 (task init time).
-            Can be a single int (same for all context data) or a list/tuple of ints.
-        :param target_delta_t: Time difference between target data and t=0 (task init time).
-            Can be a single int (same for all target data) or a list/tuple of ints.
-        :param time_freq: Time frequency of the data. Default: 'D' (daily).
-        :param xarray_interp_method: Interpolation method to use when interpolating xr.DataArray
-        :param discrete_xarray_sampling: When randomly sampling xarray variables, whether to sample
-            at discrete points defined at grid cell centres, or at continuous points within the grid.
-            Default is False.
-        :param dtype: Data type of the data. Used to cast the data to the specified dtype.
-            Default: 'float32'.
+        Args:
+            context: Context data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
+                or a list/tuple of these.
+            target: Target data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
+                or a list/tuple of these.
+            aux_at_targets: Auxiliary data at target locations. Can be a single xr.DataArray or
+                xr.Dataset. Default: None.
+            links: Specifies links between context and target data. Each link is a tuple of
+                two integers, where the first integer is the index of the context data and the second
+                integer is the index of the target data. Can be a single tuple in the case of a single
+                link. If None, no links are specified. Default: None.
+            context_delta_t: Time difference between context data and t=0 (task init time).
+                Can be a single int (same for all context data) or a list/tuple of ints.
+            target_delta_t: Time difference between target data and t=0 (task init time).
+                Can be a single int (same for all target data) or a list/tuple of ints.
+            time_freq: Time frequency of the data. Default: 'D' (daily).
+            xarray_interp_method: Interpolation method to use when interpolating xr.DataArray
+            discrete_xarray_sampling: When randomly sampling xarray variables, whether to sample
+                at discrete points defined at grid cell centres, or at continuous points within the grid.
+                Default is False.
+            dtype: Data type of the data. Used to cast the data to the specified dtype.
+                Default: 'float32'.
         """
         self.time_freq = time_freq
         self.xarray_interp_method = xarray_interp_method
         self.discrete_xarray_sampling = discrete_xarray_sampling
         self.dtype = dtype
 
         if isinstance(context, (xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series)):
             context = (context,)
         if isinstance(target, (xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series)):
             target = (target,)
-        context, target = self.cast_context_and_target_to_dtype(context, target)
+        context, target, aux_at_targets = self._cast_context_and_target_to_dtype(
+            context, target, aux_at_targets
+        )
         self.context = context
         self.target = target
+        self.aux_at_targets = self._check_aux_at_targets(aux_at_targets)
 
         self.links = self.check_links(links)
 
         if isinstance(context_delta_t, int):
             context_delta_t = (context_delta_t,) * len(context)
         else:
             assert len(context_delta_t) == len(context)
         if isinstance(target_delta_t, int):
             target_delta_t = (target_delta_t,) * len(target)
         else:
             assert len(target_delta_t) == len(target)
         self.context_delta_t = context_delta_t
         self.target_delta_t = target_delta_t
 
-        self.context_dims, self.target_dims = self.count_context_and_target_data_dims()
+        (
+            self.context_dims,
+            self.target_dims,
+            self.aux_at_target_dims,
+        ) = self.count_context_and_target_data_dims()
         (
             self.context_var_IDs,
             self.target_var_IDs,
             self.context_var_IDs_and_delta_t,
             self.target_var_IDs_and_delta_t,
+            self.aux_at_target_var_IDs,
         ) = self.infer_context_and_target_var_IDs()
 
-    def cast_context_and_target_to_dtype(
-        self, context: List, target: List
+    def _cast_context_and_target_to_dtype(
+        self,
+        context: List,
+        target: List,
+        aux_at_targets=None,
     ) -> (List, List):
         """Cast context and target data to the default dtype.
 
         Returns
         -------
         context : tuple. Tuple of context data with specified dtype.
         target : tuple. Tuple of target data with specified dtype.
@@ -114,40 +132,55 @@
                 # x1/x2 coord dtypes during task sampling
             else:
                 raise ValueError(f"Unknown type {type(var)} for context set {var}")
             return var
 
         context = tuple([cast_to_dtype(var) for var in context])
         target = tuple([cast_to_dtype(var) for var in target])
+        if aux_at_targets is not None:
+            aux_at_targets = aux_at_targets.astype(self.dtype)
 
-        return context, target
+        return context, target, aux_at_targets
+
+    def _check_aux_at_targets(self, aux_at_targets):
+        if aux_at_targets is not None and "time" in aux_at_targets.coords:
+            raise ValueError(
+                "The auxiliary data at target locations should not have a time dimension."
+            )
+        return aux_at_targets
 
     def load_dask(self) -> None:
         """Load any `dask` data into memory"""
 
         def load(datasets):
+            if not isinstance(datasets, (tuple, list)):
+                datasets = [datasets]
             for i, var in enumerate(datasets):
                 if isinstance(var, (xr.DataArray, xr.Dataset)):
                     var = var.load()
 
         load(self.context)
         load(self.target)
+        load(self.aux_at_targets)
 
         return None
 
     def count_context_and_target_data_dims(self):
         """Count the number of data dimensions in the context and target data.
 
         Returns
         -------
         context_dims : tuple. Tuple of data dimensions in the context data.
         target_dims : tuple. Tuple of data dimensions in the target data.
         """
 
         def count_data_dims_of_tuple_of_sets(datasets):
+            if not isinstance(datasets, (tuple, list)):
+                datasets = [datasets]
+
             dims = []
             # Distinguish between xr.DataArray, xr.Dataset and pd.DataFrame
             for i, var in enumerate(datasets):
                 if isinstance(var, xr.Dataset):
                     dim = len(var.data_vars)  # Multiple data variables
                 elif isinstance(var, xr.DataArray):
                     dim = 1  # Single data variable
@@ -158,28 +191,37 @@
                 else:
                     raise ValueError(f"Unknown type {type(var)} for context set {var}")
                 dims.append(dim)
             return tuple(dims)
 
         context_dims = count_data_dims_of_tuple_of_sets(self.context)
         target_dims = count_data_dims_of_tuple_of_sets(self.target)
+        if self.aux_at_targets is not None:
+            aux_at_target_dims = count_data_dims_of_tuple_of_sets(self.aux_at_targets)[
+                0
+            ]
+        else:
+            aux_at_target_dims = 0
 
-        return context_dims, target_dims
+        return context_dims, target_dims, aux_at_target_dims
 
     def infer_context_and_target_var_IDs(self):
         """Infer the variable IDs of the context and target data.
 
         Returns
         -------
         context_var_IDs : tuple. Tuple of variable IDs in the context data.
         target_var_IDs : tuple. Tuple of variable IDs in the target data.
         """
 
         def infer_var_IDs_of_tuple_of_sets(datasets, delta_ts=None):
             """If delta_ts is not None, then add the delta_t to the variable ID"""
+            if not isinstance(datasets, (tuple, list)):
+                datasets = [datasets]
+
             var_IDs = []
             # Distinguish between xr.DataArray, xr.Dataset and pd.DataFrame
             for i, var in enumerate(datasets):
                 if isinstance(var, xr.DataArray):
                     var_ID = (var.name,)  # Single data variable
                 elif isinstance(var, xr.Dataset):
                     var_ID = tuple(var.data_vars.keys())  # Multiple data variables
@@ -207,19 +249,27 @@
             self.context, self.context_delta_t
         )
         target_var_IDs = infer_var_IDs_of_tuple_of_sets(self.target)
         target_var_IDs_and_delta_t = infer_var_IDs_of_tuple_of_sets(
             self.target, self.target_delta_t
         )
 
+        if self.aux_at_targets is not None:
+            aux_at_target_var_IDs = infer_var_IDs_of_tuple_of_sets(self.aux_at_targets)[
+                0
+            ]
+        else:
+            aux_at_target_var_IDs = None
+
         return (
             context_var_IDs,
             target_var_IDs,
             context_var_IDs_and_delta_t,
             target_var_IDs_and_delta_t,
+            aux_at_target_var_IDs,
         )
 
     def check_links(self, links):
         """Check that the context-target links are valid."""
         if links is None:
             return None
 
@@ -252,31 +302,33 @@
             if not isinstance(self.target[target_idx], (pd.DataFrame, pd.Series)):
                 raise ValueError(
                     f"Target set {target_idx} must be a pandas object when using the 'split' sampling strategy"
                 )
 
         return links
 
+    def __str__(self):
+        """String representation of the TaskLoader object (user-friendly)"""
+        s = f"TaskLoader({len(self.context)} context sets, {len(self.target)} target sets)"
+        s += f"\nContext variable IDs: {self.context_var_IDs}"
+        s += f"\nTarget variable IDs: {self.target_var_IDs}"
+        if self.aux_at_targets is not None:
+            s += f"\nAuxiliary data at targets: {self.aux_at_target_var_IDs}"
+        return s
+
     def __repr__(self):
         """Representation of the TaskLoader object (for developers)
 
         TODO make this a more verbose version of __str__
         """
-        s = f"TaskLoader({len(self.context)} context sets, {len(self.target)} target sets)"
-        s += f"\nContext variable IDs: {self.context_var_IDs_and_delta_t}"
-        s += f"\nTarget variable IDs: {self.target_var_IDs_and_delta_t}"
+        s = str(self)
         s += f"\nContext data dimensions: {self.context_dims}"
         s += f"\nTarget data dimensions: {self.target_dims}"
-        return s
-
-    def __str__(self):
-        """String representation of the TaskLoader object (user-friendly)"""
-        s = f"TaskLoader({len(self.context)} context sets, {len(self.target)} target sets)"
-        s += f"\nContext variable IDs: {self.context_var_IDs}"
-        s += f"\nTarget variable IDs: {self.target_var_IDs}"
+        if self.aux_at_targets is not None:
+            s += f"\nAuxiliary data dimensions: {self.aux_at_target_dims}"
         return s
 
     def sample_da(
         self,
         da: Union[xr.DataArray, xr.Dataset],
         sampling_strat: Union[str, int, float, np.ndarray],
         seed: int = None,
@@ -408,14 +460,30 @@
         else:
             raise InvalidSamplingStrategyError(
                 f"Unknown sampling strategy {sampling_strat}"
             )
 
         return X_c, Y_c
 
+    def sample_aux_t(self, X_t: Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]):
+        if isinstance(X_t, tuple):
+            xt1, xt2 = X_t
+        else:
+            xt1, xt2 = xr.DataArray(X_t[0]), xr.DataArray(X_t[1])
+        Y_t_aux = self.aux_at_targets.sel(x1=xt1, x2=xt2, method="nearest")
+        if isinstance(Y_t_aux, xr.Dataset):
+            Y_t_aux = Y_t_aux.to_array()
+        Y_t_aux = np.array(Y_t_aux, dtype=np.float32)
+        if (isinstance(X_t, tuple) and Y_t_aux.ndim == 2) or (
+            isinstance(X_t, np.ndarray) and Y_t_aux.ndim == 1
+        ):
+            # Reshape to (variable, *spatial_dims)
+            Y_t_aux = Y_t_aux.reshape(1, *Y_t_aux.shape)
+        return Y_t_aux
+
     def task_generation(
         self,
         date: pd.Timestamp,
         context_sampling: Union[
             str, int, float, np.ndarray, List[Union[str, int, float, np.ndarray]]
         ] = "all",
         target_sampling: Union[
@@ -602,14 +670,22 @@
             task[f"Y_c"].append(Y_c)
         for j, (var, sampling_strat) in enumerate(zip(target_slices, target_sampling)):
             target_seed = seed + i + j if seed is not None else None
             X_t, Y_t = sample_variable(var, sampling_strat, target_seed)
             task[f"X_t"].append(X_t)
             task[f"Y_t"].append(Y_t)
 
+        if self.aux_at_targets is not None:
+            # Add auxiliary variable to target set
+            if len(task["X_t"]) > 1:
+                raise ValueError(
+                    "Cannot add auxiliary variable to target set when there are multiple target variables"
+                )
+            task["Y_t_aux"] = self.sample_aux_t(task["X_t"][0])
+
         return Task(task)
 
     def __call__(self, date, *args, **kwargs):
         if isinstance(date, (list, tuple, pd.core.indexes.datetimes.DatetimeIndex)):
             return [self.task_generation(d, *args, **kwargs) for d in date]
         else:
             return self.task_generation(date, *args, **kwargs)
```

### Comparing `deepsensor-0.1.5/deepsensor/data/processor.py` & `deepsensor-0.1.6/deepsensor/data/processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/data/task.py` & `deepsensor-0.1.6/deepsensor/data/task.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/data/utils.py` & `deepsensor-0.1.6/deepsensor/data/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/errors.py` & `deepsensor-0.1.6/deepsensor/errors.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/model/convnp.py` & `deepsensor-0.1.6/deepsensor/model/convnp.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,23 @@
                 print(f"dim_yc inferred from TaskLoader: {dim_yc}")
             kwargs["dim_yc"] = dim_yc
         if "dim_yt" not in kwargs:
             dim_yt = sum(task_loader.target_dims)  # Must be an int
             if verbose:
                 print(f"dim_yt inferred from TaskLoader: {dim_yt}")
             kwargs["dim_yt"] = dim_yt
+        if "dim_aux_t" not in kwargs:
+            dim_aux_t = task_loader.aux_at_target_dims
+            if verbose:
+                print(f"dim_aux_t inferred from TaskLoader: {dim_aux_t}")
+            kwargs["dim_aux_t"] = dim_aux_t
+        if "aux_t_mlp_layers" not in kwargs and kwargs["dim_aux_t"] > 0:
+            kwargs["aux_t_mlp_layers"] = (64,) * 3
+            if verbose:
+                print(f"Setting aux_t_mlp_layers: {kwargs['aux_t_mlp_layers']}")
         if "points_per_unit" not in kwargs:
             ppu = gen_ppu(task_loader)
             if verbose:
                 print(f"points_per_unit inferred from TaskLoader: {ppu}")
             kwargs["points_per_unit"] = ppu
         if "encoder_scales" not in kwargs:
             encoder_scales = gen_encoder_scales(kwargs["points_per_unit"], task_loader)
@@ -579,9 +588,11 @@
         if B.any(Y_t_nans):
             if isinstance(X, tuple):
                 # Gridded data
                 X = flatten_X(X)
                 Y = flatten_Y(Y)
             task["X_t"][i] = X[:, ~Y_t_nans]
             task["Y_t"][i] = Y[:, ~Y_t_nans]
+            if "Y_t_aux" in task.keys():
+                task["Y_t_aux"] = task["Y_t_aux"][:, ~Y_t_nans]
 
     return task, True
```

### Comparing `deepsensor-0.1.5/deepsensor/model/defaults.py` & `deepsensor-0.1.6/deepsensor/model/defaults.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/model/model.py` & `deepsensor-0.1.6/deepsensor/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
-from deepsensor.data.task import Task
+from deepsensor.data.task import Task, flatten_X
 
 from typing import List, Union
 import copy
 
 import time
 from tqdm import tqdm
 
@@ -17,15 +17,14 @@
 # For dispatching with TF and PyTorch model types when they have not yet been loaded.
 # See https://beartype.github.io/plum/types.html#moduletype
 
 
 def create_empty_spatiotemporal_xarray(
     X: Union[xr.Dataset, xr.DataArray],
     dates: List,
-    resolution_factor: Union[float, int] = 1.0,
     coord_names: dict = {"x1": "x1", "x2": "x2"},
     data_vars: List = ["var"],
     prepend_dims: List[str] = None,
     prepend_coords: dict = None,
 ):
     if prepend_dims is None:
         prepend_dims = []
@@ -35,40 +34,23 @@
     # Check for any repeated data_vars
     if len(data_vars) != len(set(data_vars)):
         raise ValueError(
             f"Duplicate data_vars found in data_vars: {data_vars}. "
             "This would cause the xarray.Dataset to have fewer variables than expected."
         )
 
-    x1_raw = X.coords[coord_names["x1"]]
-    x2_raw = X.coords[coord_names["x2"]]
+    x1_predict = X.coords[coord_names["x1"]]
+    x2_predict = X.coords[coord_names["x2"]]
 
     # Assert uniform spacing
-    if not np.allclose(np.diff(x1_raw), np.diff(x1_raw)[0]):
+    if not np.allclose(np.diff(x1_predict), np.diff(x1_predict)[0]):
         raise ValueError(f"Coordinate {coord_names['x1']} must be uniformly spaced.")
-    if not np.allclose(np.diff(x2_raw), np.diff(x2_raw)[0]):
+    if not np.allclose(np.diff(x2_predict), np.diff(x2_predict)[0]):
         raise ValueError(f"Coordinate {coord_names['x2']} must be uniformly spaced.")
 
-    if resolution_factor == 1.0:
-        x1_predict = x1_raw
-        x2_predict = x2_raw
-    else:
-        x1_predict = np.linspace(
-            x1_raw[0],
-            x1_raw[-1],
-            int(x1_raw.size * resolution_factor),
-            dtype="float32",
-        )
-        x2_predict = np.linspace(
-            x2_raw[0],
-            x2_raw[-1],
-            int(x2_raw.size * resolution_factor),
-            dtype="float32",
-        )
-
     if len(prepend_dims) != len(set(prepend_dims)):
         # TODO unit test
         raise ValueError(
             f"Length of prepend_dims ({len(prepend_dims)}) must be equal to length of "
             f"prepend_coords ({len(prepend_coords)})."
         )
 
@@ -90,14 +72,30 @@
     # TODO: Convert init time to forecast time?
     # pred_ds = pred_ds.assign_coords(
     #     time=pred_ds['time'] + pd.Timedelta(days=task_loader.target_delta_t[0]))
 
     return pred_ds
 
 
+def increase_spatial_resolution(
+    X_t_normalised, resolution_factor, coord_names: dict = {"x1": "x1", "x2": "x2"}
+):
+    # TODO wasteful to interpolate X_t_normalised
+    assert isinstance(resolution_factor, (float, int))
+    assert isinstance(X_t_normalised, (xr.DataArray, xr.Dataset))
+    x1_name, x2_name = coord_names["x1"], coord_names["x2"]
+    x1, x2 = X_t_normalised.coords[x1_name], X_t_normalised.coords[x2_name]
+    x1 = np.linspace(x1[0], x1[-1], int(x1.size * resolution_factor), dtype="float64")
+    x2 = np.linspace(x2[0], x2[-1], int(x2.size * resolution_factor), dtype="float64")
+    X_t_normalised = X_t_normalised.interp(
+        **{x1_name: x1, x2_name: x2}, method="nearest"
+    )
+    return X_t_normalised
+
+
 class ProbabilisticModel:
 
     """
     Base class for probabilistic model used for DeepSensor.
     Ensures a set of methods required for DeepSensor
     are implemented by specific model classes that inherit from it.
     """
@@ -305,14 +303,19 @@
             # Unnormalise coords to use for xarray/pandas objects for storing predictions
             X_t = self.data_processor.map_coords(X_t, unnorm=True)
         else:
             # Normalise coords to use for model
             X_t_normalised = self.data_processor.map_coords(X_t)
 
         if mode == "on-grid":
+            if resolution_factor != 1:
+                X_t_normalised = increase_spatial_resolution(
+                    X_t_normalised, resolution_factor
+                )
+            # TODO rename from _arr because not an array here
             X_t_arr = (X_t_normalised["x1"].values, X_t_normalised["x2"].values)
         elif mode == "off-grid":
             X_t_arr = X_t_normalised.reset_index()[["x1", "x2"]].values.T
 
         if not unnormalise:
             X_t = X_t_normalised
             coord_names = {"x1": "x1", "x2": "x2"}
@@ -320,33 +323,34 @@
             coord_names = {
                 "x1": self.data_processor.raw_spatial_coord_names[0],
                 "x2": self.data_processor.raw_spatial_coord_names[1],
             }
 
         # Create empty xarray/pandas objects to store predictions
         if mode == "on-grid":
+            if resolution_factor != 1:
+                X_t = increase_spatial_resolution(
+                    X_t, resolution_factor, coord_names=coord_names
+                )
             mean = create_empty_spatiotemporal_xarray(
                 X_t,
                 dates,
-                resolution_factor,
                 data_vars=target_var_IDs,
                 coord_names=coord_names,
             ).to_array(dim="data_var")
             std = create_empty_spatiotemporal_xarray(
                 X_t,
                 dates,
-                resolution_factor,
                 data_vars=target_var_IDs,
                 coord_names=coord_names,
             ).to_array(dim="data_var")
             if n_samples >= 1:
                 samples = create_empty_spatiotemporal_xarray(
                     X_t,
                     dates,
-                    resolution_factor,
                     data_vars=target_var_IDs,
                     coord_names=coord_names,
                     prepend_dims=["sample"],
                     prepend_coords={"sample": np.arange(n_samples)},
                 ).to_array(dim="data_var")
         elif mode == "off-grid":
             # Repeat target locs for each date to create multiindex
@@ -381,14 +385,18 @@
 
         # Don't change tasks by reference when overriding target locations
         tasks = copy.deepcopy(tasks)
 
         for task in tqdm(tasks, position=0, disable=progress_bar < 1, leave=True):
             task["X_t"] = [X_t_arr for _ in range(len(task["X_t"]))]
 
+            # If passing auxiliary data, need to sample it at target locations
+            if "Y_t_aux" in task.keys():
+                task["Y_t_aux"] = self.task_loader.sample_aux_t(X_t_arr)
+
             # If `DeepSensor` model child has been sub-classed with a `__call__` method,
             # we assume this is a distribution-like object that can be used to compute
             # mean, std and samples. Otherwise, run the model with `Task` for each prediction type.
             if hasattr(self, "__call__"):
                 # Run model forwards once to generate output distribution, which we re-use
                 dist = self(task, n_samples=n_samples)
                 mean_arr = self.mean(dist)
```

### Comparing `deepsensor-0.1.5/deepsensor/model/nps.py` & `deepsensor-0.1.6/deepsensor/model/nps.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         yt = B.concat(*task["Y_t"], axis=1)
     else:
         raise ValueError(
             f"Incorrect target locations and target observations (got {len(task['X_t'])} and {len(task['Y_t'])})"
         )
 
     model_kwargs = {}
-    if "Y_target_auxiliary" in task.keys():
-        model_kwargs["aux_t"] = task["Y_target_auxiliary"]
+    if "Y_t_aux" in task.keys():
+        model_kwargs["aux_t"] = task["Y_t_aux"]
 
     return context_data, xt, yt, model_kwargs
 
 
 def run_nps_model(neural_process, task, n_samples=None, requires_grad=False):
     """Run `neuralprocesses` model"""
     context_data, xt, _, model_kwargs = convert_task_to_nps_args(task)
```

### Comparing `deepsensor-0.1.5/deepsensor/plot.py` & `deepsensor-0.1.6/deepsensor/plot.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.6/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/torch/__init__.py` & `deepsensor-0.1.6/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor/train/train.py` & `deepsensor-0.1.6/deepsensor/train/train.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.6/deepsensor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
@@ -26,18 +26,22 @@
 
 -----------
 
 [![release](https://img.shields.io/badge/release-v0.1.5-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/tom-andersson/deepsensor/blob/main/LICENSE)
 
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
+For demonstrators, use cases, and videos showcasing the functionality of DeepSensor, check out the
+[DeepSensor Gallery](https://github.com/tom-andersson/deepsensor_gallery)!
+
 Why neural processes?
 -----------
 NPs are a highly flexible class of probabilistic models that can:
 - ingest multiple context sets (i.e. data streams) containing gridded or pointwise observations
 - handle multiple gridded resolutions
 - predict at arbitrary target locations
 - quantify prediction uncertainty
@@ -147,15 +151,15 @@
            40.0 250.0  277.947373
 2014-12-02 50.0 280.0   261.08943
            40.0 250.0  278.219599
 2014-12-03 50.0 280.0  257.128185
            40.0 250.0  278.444229
 ```
 
-This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/quickstart_example.ipynb) with added visualisations.
+This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor_demos/blob/main/demonstrators/quickstart.ipynb) with added visualisations.
 
 Extending DeepSensor with new models
 ----------
 To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
 and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
 such as `.mean` and `.stddev`.
 ```python
@@ -171,21 +175,9 @@
     def stddev(self, task: Task):
         """Compute stddev at target locations"""
         return 0.1
     
     ...
 ```
 `NewModel` can then be used in the same way as the built-in `ConvNP` model.
-See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/extending_models.ipynb)
+See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor_gallery/blob/main/demonstrators/extending_models.ipynb)
 for more details.
-
-Learn more
-----------
-- Documentation: TODO
-- Issue tracker: https://github.com/tom-andersson/deepsensor/issues
-- Source code: https://github.com/tom-andersson/deepsensor
-
-**Talks**
-- Environmental Sensor Placement with ConvGNPs: https://youtu.be/v0pmqh09u1Y
-
-**Papers**
-- TODO
```

### Comparing `deepsensor-0.1.5/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.6/deepsensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/setup.cfg` & `deepsensor-0.1.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepsensor
-version = 0.1.5
+version = 0.1.6
 author = Tom R. Andersson
 author_email = tomand@bas.ac.uk
 description = A Python package for modelling xarray and pandas data with neural processes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tom-andersson/deepsensor
 license = MIT
```

### Comparing `deepsensor-0.1.5/tests/test_active_learning.py` & `deepsensor-0.1.6/tests/test_active_learning.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Stddev,
     ExpectedImprovement,
     Random,
     OracleMAE,
     OracleRMSE,
     OracleMarginalNLL,
     OracleJointNLL,
+    AcquisitionFunction,
 )
 from deepsensor.active_learning.algorithms import GreedyAlgorithm
 
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor, xarray_to_coord_array_normalised
 from deepsensor.data.task import append_obs_to_task
 from deepsensor.errors import TaskSetIndexError, GriddedDataError
@@ -144,15 +145,15 @@
                 model=self.model,
                 X_t=self.ds_raw,
                 X_s=self.ds_raw,
                 N_new_context=10_000,  # > number of search points
             )
 
     def test_acquisition_fns_run(self):
-        """Run each acquisition function to check that it runs without error"""
+        """Run each acquisition function to check that it runs and returns correct shape"""
         sequential_acquisition_fns = [
             MeanStddev(self.model),
             MeanVariance(self.model),
             pNormStddev(self.model, p=3),
             MeanMarginalEntropy(self.model),
             JointEntropy(self.model),
             OracleMAE(self.model),
@@ -199,15 +200,53 @@
         )
 
         task = self.task_loader("2014-12-31", context_sampling=10)
 
         for acquisition_fn in acquisition_fns:
             X_new_df, acquisition_fn_ds = alg(acquisition_fn, task)
 
-    def test_oracle_acquisition_fn_without_task_loader_raises_value_error(self):
+    def test_greedy_alg_with_oracle_acquisition_fn(self):
+        acquisition_fn = OracleMAE(self.model)
+
+        # Coarsen search points to speed up computation
+        X_s = self.ds_raw.air.coarsen(lat=10, lon=10, boundary="trim").mean()
+
+        alg = GreedyAlgorithm(
+            model=self.model,
+            X_t=X_s,
+            X_s=X_s,
+            N_new_context=2,
+            task_loader=self.task_loader,
+        )
+
+        task = self.task_loader("2014-12-31", context_sampling=10)
+
+        _ = alg(acquisition_fn, task)
+
+    def test_greedy_alg_with_sequential_acquisition_fn(self):
+        acquisition_fn = Stddev(self.model)
+
+        # Coarsen search points to speed up computation
+        X_s = self.ds_raw.air.coarsen(lat=10, lon=10, boundary="trim").mean()
+
+        alg = GreedyAlgorithm(
+            model=self.model,
+            X_t=X_s,
+            X_s=X_s,
+            N_new_context=2,
+            task_loader=self.task_loader,
+        )
+
+        task = self.task_loader("2014-12-31", context_sampling=10)
+
+        _ = alg(acquisition_fn, task)
+
+    def test_greedy_alg_with_oracle_acquisition_fn_without_task_loader_raises_value_error(
+        self,
+    ):
         acquisition_fn = OracleMAE(self.model)
 
         # Coarsen search points to speed up computation
         X_s = self.ds_raw.air.coarsen(lat=10, lon=10, boundary="trim").mean()
 
         alg = GreedyAlgorithm(
             model=self.model,
@@ -216,7 +255,28 @@
             N_new_context=2,
         )
 
         task = self.task_loader("2014-12-31", context_sampling=10)
 
         with self.assertRaises(ValueError):
             _ = alg(acquisition_fn, task)
+
+    def assert_acquisition_fn_without_min_or_max_raises_error(
+        self,
+    ):
+        class DummyAcquisitionFn(AcquisitionFunction):
+            """Dummy acquisition function that doesn't set min or max"""
+
+            def __call__(self, **kwargs):
+                return np.zeros(1)
+
+        acquisition_fn = DummyAcquisitionFn(self.model)
+
+        X_s = self.ds_raw.air
+
+        with self.assertRaises(ValueError):
+            alg = GreedyAlgorithm(
+                model=self.model,
+                X_t=X_s,
+                X_s=X_s,
+                N_new_context=2,
+            )
```

### Comparing `deepsensor-0.1.5/tests/test_data_processor.py` & `deepsensor-0.1.6/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/tests/test_model.py` & `deepsensor-0.1.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/tests/test_plotting.py` & `deepsensor-0.1.6/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/tests/test_task_loader.py` & `deepsensor-0.1.6/tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/tests/test_training.py` & `deepsensor-0.1.6/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.5/tests/utils.py` & `deepsensor-0.1.6/tests/utils.py`

 * *Files identical despite different names*

