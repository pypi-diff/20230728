# Comparing `tmp/bojaxns-1.0.4.tar.gz` & `tmp/bojaxns-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bojaxns-1.0.4.tar", last modified: Tue Jul 25 17:11:43 2023, max compression
+gzip compressed data, was "bojaxns-1.0.5.tar", last modified: Fri Jul 28 19:18:55 2023, max compression
```

## Comparing `bojaxns-1.0.4.tar` & `bojaxns-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.346069 bojaxns-1.0.4/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.4/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 17:11:43.346069 bojaxns-1.0.4/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.4/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/base.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.4/bojaxns/basic.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/experiment.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/
--rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11415 2023-07-25 15:21:05.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15709 2023-07-25 17:10:14.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/distribution_math.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5288 2023-07-25 15:21:05.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9505 2023-07-25 17:10:14.000000 bojaxns-1.0.4/bojaxns/service.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/test_experiment.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/test_parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.4/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-25 17:11:43.346069 bojaxns-1.0.4/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-25 17:11:12.000000 bojaxns-1.0.4/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 19:18:55.044353 bojaxns-1.0.5/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.5/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-28 19:18:55.044353 bojaxns-1.0.5/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.5/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 19:18:55.044353 bojaxns-1.0.5/bojaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/base.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.5/bojaxns/basic.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      343 2023-07-27 22:17:59.000000 bojaxns-1.0.5/bojaxns/common.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3064 2023-07-27 22:17:59.000000 bojaxns-1.0.5/bojaxns/experiment.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 19:18:55.044353 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11415 2023-07-25 15:21:05.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15709 2023-07-25 17:10:14.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/distribution_math.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 19:18:55.044353 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5288 2023-07-25 15:21:05.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     8106 2023-07-28 17:19:30.000000 bojaxns-1.0.5/bojaxns/parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9893 2023-07-28 18:59:26.000000 bojaxns-1.0.5/bojaxns/service.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 19:18:55.044353 bojaxns-1.0.5/bojaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2207 2023-07-28 16:56:36.000000 bojaxns-1.0.5/bojaxns/tests/test_experiment.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5910 2023-07-28 17:20:52.000000 bojaxns-1.0.5/bojaxns/tests/test_parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.5/bojaxns/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 19:18:55.044353 bojaxns-1.0.5/bojaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-28 19:18:55.000000 bojaxns-1.0.5/bojaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      914 2023-07-28 19:18:55.000000 bojaxns-1.0.5/bojaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-28 19:18:55.000000 bojaxns-1.0.5/bojaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-28 19:18:55.000000 bojaxns-1.0.5/bojaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.5/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-28 19:18:55.044353 bojaxns-1.0.5/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-28 18:59:26.000000 bojaxns-1.0.5/setup.py
```

### Comparing `bojaxns-1.0.4/LICENSE` & `bojaxns-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/PKG-INFO` & `bojaxns-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bojaxns-1.0.4/README.md` & `bojaxns-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/base.py` & `bojaxns-1.0.5/bojaxns/base.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/basic.py` & `bojaxns-1.0.5/bojaxns/basic.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/experiment.py` & `bojaxns-1.0.5/bojaxns/experiment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 from datetime import datetime
-from typing import Literal, List, Dict, Union
+from typing import Dict
 from uuid import uuid4
 
-from pydantic import BaseModel, Field, validator, conint, confloat
+from pydantic import BaseModel, Field, validator, conint
 
+from bojaxns.common import FloatValue, ParamValues, UValue
 from bojaxns.parameter_space import ParameterSpace
 from bojaxns.utils import current_utc, build_example
 
 __all__ = [
-    'FloatValue',
-    'IntValue',
     'Trial',
     'TrialUpdate',
     'OptimisationExperiment',
     'NewExperimentRequest',
 ]
 
 
-class FloatValue(BaseModel):
-    type: Literal['float'] = 'float'
-    value: float
-
-
-class IntValue(BaseModel):
-    type: Literal['int'] = 'int'
-    value: int
-
-
 class TrialUpdate(BaseModel):
     ref_id: str = Field(
         description="An identifier of the measurement, e.g. user UUID.",
         example=str(uuid4())
     )
     measurement_dt: datetime = Field(
         default_factory=current_utc,
@@ -50,19 +39,19 @@
         example=str(uuid4())
     )
     create_dt: datetime = Field(
         default_factory=current_utc,
         description='The datetime the param_value was determined.',
         example=current_utc()
     )
