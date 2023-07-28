# Comparing `tmp/hyperopt_prophet-0.2.2.tar.gz` & `tmp/hyperopt_prophet-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.2.2.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.2.3.tar", max compression
```

## Comparing `hyperopt_prophet-0.2.2.tar` & `hyperopt_prophet-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-07-28 01:04:39.039918 hyperopt_prophet-0.2.2/LICENSE
--rw-r--r--   0        0        0      980 2023-07-28 01:04:39.039918 hyperopt_prophet-0.2.2/README.md
--rw-r--r--   0        0        0      118 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0     5047 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    15953 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/hyperopt_prophet/model.py
--rw-r--r--   0        0        0     9216 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/hyperopt_prophet/training.py
--rw-r--r--   0        0        0    10777 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/main.py
--rw-r--r--   0        0        0      803 2023-07-28 01:04:39.079918 hyperopt_prophet-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 hyperopt_prophet-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-28 02:05:40.057166 hyperopt_prophet-0.2.3/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-28 02:05:40.057166 hyperopt_prophet-0.2.3/README.md
+-rw-r--r--   0        0        0      118 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0     5047 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    15953 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0     9206 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0    10777 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/main.py
+-rw-r--r--   0        0        0      821 2023-07-28 02:05:40.097169 hyperopt_prophet-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 hyperopt_prophet-0.2.3/PKG-INFO
```

### Comparing `hyperopt_prophet-0.2.2/LICENSE` & `hyperopt_prophet-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.2/README.md` & `hyperopt_prophet-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.2/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.2.3/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.2/hyperopt_prophet/model.py` & `hyperopt_prophet-0.2.3/hyperopt_prophet/model.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.2/hyperopt_prophet/training.py` & `hyperopt_prophet-0.2.3/hyperopt_prophet/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,24 +169,24 @@
             model_json=model_json,
             horizon=self.training_params.horizon,
             frequency=self.training_params.unit,
             time_col=self.training_params.time_col,
             regressors=self.training_params.regressors,
         )
 
-        # prediction = prophet_model.predict_timeseries(
-        #     horizon=self.training_params.horizon, include_history=True
-        # )
+        prediction = prophet_model.predict_timeseries(
+            horizon=self.training_params.horizon, include_history=True
+        )
 
         result["run_id"] = "local_training"
 
         # calculate the duration of the run in seconds
         result["training_duration"] = time() - run_start_time
 
-        return prophet_model, model_json, result, avg_metrics  # , prediction
+        return prophet_model, model_json, result, avg_metrics, prediction
 
     def train_with_mlflow(self, mlflow_run):
         prophet_model, model_json, result, avg_metrics, prediction = self.training()
 
         # Generate sample input dataframe
         sample_input = self.training_data.head(20)
         sample_input[self.training_params.time_col] = pd.to_datetime(
```

### Comparing `hyperopt_prophet-0.2.2/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.2.3/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.2.2/pyproject.toml` & `hyperopt_prophet-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.2.2"
+version = "0.2.3"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 prophet = "1.1.1"
 holidays = "0.24"
+plotly = "5.15.0"
 pandas = "^2.0.3"
 pydantic = "^2.1.0"
 hyperopt = "0.2.7"
 mlflow = "2.5.0"
 cloudpickle = "^2.2.1"
 cython = "^3.0.0"
 mlflowops = '^0.1.2'
```

### Comparing `hyperopt_prophet-0.2.2/PKG-INFO` & `hyperopt_prophet-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.2.2
+Version: 0.2.3
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: cython (>=3.0.0,<4.0.0)
 Requires-Dist: holidays (==0.24)
 Requires-Dist: hyperopt (==0.2.7)
 Requires-Dist: mlflow (==2.5.0)
 Requires-Dist: mlflowops (>=0.1.2,<0.2.0)
 Requires-Dist: nbformat (>=5.9.1,<6.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: plotly (==5.15.0)
 Requires-Dist: prophet (==1.1.1)
 Requires-Dist: pydantic (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Hyperopt Prophet
 
 **Integration of prophet forecasting with hyperopt, mlflow**
```

