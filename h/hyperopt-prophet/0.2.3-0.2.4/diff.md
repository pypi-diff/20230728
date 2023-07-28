# Comparing `tmp/hyperopt_prophet-0.2.3.tar.gz` & `tmp/hyperopt_prophet-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.2.3.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.2.4.tar", max compression
```

## Comparing `hyperopt_prophet-0.2.3.tar` & `hyperopt_prophet-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-07-28 02:05:40.057166 hyperopt_prophet-0.2.3/LICENSE
--rw-r--r--   0        0        0      980 2023-07-28 02:05:40.057166 hyperopt_prophet-0.2.3/README.md
--rw-r--r--   0        0        0      118 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0     5047 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    15953 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/model.py
--rw-r--r--   0        0        0     9206 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/training.py
--rw-r--r--   0        0        0    10777 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/main.py
--rw-r--r--   0        0        0      821 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 hyperopt_prophet-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-28 04:02:44.355848 hyperopt_prophet-0.2.4/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-28 04:02:44.355848 hyperopt_prophet-0.2.4/README.md
+-rw-r--r--   0        0        0      118 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0     5047 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    15979 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0     9233 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0    10777 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/main.py
+-rw-r--r--   0        0        0      821 2023-07-28 04:02:44.395848 hyperopt_prophet-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 hyperopt_prophet-0.2.4/PKG-INFO
```

### Comparing `hyperopt_prophet-0.2.3/LICENSE` & `hyperopt_prophet-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.3/README.md` & `hyperopt_prophet-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.3/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.2.4/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.3/hyperopt_prophet/model.py` & `hyperopt_prophet-0.2.4/hyperopt_prophet/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     OFFSET_ALIAS_MAP,
     generate_cutoffs,
     get_validation_horizon,
     is_quaterly_alias,
 )
 
 import logging
-
-logging.getLogger("prophet").setLevel(logging.WARNING)
-logging.getLogger("cmdstanpy").setLevel(logging.WARNING)
-
+logger = logging.getLogger('cmdstanpy')
+logger.addHandler(logging.NullHandler())
+logger.propagate = False
+logger.setLevel(logging.CRITICAL)
 
 class ForecastModel(ABC, mlflow.pyfunc.PythonModel):
     @abstractmethod
     def __init__(self):
         super().__init__()
 
     @property
```

### Comparing `hyperopt_prophet-0.2.3/hyperopt_prophet/training.py` & `hyperopt_prophet-0.2.4/hyperopt_prophet/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from mlflowops import MLFlowOps
 from pydantic import BaseModel
 
 from .model import ProphetHyperoptEstimator, mlflow_prophet_log_model, ProphetModel
 from .utils import get_plotly_forecast, plotly_fig2pil
 
 import logging
-
-logging.getLogger("prophet").setLevel(logging.WARNING)
-logging.getLogger("cmdstanpy").setLevel(logging.WARNING)
+logger = logging.getLogger('cmdstanpy')
+logger.addHandler(logging.NullHandler())
+logger.propagate = False
+logger.setLevel(logging.CRITICAL)
 
 
 warnings.filterwarnings("ignore")
 
 
 class ProphetTrainingParams(BaseModel):
     """
```

### Comparing `hyperopt_prophet-0.2.3/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.2.4/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.3/pyproject.toml` & `hyperopt_prophet-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.2.3"
+version = "0.2.4"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
```

### Comparing `hyperopt_prophet-0.2.3/PKG-INFO` & `hyperopt_prophet-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.2.3
+Version: 0.2.4
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