-    param_values: Dict[str, Union[FloatValue, IntValue]] = Field(
+    param_values: ParamValues = Field(
         description="The parameter mapping for trial.",
         example={'price': FloatValue(value=1.)}
     )
-    U_value: List[confloat(ge=0., le=1.)] = Field(
+    U_value: UValue = Field(
         description="The U-space value of parameters.",
         example=[0.2]
     )
     trial_updates: Dict[str, TrialUpdate] = Field(
         default_factory=dict,
         description="The measurement of trial updates.",
         example={"124": build_example(TrialUpdate)}
```

### Comparing `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/bayesian_optimiser.py` & `bojaxns-1.0.5/bojaxns/gaussian_process_formulation/bayesian_optimiser.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/distribution_math.py` & `bojaxns-1.0.5/bojaxns/gaussian_process_formulation/distribution_math.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/multi_step_lookahead.py` & `bojaxns-1.0.5/bojaxns/gaussian_process_formulation/multi_step_lookahead.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py` & `bojaxns-1.0.5/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py` & `bojaxns-1.0.5/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/service.py` & `bojaxns-1.0.5/bojaxns/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import numpy as np
 import pylab as plt
 from jax import random, numpy as jnp
 from jax._src.random import PRNGKey
 from jaxns.prior import parse_prior, PriorModelType, transform
 from matplotlib import dates as mdates
 
-from bojaxns.experiment import OptimisationExperiment, NewExperimentRequest, Trial, FloatValue, \
-    IntValue, TrialUpdate
+from bojaxns.common import FloatValue, IntValue, ParamValues
+from bojaxns.experiment import OptimisationExperiment, NewExperimentRequest, Trial, TrialUpdate
 from bojaxns.gaussian_process_formulation.bayesian_optimiser import BayesianOptimiser
-from bojaxns.parameter_space import build_prior_model, ContinuousPrior, IntegerPrior, CategoricalPrior
+from bojaxns.parameter_space import build_prior_model, ContinuousPrior, IntegerPrior, CategoricalPrior, sample_U_value
 from bojaxns.utils import latin_hypercube
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 __all__ = [
     'InvalidTrial',
@@ -72,14 +72,20 @@
                 continue
             if isinstance(param.prior, CategoricalPrior):
                 param_values[param.name] = IntValue(value=int(val))
                 continue
         trial = Trial(param_values=param_values, U_value=U.tolist())
         return trial
 
+    def add_trial_from_data(self, key: PRNGKey, param_values: ParamValues) -> str:
+        U = sample_U_value(key=key, param_space=self._experiment.parameter_space, param_values=param_values)
+        trial = Trial(param_values=param_values, U_value=U)
+        self._experiment.trials[trial.trial_id] = trial
+        return trial.trial_id
+
     def create_new_trial(self, key: PRNGKey, random_explore: bool = False, beta: float = 0.5) -> str:
 
         # Go through trials, and find one with unfilled values. Give that one.
         for trial in sorted(self._experiment.trials.values(), key=lambda t: t.create_dt):
             if len(trial.trial_updates) == 0:
                 return trial.trial_id
```

### Comparing `bojaxns-1.0.4/bojaxns/tests/test_experiment.py` & `bojaxns-1.0.5/bojaxns/tests/test_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from jax import numpy as jnp
 
-from bojaxns.experiment import Trial, FloatValue, IntValue, OptimisationExperiment, \
+from bojaxns.common import FloatValue, IntValue
+from bojaxns.experiment import Trial, OptimisationExperiment, \
     TrialUpdate
 from bojaxns.parameter_space import Parameter, IntegerPrior, CategoricalPrior, ParameterSpace, \
     ContinuousPrior
 from bojaxns.utils import current_utc
 
 
 def test_optimisation_experiment():
```

### Comparing `bojaxns-1.0.4/bojaxns/tests/test_parameter_space.py` & `bojaxns-1.0.5/bojaxns/tests/test_parameter_space.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from jax import vmap, random, numpy as jnp
-from jaxns.prior import transform, parse_prior
-from jaxns.types import float_type
 
+from bojaxns.common import FloatValue, IntValue
 from bojaxns.parameter_space import IntegerPrior, CategoricalPrior, ParameterSpace, \
-    Parameter, build_prior_model, ContinuousPrior
+    Parameter, build_prior_model, ContinuousPrior, sample_U_value
 from bojaxns.utils import build_example
+from jaxns.prior import transform, parse_prior
+from jaxns.types import float_type
 
 
 def test_serialisation():
     for m in [
         IntegerPrior,
         CategoricalPrior,
         ContinuousPrior
@@ -72,14 +73,41 @@
     assert jnp.all(x >= 0)
     assert jnp.all(x <= 2)
     assert jnp.any(x == 0)
     assert jnp.any(x == 1)
     assert jnp.any(x == 2)
 
 
+def test_decision_variable():
+    def _sample_prior(key, prior_model):
+        U_placeholder, X_placeholder = parse_prior(prior_model=prior_model)
+        U_ndims = U_placeholder.size
+        U = random.uniform(key=key, shape=(U_ndims,), dtype=float_type)
+        X = transform(U=U, prior_model=prior_model)
+        return X
+
+    parameter_space = ParameterSpace(parameters=[
+        Parameter(
+            name='categorical',
+            prior=CategoricalPrior(
+                probs=[1., 1.]
+            )
+        )
+    ])
+    prior_model = build_prior_model(parameter_space=parameter_space)
+
+    X = vmap(lambda key: _sample_prior(key=key, prior_model=prior_model))(random.split(random.PRNGKey(42), 1000))
+
+    x = X['categorical']
+    assert jnp.all(x >= 0)
+    assert jnp.all(x <= 1)
+    assert jnp.any(x == 0)
+    assert jnp.any(x == 1)
+
+
 def test_close_to_zero():
     def _sample_prior(key, prior_model):
         U_placeholder, X_placeholder = parse_prior(prior_model=prior_model)
         U_ndims = U_placeholder.size
         U = random.uniform(key=key, shape=(U_ndims,), dtype=float_type)
         X = transform(U=U, prior_model=prior_model)
         return X
@@ -123,7 +151,52 @@
 
     _ = ParameterSpace(parameters=[param1, param2, param3])
     try:
         _ = ParameterSpace(parameters=[param1, param1])
         assert False
     except ValueError as e:
         assert 'parameter names must be unique' in str(e)
+
+
+def test_sample_U_value():
+    param1 = Parameter(
+        name='continuous',
+        prior=build_example(ContinuousPrior)
+    )
+
+    param2 = Parameter(
+        name='integers',
+        prior=build_example(IntegerPrior)
+    )
+
+    param3 = Parameter(
+        name='categorical',
+        prior=build_example(CategoricalPrior)
+    )
+
+    parameter_space = ParameterSpace(parameters=[param1, param2, param3])
+
+    param_values = {
+        'continuous': FloatValue(value=param1.prior.lower),
+        'integers': IntValue(value=param2.prior.lower),
+        'categorical': IntValue(value=0)
+    }
+    U_sample = sample_U_value(key=random.PRNGKey(42), param_space=parameter_space,
+                              param_values=param_values)
+
+    prior_model = build_prior_model(parameter_space=parameter_space)
+    X = transform(U=jnp.asarray(U_sample), prior_model=prior_model)
+    for key in X:
+        assert jnp.allclose(X[key], param_values[key].value)
+
+    param_values = {
+        'continuous': FloatValue(value=param1.prior.upper),
+        'integers': IntValue(value=param2.prior.upper),
+        'categorical': IntValue(value=0)
+    }
+    U_sample = sample_U_value(key=random.PRNGKey(42), param_space=parameter_space,
+                              param_values=param_values)
+
+    prior_model = build_prior_model(parameter_space=parameter_space)
+    X = transform(U=jnp.asarray(U_sample), prior_model=prior_model)
+    for key in X:
+        assert jnp.allclose(X[key], param_values[key].value)
```

### Comparing `bojaxns-1.0.4/bojaxns/tests/test_utils.py` & `bojaxns-1.0.5/bojaxns/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns/utils.py` & `bojaxns-1.0.5/bojaxns/utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.4/bojaxns.egg-info/PKG-INFO` & `bojaxns-1.0.5/bojaxns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bojaxns-1.0.4/bojaxns.egg-info/SOURCES.txt` & `bojaxns-1.0.5/bojaxns.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 ./bojaxns/__init__.py
 ./bojaxns/base.py
 ./bojaxns/basic.py
+./bojaxns/common.py
 ./bojaxns/experiment.py
 ./bojaxns/parameter_space.py
 ./bojaxns/service.py
 ./bojaxns/utils.py
 ./bojaxns.egg-info/PKG-INFO
 ./bojaxns.egg-info/SOURCES.txt
 ./bojaxns.egg-info/dependency_links.txt
```

### Comparing `bojaxns-1.0.4/setup.py` & `bojaxns-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'pydantic'
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='bojaxns',
-      version='1.0.4',
+      version='1.0.5',
       description='Bayesian Optimisation with JAXNS',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/bojaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

